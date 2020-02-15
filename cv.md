# Gulmira Yerzhanova

Contact information: g.t.yerzhanova@gmail.com, 8-701-832-00-08

Fulfilling a childhood dream after many years.

Programming languages: Golang. HTML. CSS. GIT. VSCodium.

My last code:
 ```go
func Atoi(s string) int {
	var itog int
	sum := -1
	var flag bool
	len := 0
	for range s {
		len++
	}
	if len > 0 {
		if (s[0] == 45 || s[0] == 43) && len > 20 || !(s[0] == 45 || s[0] == 43) && len > 19 {
			return 0
		} else {
			for i, r := range s {
				if i == 0 && r == 45 {
					flag = true
					sum++
				}
				if i == 0 && r == 43 {
					sum++
				}
				if r >= 48 && r <= 57 {
					itog = itog*10 + int(r-48)
					sum++
				}
				if i != sum {
					itog = 0
				}
			}
			if flag {
				itog = -itog
			}
			if !flag && itog < 0 || flag && itog > 0 {
				return 0
			}
		}
	}
	return itog
}

```

Education: Alem school student, 2019

Experience: Alem school projects, HTML Academy

Languages: Russian, English