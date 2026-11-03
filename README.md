# assets

CDN de assets estáticos. Os arquivos são servidos pelo jsDelivr:

```
https://cdn.jsdelivr.net/gh/gabrieldonato-affbr/assets@main/<caminho>
```

## moedas/

Moedas douradas e animação do baú (tigre + coelho).

| Arquivo | Tamanho | Formato |
|---|---|---|
| `moeda-10.webp` | 247 KB | imagem estática |
| `moeda-30.webp` | 256 KB | imagem estática |
| `moeda-60.webp` | 257 KB | imagem estática |
| `moeda-720.mp4` | 404 KB | vídeo 720px 30fps — **use este na web** |
| `moeda-leve.gif` | 2,1 MB | GIF 300px 15fps |
| `moeda-600-leve.webp` | 2,3 MB | WebP animado 600px 24fps |
| `moeda-media.gif` | 4,0 MB | GIF 420px 20fps |
| `moeda-600.webp` | 4,1 MB | WebP animado 600px 24fps |
| `moeda-hd.gif` | 10 MB | GIF 600px 24fps |

### Uso na web

```html
<video src="https://cdn.jsdelivr.net/gh/gabrieldonato-affbr/assets@main/moedas/moeda-720.mp4"
       autoplay loop muted playsinline></video>
```
