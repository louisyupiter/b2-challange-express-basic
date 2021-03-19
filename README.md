```json
[
	{
		"ID": 1,
		"name": "Alpha",
		"score": 100,
		"class": "satu"
	},
	{
		"ID": 2,
		"name": "Beta",
		"score": 76,
		"class": "dua"
	},
	{
		"ID": 3,
		"name": "Charlie",
		"score": 92,
		"class": "tiga"
	},
	{
		"ID": 4,
		"name": "Delta",
		"score": 71,
		"class": "satu"
	},
	{
		"ID": 5,
		"name": "Echo",
		"score": 80,
		"class": "tiga"
	}
]
```

---

# berdasarkan data JSON diatas, gunakan method GET dan Buatlah endpoint untuk mendapatkan data seperti berikut:

## /students

localhost:3000/students

### mendapatkan data seluruh students

output:

```json
[
  {
		"ID": ...,
		"name": ...,
		"score": ...,
		"class": ...
  },
  {
		"ID": ...,
		"name": ...,
		"score": ...,
		"class": ...
  },
  ...
]
```

---

## /students/:id

### mendapatkan SATU data spesifik sesuai dengan id

localhost:3000/students/1

```json
{
	"ID": 1,
	"name": "Alpha",
	"score": 100,
	"class": "satu"
}
```

---

## /classes

### mendapatkan semua nama kelas

contoh: localhost:3000/classes

```json
{
	"satu": [
		{ "ID": 1, "name": "Alpha", "score": 100 },
		{ "ID": 4, "name": "Delta", "score": 71 }
	],
	"dua": [{ "ID": 2, "name": "Beta", "score": 76 }],
	"tiga": [
		{ "ID": 3, "name": "Charlie", "score": 92 },
		{ "ID": 5, "name": "Echo", "score": 80 }
	]
}
```

---

## /classes/:className

### mendapatkan data member class dari parameter

contoh: localhost:3000/classes/satu

```json
[
	{ "ID": 1, "name": "Alpha", "score": 100 },
	{ ... }
]
```

---

## /top

### mengembalikan 3 data siswa dengan nilai tertinggi

contoh: localhost:3000/top

```json
[
	{
		"ID": 1,
		"name": "Alpha",
		"score": 100,
		"class": "satu"
	},
	{
		"ID": 3,
		"name": "Charlie",
		"score": 92,
		"class": "tiga"
    },
    {...}
]
```

### rules:
- duedate: jumat
- cara pengumpulan: biasa di drive, di folder masing2, buat folder challenge-2, baru masukin disini zip workspace nya (jangan lupa di zip/rar ya). lalu node_module nya tidak perlu dikumpulkan.
