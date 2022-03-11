![Flowtron](https://nv-adlr.github.io/images/flowtron_logo.png "Flowtron")

## Flowtron: Autoregresyjna sieć oparta na przepływie do syntezy tekstu na spektrogramy Mel

### Rafael Valle, Kevin Shih, Ryan Prenger and Bryan Catanzaro

W naszym ostatnim [artykule] proponujemy Flowtron: autoregresyjną sieć generatywną
opartą na przepływach generatywną sieć do syntezy tekstu na mowę z kontrolą
zmiennością mowy i transferem stylu. Flowtron zapożycza wiedzę z przepływów autoregresyjnych
i przekształca [Tacotron] w celu zapewnienia wysokiej jakości i ekspresyjnej syntezy mel-spektrogramu.
Flowtron jest optymalizowany poprzez maksymalizację prawdopodobieństwa danych treningowych,
co sprawia, że trening jest prosty i stabilny. Flowtron uczy się odwracalnego
odwzorowania danych na przestrzeń ukrytą, która może być wykorzystywana do sterowania
wieloma aspektami syntezy mowy (wysokość, ton, tempo mowy, kadencja, akcent).

Nasze średnie wyniki opinii (MOS) pokazują, że Flowtron dorównuje najnowocześniejszym modelom TTS
pod względem jakości mowy. Ponadto, przedstawiamy wyniki dotyczące kontroli
zmienności mowy, interpolacji między próbkami i transferu stylu między
mówcami widzianymi i niewidzianymi podczas treningu.

Odwiedź naszą [stronę], by posłuchać przykładowych próbek dźwiękowych.


## Powiązane repozytoria
[WaveGlow](https://github.com/NVIDIA/WaveGlow) Szybsza niż w czasie rzeczywistym
sieć generatywna oparta na przepływie do syntezy mowy

## Podziękowanie
Ta implementacja używa kodu z następujących repozytoriów: [Keith
Ito](https://github.com/keithito/tacotron/), [Prem
Seetharaman](https://github.com/pseeth/pytorch-stft) i [Liyuan Liu](https://github.com/LiyuanLucasLiu/RAdam) zgodnie z opisem w naszym kodzie.

[ignored]: https://github.com/NVIDIA/flowtron/config.json#L12
[artykule]: https://arxiv.org/abs/2005.05957
[Flowtron LJS]: https://drive.google.com/open?id=1Cjd6dK_eFz6DE0PKXKgKxrzTUqzzUDW-
[Flowtron LibriTTS]: https://drive.google.com/open?id=1KhJcPawFgmfvwV7tQAOeC253rYstLrs8
[Flowtron LibriTTS2K]: https://drive.google.com/open?id=1sKTImKkU0Cmlhjc_OeUDLrOLIXvUPwnO
[WaveGlow]: https://drive.google.com/open?id=1rpK8CzAAirq9sWZhe9nlfvxMF1dRgFbF
[PyTorch]: https://github.com/pytorch/pytorch#installation
[stronę]: https://nv-adlr.github.io/Flowtron
[AMP]: https://github.com/NVIDIA/apex/tree/master/apex/amp
[Tacotron]: https://arxiv.org/abs/1712.05884
