# TrioGrip

Instrumento musical em software para o celular: guitarra, baixo ou bateria de um **power trio**. Blues e rock and roll. Áudio local (Web Audio). Sem build, sem conta, sem telemetria.

Página: [steixeiradecarvalho.github.io/TrioGrip](https://steixeiradecarvalho.github.io/TrioGrip/)  
Instrumento: [app.html](https://steixeiradecarvalho.github.io/TrioGrip/app.html)

## O que é

Um telefone em paisagem, duas mãos. Cinco graus de escala (pentatônica menor, blues ou mixolídia). Palhetada. Inclinação para bend. Três papéis no mesmo código. Perfis Cream, Hendrix e ZZ Top.

Não é DAW, não é escola gamificada, não é jam na nuvem. O som nasce no aparelho. A rede local, se houver, só carrega o pulso.

## Arquivos

| Arquivo | Função |
|---|---|
| `index.html` | Landing / apresentação |
| `app.html` | O instrumento |
| `primeira-peca.html` | Tutorial do primeiro uso (8 compassos em Lá) |
| `LICENSE` | MIT |

## Como rodar

Abra `app.html` no Chrome do celular (paisagem). Melhor servir por HTTP — sensores e `AudioContext` falham com frequência em `file://`:

```bash
python3 -m http.server 8080
```

No telefone: `http://IP-DA-MAQUINA:8080/app.html`.

## GitHub Pages

Settings → Pages → Deploy from branch `main` / root.  
URL esperada: `https://<usuario>.github.io/TrioGrip/`.

## Princípios para contribuir

1. Áudio no dispositivo. Não enviar waveform pela rede.
2. Tocabilidade em hardware modesto (o modo leve existe por causa de um Galaxy A20).
3. Vocabulário reduzido: escala trancada, alvos grandes, duas mãos.
4. Sem dependências de build no núcleo do instrumento.

Relatos de tocabilidade (o que o corpo não entendeu) valem mais que features.

## Licença

MIT. Veja `LICENSE`.
