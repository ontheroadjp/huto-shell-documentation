# Toybox Hugo Documentaion

## Getting Start

### Initialize Hugo Site
```bash
sh bin/init.sh
```

### Start Hugo server
```bash
cd site
docker-compose up -d
```

## Create New document

### Create new section
```bash
cd site
sh bin/section <section name>
```

### Create content
```bash
sh bin/post <section name>/<post name>.md
```

## Theme

[matcornic/hugo-theme-learn](https://github.com/matcornic/hugo-theme-learn)
