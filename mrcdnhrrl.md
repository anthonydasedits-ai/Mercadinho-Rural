<!DOCTYPE html>
<html lang="pt-BR"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Mercadinho Rural – Jogo de fazenda e comércio em pixel art</title>
<link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
<style>
:root{--bg:#fff8e6;--card:#ffffff;--ink:#3b2a1a;--mute:#7a6246;--line:#e3cf9f;--acc:#f4c542;--grass:#5fae48;--dark:#3b2a1a;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#1d2b1f;--card:#2a3a2c;--ink:#fff4d6;--mute:#c9bd9a;--line:#4a5e4c}}
*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{margin:0;background:var(--bg);color:var(--ink);font-family:system-ui,-apple-system,Segoe UI,Roboto,sans-serif;line-height:1.55}
.px{font-family:'Press Start 2P',ui-monospace,monospace;line-height:1.4}
header{position:sticky;top:0;z-index:5;background:var(--dark);color:#fff;display:flex;align-items:center;justify-content:space-between;padding:10px 16px;border-bottom:4px solid #6b4a2b}
header b{font-size:11px}
header a.b{font-size:10px;padding:8px 12px}
.hero{position:relative;text-align:center;padding:56px 18px 120px;background:linear-gradient(#7fd0ff 0%,#bfe9ff 60%,#fff2c2 100%);color:#3b2a1a;overflow:hidden}
.sun{position:absolute;top:26px;right:12%;width:56px;height:56px;background:#ffd84a;box-shadow:0 0 0 8px #ffe98a88}
.cloud{position:absolute;width:70px;height:22px;background:#fff;box-shadow:14px -12px 0 #fff,34px -8px 0 #fff;animation:fl 18s linear infinite}
.cloud.c2{top:90px;left:-80px;animation-duration:26s}.cloud.c1{top:40px;left:-120px}
@keyframes fl{to{transform:translateX(130vw)}}
.hero h1{font-size:clamp(20px,6vw,44px);margin:12px 0;text-shadow:3px 3px 0 #fff,6px 6px 0 #f4c542}
.hero p{max-width:560px;margin:0 auto 24px;font-size:17px}
.b{display:inline-block;background:var(--acc);color:#3b2a1a;text-decoration:none;font-weight:800;border:4px solid #3b2a1a;box-shadow:4px 4px 0 #3b2a1a;padding:14px 22px;font-size:13px}
.b:active{transform:translate(3px,3px);box-shadow:1px 1px 0 #3b2a1a}
.b.big{font-size:14px;padding:18px 28px}
.field{position:absolute;left:0;right:0;bottom:0;height:90px;background:var(--grass);border-top:8px solid #4a9a3a;display:flex;justify-content:space-around;align-items:flex-start;font-size:34px;padding-top:6px}
.field span{animation:bob 2.4s ease-in-out infinite}.field span:nth-child(2n){animation-delay:.6s}.field span:nth-child(3n){animation-delay:1.1s}
@keyframes bob{50%{transform:translateY(-6px)}}
section{max-width:960px;margin:0 auto;padding:44px 18px}
h2{font-size:clamp(13px,3.6vw,18px);margin:0 0 22px;text-align:center}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(210px,1fr));gap:14px}
.card{background:var(--card);border:3px solid var(--line);padding:16px;box-shadow:4px 4px 0 var(--line)}
.card .e{font-size:30px}.card h3{margin:6px 0 4px;font-size:16px}.card p{margin:0;color:var(--mute);font-size:14px}
.steps{display:flex;flex-direction:column;gap:10px;max-width:640px;margin:0 auto}
.steps div{display:flex;gap:12px;align-items:center;background:var(--card);border:3px solid var(--line);padding:10px 14px}
.steps b{background:var(--acc);color:#3b2a1a;min-width:30px;height:30px;display:grid;place-items:center;font-size:12px}
.lv{display:flex;flex-wrap:wrap;justify-content:center;gap:8px;align-items:center}
.lv span{background:var(--card);border:3px solid var(--line);padding:10px 12px;font-size:9px}
.ctl{display:flex;flex-wrap:wrap;gap:14px;justify-content:center}
.ctl .card{flex:1 1 220px;text-align:center}
.cta{text-align:center;background:var(--dark);color:#fff;padding:50px 18px}
.cta h2{color:#ffd84a}
footer{text-align:center;padding:18px;font-size:13px;color:var(--mute)}
</style></head><body>
<header><b class="px">🌽 MERCADINHO RURAL</b><a class="b px" href="#jogar">JOGAR</a></header>

<div class="hero">
 <div class="sun"></div><div class="cloud c1"></div><div class="cloud c2"></div>
 <div class="px" style="font-size:11px">JOGO INDIE · PIXEL ART · GRÁTIS</div>
 <h1 class="px">MERCADINHO<br>RURAL</h1>
 <p>Plante, colha, cuide dos animais e venda tudo no seu mercadinho. Comece com uma barraca e construa um hipermercado!</p>
 <a class="b big px" href="https://claude.ai/artifact/CmepxJAM4qmBCxRkYM3D49" target="_blank" rel="noopener">▶ JOGAR AGORA</a>
 <div class="field"><span>🥕</span><span>🍅</span><span>🌽</span><span>🐄</span><span>🥔</span><span>🐔</span><span>🍓</span><span>🐑</span></div>
</div>

<section>
 <h2 class="px">O QUE VOCÊ VAI FAZER</h2>
 <div class="grid">
  <div class="card"><div class="e">🌱</div><h3>Plantar e colher</h3><p>Cenoura, tomate, milho, batata e morango. Cada planta cresce em fases e precisa de água.</p></div>
  <div class="card"><div class="e">🏪</div><h3>Vender na loja</h3><p>Coloque os produtos nas prateleiras e veja os clientes escolherem e pagarem no caixa.</p></div>
  <div class="card"><div class="e">🐄</div><h3>Criar animais</h3><p>Vacas dão leite, galinhas dão ovos, ovelhas dão lã e porcos acham trufas.</p></div>
  <div class="card"><div class="e">🚚</div><h3>Entregas</h3><p>Receba pedidos no caminhão e ganhe moedas extras por cada entrega.</p></div>
  <div class="card"><div class="e">🌧️</div><h3>Dia, noite e chuva</h3><p>O tempo muda sozinho. A chuva rega as plantações pra você.</p></div>
  <div class="card"><div class="e">💾</div><h3>Salva sozinho</h3><p>Moedas, inventário, plantações e melhorias ficam guardados no seu aparelho.</p></div>
 </div>
</section>

<section>
 <h2 class="px">COMO JOGAR</h2>
 <div class="steps">
  <div><b class="px">1</b>Compre sementes no 🛒 Menu e selecione no inventário.</div>
  <div><b class="px">2</b>Ande até um terreno e toque no botão A para plantar e regar.</div>
  <div><b class="px">3</b>Quando estiver pronto, colha com o botão A.</div>
  <div><b class="px">4</b>Entre na loja e coloque os produtos nas prateleiras.</div>
  <div><b class="px">5</b>Use as moedas para melhorar a loja e comprar animais.</div>
 </div>
</section>

<section>
 <h2 class="px">CRESÇA SEU NEGÓCIO</h2>
 <div class="lv"><span class="px">BARRACA</span>➜<span class="px">MERCADINHO</span>➜<span class="px">SUPERMERCADO</span>➜<span class="px">HIPERMERCADO</span></div>
</section>

<section>
 <h2 class="px">CONTROLES</h2>
 <div class="ctl">
  <div class="card"><div class="e">📱</div><h3>No celular</h3><p>Gire o aparelho para deitado. Analógico à esquerda e botão A à direita.</p></div>
  <div class="card"><div class="e">⌨️</div><h3>No computador</h3><p>Setas ou WASD para andar. Espaço ou E para agir. M abre o menu.</p></div>
 </div>
</section>

<div class="cta" id="jogar">
 <h2 class="px">PRONTO PRA PLANTAR?</h2>
 <p style="margin:0 0 22px">Abra o jogo e comece com 100 moedas, 5 sementes de cenoura e 2 de tomate.</p>
 <a class="b big px" href="https://claude.ai/artifact/CmepxJAM4qmBCxRkYM3D49" target="_blank" rel="noopener">▶ JOGAR AGORA</a>
</div>
<footer>© 2026 Mercadinho Rural · Feito com ♥ e muito pixel</footer>
</body></html>
