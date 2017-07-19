all: 20170719_PJLConfiance_AmendementsHemicycle.pdf 20170719_PJLConfiance_AmendementsHemicycle.odt 20170719_PJLConfiance_AmendementsHemicycle.doc

20170719_PJLConfiance_AmendementsHemicycle.pdf: 20170719_PJLConfiance_AmendementsHemicycle.md confiance_transparence.png header.md
	cat header.md 20170719_PJLConfiance_AmendementsHemicycle.md | sed 's/^\(#[^#]\)/\\newpage\n\n\1/' | pandoc -V papersize=a4 -V lang=fr -s -S --toc --toc-depth=1 -o 20170719_PJLConfiance_AmendementsHemicycle.pdf /dev/stdin

20170719_PJLConfiance_AmendementsHemicycle.odt: 20170719_PJLConfiance_AmendementsHemicycle.pdf
	cat header.md 20170719_PJLConfiance_AmendementsHemicycle.md | sed 's/^\(#[^#]\)/\\newpage\n\n\1/' | pandoc -V papersize=a4 -V lang=fr -s -S --toc --toc-depth=1 -o 20170719_PJLConfiance_AmendementsHemicycle.odt /dev/stdin

20170719_PJLConfiance_AmendementsHemicycle.doc: 20170719_PJLConfiance_AmendementsHemicycle.pdf
	cat header.md 20170719_PJLConfiance_AmendementsHemicycle.md | sed 's/^\(#[^#]\)/\\newpage\n\n\1/' | pandoc -V papersize=a4 -V lang=fr -s -S --toc --toc-depth=1 -o 20170719_PJLConfiance_AmendementsHemicycle.doc /dev/stdin
