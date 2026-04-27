# kalkulator untuk ceweku tercinta
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kalkulator Proses - Dept. B</title>
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: Arial, sans-serif; background: #f5f5f5; color: #222; padding: 24px 16px; }
  .wrap { max-width: 720px; margin: 0 auto; }
  h1 { font-size: 20px; font-weight: 600; margin-bottom: 4px; }
  .sub { font-size: 13px; color: #666; margin-bottom: 20px; }
  .section { background: #fff; border: 1px solid #e0e0e0; border-radius: 10px; padding: 16px 20px; margin-bottom: 14px; }
  .sec-title { font-size: 12px; font-weight: 600; color: #888; text-transform: uppercase; letter-spacing: .05em; margin-bottom: 12px; }
  .grid2 { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
  .grid3 { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 12px; }
  .field label { font-size: 13px; color: #555; display: block; margin-bottom: 4px; }
  .field input { width: 100%; padding: 8px 10px; border: 1px solid #ccc; border-radius: 6px; font-size: 14px; color: #222; background: #fff; }
  .field input:focus { outline: none; border-color: #378ADD; box-shadow: 0 0 0 2px #378ADD33; }
  .field input[readonly] { background: #f0f0f0; color: #888; }
  .btn { width: 100%; padding: 11px; border: none; border-radius: 8px; background: #378ADD; color: #fff; font-size: 15px; font-weight: 600; cursor: pointer; margin-top: 4px; transition: background .15s; }
  .btn:hover { background: #185FA5; }
  .btn:active { transform: scale(.98); }
  .result-wrap { display: none; margin-top: 16px; }
  .metric-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-bottom: 14px; }
  .metric { background: #f0f6ff; border-radius: 8px; padding: 12px 14px; }
  .metric .mlabel { font-size: 12px; color: #555; margin-bottom: 4px; }
  .metric .mval { font-size: 20px; font-weight: 600; color: #185FA5; }
  .metric .munit { font-size: 12px; color: #888; }
  .table-wrap { overflow-x: auto; }
  table { width: 100%; border-collapse: collapse; font-size: 13px; }
  thead tr { background: #f5f5f5; }
  th { text-align: left; padding: 8px 10px; color: #666; font-weight: 600; font-size: 12px; border-bottom: 1px solid #e0e0e0; }
  td { padding: 8px 10px; color: #222; border-bottom: 1px solid #f0f0f0; }
  tr:last-child td { border-bottom: none; }
  .total-row td { font-weight: 600; background: #f0f6ff; }
  .alert { border-radius: 8px; padding: 10px 14px; font-size: 13px; margin-bottom: 12px; }
  .alert-ok { background: #eaf3de; border: 1px solid #c0dd97; color: #27500a; }
  .alert-warn { background: #fcebeb; border: 1px solid #f7c1c1; color: #a32d2d; }
  .divider { border: none; border-top: 1px solid #e0e0e0; margin: 16px 0; }
  .reset-btn { background: none; border: none; color: #888; font-size: 12px; cursor: pointer; text-decoration: underline; margin-top: 8px; }
  @media (max-width: 480px) {
    .grid2, .grid3 { grid-template-columns: 1fr; }
    .metric-grid { grid-template-columns: 1fr; }
  }
</style>
</head>
<body>
<div class="wrap">
  <h1>Kalkulator metode harga pokok</h1>
  <p class="sub">Departemen B - Metode Weighted Average</p>

  <div class="section">
    <div class="sec-title">Data Produksi (kg)</div>
    <div class="grid3">
      <div class="field"><label>Masuk dari Dept. A</label><input type="number" id="inp_masuk" value="50000" min="0"></div>
      <div class="field"><label>Transfer ke gudang</label><input type="number" id="inp_jadi" value="40000" min="0"></div>
      <div class="field"><label>WIP akhir</label><input type="number" id="inp_wip" value="10000" min="0"></div>
    </div>
  </div>

  <div class="section">
    <div class="sec-title">Tingkat Penyelesaian WIP Akhir</div>
    <div class="grid2">
      <div class="field"><label>BBB Dept. B (%)</label><input type="number" id="inp_pct_bbb" value="80" min="0" max="100"></div>
      <div class="field"><label>Biaya Konversi (%)</label><input type="number" id="inp_pct_kon" value="40" min="0" max="100"></div>
    </div>
  </div>

  <div class="section">
    <div class="sec-title">Biaya Dept. A (Rp)</div>
    <div class="grid2">
      <div class="field"><label>Harga per kg dari Dept. A</label><input type="number" id="inp_ha_perkg" value="3000" min="0"></div>
      <div class="field"><label>Total biaya Dept. A (otomatis)</label><input type="number" id="inp_ha_total" readonly></div>
    </div>
  </div>

  <div class="section">
    <div class="sec-title">Biaya Produksi Dept. B (Rp)</div>
    <div class="grid3">
      <div class="field"><label>Biaya Bahan Baku</label><input type="number" id="inp_bbb" value="17000000" min="0"></div>
      <div class="field"><label>Biaya Tenaga Kerja</label><input type="number" id="inp_btk" value="32000000" min="0"></div>
      <div class="field"><label>Biaya Overhead Pabrik</label><input type="number" id="inp_bop" value="19500000" min="0"></div>
    </div>
  </div>

  <button class="btn" onclick="hitung()">Hitung Sekarang</button>

  <div class="result-wrap" id="resultArea">
    <hr class="divider">
    <div class="alert" id="alertBalance"></div>

  <div class="section">
      <div class="sec-title">Ringkasan Hasil</div>
      <div class="metric-grid">
        <div class="metric">
          <div class="mlabel">HPP per unit Dept. A</div>
          <div class="mval" id="r_hpp_a">-</div>
          <div class="munit">Rp / kg</div>
        </div>
        <div class="metric">
          <div class="mlabel">Biaya Dept. B per unit</div>
          <div class="mval" id="r_biaya_b">-</div>
          <div class="munit">Rp / kg</div>
        </div>
        <div class="metric">
          <div class="mlabel">HPP total per unit (A+B)</div>
          <div class="mval" id="r_hpp_total">-</div>
          <div class="munit">Rp / kg</div>
        </div>
        <div class="metric">
          <div class="mlabel">Total biaya Dept. B</div>
          <div class="mval" id="r_total_b">-</div>
          <div class="munit">Rp</div>
        </div>
      </div>
    </div>

   <div class="section">
      <div class="sec-title">Tabel Unit Ekuivalen</div>
      <div class="table-wrap">
        <table>
          <thead><tr><th>Elemen Biaya</th><th>Unit Selesai</th><th>WIP x %</th><th>Total EU</th></tr></thead>
          <tbody id="tbl_eu"></tbody>
        </table>
      </div>
    </div>

  <div class="section">
      <div class="sec-title">Tabel Biaya per Unit</div>
      <div class="table-wrap">
        <table>
          <thead><tr><th>Elemen</th><th>Total Biaya</th><th>Unit Ekuivalen</th><th>Biaya / Unit</th></tr></thead>
          <tbody id="tbl_biaya"></tbody>
        </table>
      </div>
    </div>

   <div class="section">
      <div class="sec-title">Verifikasi Balance</div>
      <div class="table-wrap">
        <table>
          <thead><tr><th>Komponen</th><th>Nilai (Rp)</th></tr></thead>
          <tbody id="tbl_verify"></tbody>
        </table>
      </div>
    </div>

   <button class="reset-btn" onclick="resetForm()">Reset ke nilai awal</button>
  </div>
</div>

<script>
  const fmt = (n) => Math.round(n).toLocaleString('id-ID');
  const fmtDec = (n) => parseFloat(n.toFixed(2)).toLocaleString('id-ID', { minimumFractionDigits: 2, maximumFractionDigits: 2 });

  document.getElementById('inp_masuk').addEventListener('input', autoTotal);
  document.getElementById('inp_ha_perkg').addEventListener('input', autoTotal);

  function autoTotal() {
    const m = +document.getElementById('inp_masuk').value || 0;
    const p = +document.getElementById('inp_ha_perkg').value || 0;
    document.getElementById('inp_ha_total').value = m * p;
  }
  autoTotal();

  function hitung() {
    const masuk   = +document.getElementById('inp_masuk').value || 0;
    const jadi    = +document.getElementById('inp_jadi').value || 0;
    const wip     = +document.getElementById('inp_wip').value || 0;
    const pctBBB  = (+document.getElementById('inp_pct_bbb').value || 0) / 100;
    const pctKon  = (+document.getElementById('inp_pct_kon').value || 0) / 100;
    const haPerkg = +document.getElementById('inp_ha_perkg').value || 0;
    const haTot   = masuk * haPerkg;
    const bbb     = +document.getElementById('inp_bbb').value || 0;
    const btk     = +document.getElementById('inp_btk').value || 0;
    const bop     = +document.getElementById('inp_bop').value || 0;

    const alertEl = document.getElementById('alertBalance');
    if (jadi + wip === masuk) {
      alertEl.className = 'alert alert-ok';
      alertEl.innerHTML = 'Unit balance: ' + fmt(masuk) + ' = ' + fmt(jadi) + ' + ' + fmt(wip) + ' ✓';
    } else {
      alertEl.className = 'alert alert-warn';
      alertEl.innerHTML = 'Perhatian: unit tidak balance. ' + fmt(jadi) + ' + ' + fmt(wip) + ' = ' + fmt(jadi + wip) + ' tidak sama dengan ' + fmt(masuk);
    }

    const eu_a   = jadi + wip * 1;
    const eu_bbb = jadi + wip * pctBBB;
    const eu_kon = jadi + wip * pctKon;

    const hpp_a_unit = eu_a > 0 ? haTot / eu_a : 0;
    const bbb_unit   = eu_bbb > 0 ? bbb / eu_bbb : 0;
    const btk_unit   = eu_kon > 0 ? btk / eu_kon : 0;
    const bop_unit   = eu_kon > 0 ? bop / eu_kon : 0;
    const kon_unit   = btk_unit + bop_unit;
    const totalB_unit = bbb_unit + kon_unit;
    const hppTotal    = hpp_a_unit + totalB_unit;
    const totalBiayaB = bbb + btk + bop;

    document.getElementById('r_hpp_a').textContent     = fmtDec(hpp_a_unit);
    document.getElementById('r_biaya_b').textContent   = fmtDec(totalB_unit);
    document.getElementById('r_hpp_total').textContent = fmtDec(hppTotal);
    document.getElementById('r_total_b').textContent   = fmt(totalBiayaB);

    document.getElementById('tbl_eu').innerHTML = `
      <tr><td>Biaya Dept. A</td><td>${fmt(jadi)}</td><td>${fmt(wip)} x 100%</td><td><b>${fmt(eu_a)}</b></td></tr>
      <tr><td>BBB Dept. B</td><td>${fmt(jadi)}</td><td>${fmt(wip)} x ${(pctBBB * 100).toFixed(0)}%</td><td><b>${fmt(eu_bbb)}</b></td></tr>
      <tr><td>Biaya Konversi (BTK+BOP)</td><td>${fmt(jadi)}</td><td>${fmt(wip)} x ${(pctKon * 100).toFixed(0)}%</td><td><b>${fmt(eu_kon)}</b></td></tr>
    `;

    document.getElementById('tbl_biaya').innerHTML = `
      <tr><td>Biaya Dept. A</td><td>Rp ${fmt(haTot)}</td><td>${fmt(eu_a)} kg</td><td>Rp ${fmtDec(hpp_a_unit)}</td></tr>
      <tr><td>BBB Dept. B</td><td>Rp ${fmt(bbb)}</td><td>${fmt(eu_bbb)} kg</td><td>Rp ${fmtDec(bbb_unit)}</td></tr>
      <tr><td>BTK Dept. B</td><td>Rp ${fmt(btk)}</td><td>${fmt(eu_kon)} kg</td><td>Rp ${fmtDec(btk_unit)}</td></tr>
      <tr><td>BOP Dept. B</td><td>Rp ${fmt(bop)}</td><td>${fmt(eu_kon)} kg</td><td>Rp ${fmtDec(bop_unit)}</td></tr>
      <tr class="total-row"><td>Total HPP per unit</td><td>-</td><td>-</td><td>Rp ${fmtDec(hppTotal)}</td></tr>
    `;

    const nilaiJadi = jadi * hppTotal;
    const wipA      = wip * hpp_a_unit;
    const wipBBB    = wip * pctBBB * bbb_unit;
    const wipKon    = wip * pctKon * kon_unit;
    const nilaiWip  = wipA + wipBBB + wipKon;
    const totalMasuk  = haTot + totalBiayaB;
    const totalKeluar = nilaiJadi + nilaiWip;

    document.getElementById('tbl_verify').innerHTML = `
      <tr><td>Total biaya masuk (Dept. A + B)</td><td>Rp ${fmt(totalMasuk)}</td></tr>
      <tr><td>Nilai produk jadi (${fmt(jadi)} kg x Rp ${fmtDec(hppTotal)})</td><td>Rp ${fmt(nilaiJadi)}</td></tr>
      <tr><td>Nilai WIP akhir</td><td>Rp ${fmt(nilaiWip)}</td></tr>
      <tr class="total-row"><td>Total keluar</td><td>Rp ${fmt(totalKeluar)}</td></tr>
      <tr><td>Selisih (pembulatan)</td><td>Rp ${fmt(Math.abs(totalMasuk - totalKeluar))}</td></tr>
    `;

    document.getElementById('resultArea').style.display = 'block';
  }

  function resetForm() {
    document.getElementById('inp_masuk').value   = 50000;
    document.getElementById('inp_jadi').value    = 40000;
    document.getElementById('inp_wip').value     = 10000;
    document.getElementById('inp_pct_bbb').value = 80;
    document.getElementById('inp_pct_kon').value = 40;
    document.getElementById('inp_ha_perkg').value= 3000;
    document.getElementById('inp_bbb').value     = 17000000;
    document.getElementById('inp_btk').value     = 32000000;
    document.getElementById('inp_bop').value     = 19500000;
    autoTotal();
    document.getElementById('resultArea').style.display = 'none';
  }
</script>
</body>
</html>
