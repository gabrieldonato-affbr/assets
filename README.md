# assets

CDN de assets estáticos. Os arquivos são servidos pelo jsDelivr:

```
https://cdn.jsdelivr.net/gh/gabrieldonato-affbr/assets@main/<caminho>
```

---

## moedas/ — imagens estáticas

Moedas douradas, uma por valor. **São imagens paradas, não animações.**

| Arquivo | Tamanho | Dimensão |
|---|---|---|
| `moedas/moeda-10.webp` | 247 KB | 1254×1254 |
| `moedas/moeda-30.webp` | 256 KB | 1254×1254 |
| `moedas/moeda-60.webp` | 257 KB | 1254×1254 |

---

## bau-animacao/ — animação em loop

Cena animada do baú com o tigre e o coelho, 5 segundos em loop.
Todos os arquivos abaixo são o **mesmo conteúdo**, em formatos e pesos diferentes.

| Arquivo | Tamanho | Dimensão / FPS | Quando usar |
|---|---|---|---|
| `bau-animacao/bau.mp4` | 404 KB | 720px · 30fps | **Padrão para web.** Menor e com melhor qualidade. |
| `bau-animacao/bau-300.gif` | 2,1 MB | 300px · 15fps | WhatsApp, Telegram, e-mail |
| `bau-animacao/bau-600-leve.webp` | 2,3 MB | 600px · 24fps | web, quando MP4 não serve |
| `bau-animacao/bau-420.gif` | 4,0 MB | 420px · 20fps | meio-termo |
| `bau-animacao/bau-600.webp` | 4,1 MB | 600px · 24fps | web, qualidade maior |
| `bau-animacao/bau-600.gif` | 10 MB | 600px · 24fps | onde o peso não importa |

### Uso na web

Prefira o MP4 — é 25x mais leve que o GIF equivalente e tem qualidade melhor.
Com estes atributos ele se comporta como um GIF para o usuário:

```html
<video src="https://cdn.jsdelivr.net/gh/gabrieldonato-affbr/assets@main/bau-animacao/bau.mp4"
       autoplay loop muted playsinline></video>
```

---

## Como adicionar arquivos

1. Copiar para uma subpasta temática deste repositório
2. `git add . && git commit && git push`
3. A URL fica disponível no jsDelivr em segundos, sem build

**O repositório é público.** Nada sensível aqui.

**Cache:** URLs com `@main` ficam em cache por até 7 dias. Para substituir um
arquivo, use um nome novo (`bau-v2.mp4`) ou crie uma tag e referencie `@v2`.
