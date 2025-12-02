<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Monitoring Kesehatan Pernapasan - Breathery</title>
  <style>
    body {
      font-family: "Poppins", sans-serif;
      background-color: #f7f3fa;
      color: #4a306d;
      text-align: center;
      margin: 0;
      padding: 20px;
    }
    header {
      background-color: #cdb4db;
      color: #fff;
      padding: 20px;
      border-radius: 0 0 20px 20px;
    }
    section {
      margin: 30px auto;
      width: 90%;
      max-width: 720px;
      background: #fff;
      padding: 25px;
      border-radius: 15px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      position: relative;
      overflow: hidden;
      text-align: left;
    }
    #halamanInformasi {
      background-image: url('https://rsko-jakarta.com/rahasia/assets/upload/Desain_tanpa_judul_(26).png');
      background-size: cover;
      background-position: center;
    }
    /* overlay tipis agar teks tetap terbaca; jika ingin hilang, ubah alpha */
    #halamanInformasi::before {
      content: "";
      position: absolute;
      inset: 0;
      background: rgba(255,255,255,0.60);
      border-radius: 15px;
      z-index: 1;
    }
    #halamanInformasi * { position: relative; z-index: 2; }
    select, button {
      width: 100%;
      padding: 10px;
      margin-top: 10px;
      border-radius: 8px;
      border: 1px solid #b495c9;
      font-size: 15px;
    }
    button {
      background-color: #b495c9;
      color: white;
      font-weight: bold;
      cursor: pointer;
    }
    button:hover { background-color: #9c7ebd; }
    #infoPenyakit {
      margin-top: 20px;
      background: #f5edfa;
      padding: 15px;
      border-radius: 10px;
      text-align: left;
    }
    .hidden { display: none; }
    .pertanyaan { text-align: left; margin: 12px 0; }
    .pertanyaan label { margin-right: 12px; cursor: pointer; }
    .hasil-card {
      background: linear-gradient(180deg,#fff,#fbf8ff);
      border-radius: 12px;
      padding: 16px;
      border: 1px solid rgba(148,122,189,0.12);
    }
    .hasil-title { color: #4a306d; font-weight: 700; margin-bottom: 8px; }
  </style>
</head>
<body>

  <header>
    <h1> ╭────╮<br>Breathery<br>╰────╯ </h1>
    <p>Pelajari penyakit pernapasan dan lakukan tes kesehatanmu!</p>
  </header>

  <!-- HALAMAN INFORMASI -->
  <section id="halamanInformasi">
    <h2>🫁 Informasi Penyakit Pernapasan</h2>
    <p>Pilih penyakit untuk melihat informasinya:</p>

    <select id="penyakitSelect">
      <option value="">-- Pilih penyakit --</option>
      <option value="asma">Asma</option>
      <option value="bronkitis">Bronkitis</option>
      <option value="ppok">PPOK</option>
      <option value="kanker">Kanker Paru-Paru</option>
      <option value="pneumonia">Pneumonia</option>
    </select>

    <div id="infoPenyakit" class="hidden"></div>

    <br>
    <button onclick="bukaTes()">🩺 Tes Kesehatan Pernapasan</button>
  </section>

  <!-- HALAMAN TES -->
  <section id="halamanTes" class="hidden">
    <h2>🩺 Tes Kesehatan Pernapasan</h2>
    <p>Jawab pertanyaan berikut dengan memilih <strong>Yes</strong> atau <strong>No</strong>.</p>

    <form id="formTes">
      <div class="pertanyaan">
        1. Apakah Anda mengalami batuk berkepanjangan?
        <br>
        <label><input type="radio" name="batuk" value="yes"> Yes</label>
        <label><input type="radio" name="batuk" value="no"> No</label>
      </div>

      <div class="pertanyaan">
        2. Apakah Anda mengalami sesak napas?
        <br>
        <label><input type="radio" name="sesak" value="yes"> Yes</label>
        <label><input type="radio" name="sesak" value="no"> No</label>
      </div>

      <div class="pertanyaan">
        3. Apakah Anda mudah lelah saat aktivitas ringan?
        <br>
        <label><input type="radio" name="lelah" value="yes"> Yes</label>
        <label><input type="radio" name="lelah" value="no"> No</label>
      </div>

      <div class="pertanyaan">
        4. Apakah Anda sering terpapar debu atau polusi setiap hari?
        <br>
        <label><input type="radio" name="debu" value="yes"> Yes</label>
        <label><input type="radio" name="debu" value="no"> No</label>
      </div>

      <div class="pertanyaan">
        5. Apakah Anda mengalami demam atau meningkatnya suhu badan baru-baru ini?
        <br>
        <label><input type="radio" name="demam" value="yes"> Yes</label>
        <label><input type="radio" name="demam" value="no"> No</label>
      </div>

      <div class="pertanyaan">
        6. Apakah Anda merasakan nyeri atau sakit pada dada saat bernapas?
        <br>
        <label><input type="radio" name="nyeri" value="yes"> Yes</label>
        <label><input type="radio" name="nyeri" value="no"> No</label>
      </div>

      <button type="submit">Lihat Hasil Tes</button>
    </form>
  </section>

  <!-- HALAMAN HASIL -->
  <section id="halamanHasil" class="hidden">
    <h2>📊 Hasil Tes & Saran</h2>
    <div id="hasil"></div>
    <br>
    <button onclick="kembaliHome()">⬅️ Kembali ke Halaman Utama</button>
  </section>

<script>
/* ---------------------- DATA INFORMASI & SARAN ---------------------- */
const penyakitData = {
  asma: {
    info: `
      <b>Asma</b> adalah penyakit kronis pada saluran pernapasan yang ditandai dengan penyempitan dan peradangan saluran napas.
      <br><br><b>Gejala:</b><br>
      • Sesak napas<br>• Batuk berulang terutama malam/dini hari<br>• Mengi (ngik-ngik)<br>• Dada terasa berat<br>• Mudah lelah<br>
      <br><b>Penyebab:</b><br>
      • Riwayat keluarga, alergi (debu, bulu hewan), paparan asap rokok & polusi
    `,
    saran: `Gunakan masker saat udara buruk, hindari pemicu seperti debu dan asap rokok, siapkan inhaler jika diresepkan dokter, dan lakukan olahraga pernapasan secara teratur.`
  },
  bronkitis: {
    info: `
      <b>Bronkitis</b> adalah peradangan pada saluran bronkus yang menyebabkan produksi lendir berlebih.
      <br><br><b>Gejala:</b><br>
      • Batuk berdahak lama<br>• Sesak napas<br>• Dada berat/nyeri<br>• Demam ringan<br>
      <br><b>Penyebab:</b><br>
      • Infeksi virus/bakteri, paparan asap rokok, polusi
    `,
    saran: `Jalani vaksinasi jika direkomendasikan, hindari paparan asap rokok, gunakan masker saat polusi, batasi kontak dengan orang sakit, dan istirahat bila perlu.`
  },
  ppok: {
    info: `
      <b>PPOK</b> adalah penyakit paru kronis yang menyebabkan penyumbatan aliran udara secara permanen.
      <br><br><b>Gejala:</b><br>
      • Sesak berkepanjangan<br>• Batuk berdahak kronis<br>• Berat badan menurun<br>
      <br><b>Penyebab:</b><br>
      • Merokok (penyebab utama), paparan asap pembakaran, polusi jangka panjang
    `,
    saran: `Hindari asap rokok sepenuhnya, kurangi aktivitas berat saat polusi tinggi, konsumsi makanan bergizi, dan lakukan latihan pernapasan secara rutin.`
  },
  kanker: {
    info: `
      <b>Kanker Paru-Paru</b> adalah pertumbuhan sel abnormal di paru-paru yang dapat menyebar.
      <br><br><b>Gejala:</b><br>
      • Batuk berkepanjangan<br>• Batuk darah<br>• Nyeri dada<br>• Penurunan berat badan<br>
      <br><b>Penyebab:</b><br>
      • Merokok, paparan zat kimia berbahaya
    `,
    saran: `Berhenti merokok dan hindari asap rokok, lakukan pemeriksaan medis secara rutin, dan jalani pola hidup sehat serta olahraga teratur.`
  },
  pneumonia: {
    info: `
      <b>Pneumonia</b> adalah infeksi pada jaringan paru-paru yang membuat alveoli terisi cairan atau nanah.
      <br><br><b>Gejala:</b><br>
      • Demam tinggi<br>• Batuk berdahak kental<br>• Sesak napas<br>• Nyeri dada saat bernapas<br>
      <br><b>Penyebab:</b><br>
      • Bakteri, virus, jamur; sistem kekebalan lemah
    `,
    saran: `Tingkatkan daya tahan tubuh, jalani vaksinasi bila dianjurkan, jaga kebersihan, istirahat cukup, dan segera periksa ke fasilitas kesehatan bila gejala berat.`
  }
};

/* ---------------------- tampilkan info penyakit saat dipilih ---------------------- */
const penyakitSelect = document.getElementById("penyakitSelect");
const infoPenyakit = document.getElementById("infoPenyakit");

penyakitSelect.addEventListener("change", function () {
  const p = this.value;
  if (p && penyakitData[p]) {
    infoPenyakit.innerHTML = penyakitData[p].info;
    infoPenyakit.classList.remove("hidden");
  } else {
    infoPenyakit.classList.add("hidden");
  }
});

/* ---------------------- navigasi halaman ---------------------- */
function bukaTes() {
  document.getElementById("halamanInformasi").classList.add("hidden");
  document.getElementById("halamanTes").classList.remove("hidden");
  // scroll ke atas agar user melihat form
  window.scrollTo({ top: 0, behavior: "smooth" });
}
function kembaliHome() {
  document.getElementById("halamanHasil").classList.add("hidden");
  document.getElementById("halamanTes").classList.add("hidden");
  document.getElementById("halamanInformasi").classList.remove("hidden");
  window.scrollTo({ top: 0, behavior: "smooth" });
}

/* ---------------------- SKORING (metode A: bobot per gejala) ---------------------- */
/*
  Kita gunakan 6 gejala: batuk, sesak, lelah, debu, demam, nyeri
  Untuk tiap penyakit, tentukan bobot (lebih tinggi = gejala lebih determinan)
  Persentase = (skor_user / total_bobot_penyakit) * 100
*/
const bobotPenyakit = {
  asma:    { batuk: 10, sesak: 30, lelah: 10, debu: 20, demam: 5, nyeri: 5 },   // total 80
  bronkitis:{ batuk: 30, sesak: 15, lelah: 5, debu: 20, demam: 20, nyeri:10 },  // total 100
  ppok:    { batuk: 25, sesak: 30, lelah: 10, debu: 25, demam: 5, nyeri:5 },   // total 100
  pneumonia:{ batuk: 20, sesak: 25, lelah: 20, debu: 5, demam: 25, nyeri:5 },  // total 100
  kanker:  { batuk: 25, sesak: 15, lelah: 10, debu: 10, demam: 5, nyeri:35 }   // total 100 (nyeri/berat badan penting)
};

// fungsi bantu: ambil nilai radio
function getRadioValue(name) {
  const el = document.querySelector("input[name='" + name + "']:checked");
  return el ? el.value : null;
}

// submit form: hitung persentase untuk tiap penyakit, pilih tertinggi
document.getElementById("formTes").addEventListener("submit", function (e) {
  e.preventDefault();

  // ambil jawaban
  const jawaban = {
    batuk: getRadioValue("batuk"),
    sesak: getRadioValue("sesak"),
    lelah: getRadioValue("lelah"),
    debu: getRadioValue("debu"),
    demam: getRadioValue("demam"),
    nyeri: getRadioValue("nyeri")
  };

  // pastikan semua terisi
  for (const k in jawaban) {
    if (jawaban[k] === null) {
      alert("Harap jawab semua pertanyaan sebelum melihat hasil.");
      return;
    }
  }

  // hitung skor per penyakit
  const hasilSkor = {};
  for (const penyakit in bobotPenyakit) {
    let skor = 0;
    const bobot = bobotPenyakit[penyakit];
    for (const g in jawaban) {
      if (jawaban[g] === "yes") {
        skor += (bobot[g] || 0);
      }
    }
    // total bobot maksimal untuk penyakit tersebut:
    const totalBobot = Object.values(bobot).reduce((a,b)=>a+b,0);
    const persen = Math.round((skor / totalBobot) * 100); // 0..100
    hasilSkor[penyakit] = { skor, persen };
  }

  // cari penyakit tertinggi (persen terbesar)
  const entries = Object.entries(hasilSkor).sort((a,b)=> b[1].persen - a[1].persen);
  const top = entries[0]; // [penyakit, {skor, persen}]
  const topName = top[0];
  const topPersen = top[1].persen;

  // Jika semua 0 (tidak ada gejala yes), beri hasil sehat
  const sumPersen = entries.reduce((s, e) => s + e[1].persen, 0);
  let hasilHTML = '';
  if (sumPersen === 0) {
    hasilHTML = `
      <div class="hasil-card">
        <div class="hasil-title">Kesehatan pernapasan Anda tampak baik</div>
        <div>Tidak terdeteksi gejala signifikan berdasarkan jawaban Anda. Lanjutkan pola hidup sehat, hindari polusi, dan periksa berkala bila diperlukan.</div>
      </div>
    `;
  } else {
    // tampilkan ringkasan beberapa kemungkinan teratas (maks 3) + saran khusus untuk top 1
    const topList = entries.slice(0,3);
    let listHTML = '<div class="hasil-card">';
    listHTML += '<div class="hasil-title">Kemungkinan berdasarkan gejala</div>';
    listHTML += '<ul>';
    topList.forEach(item => {
      const name = item[0];
      const p = item[1].persen;
      listHTML += `<li><b>${name.toUpperCase()}</b>: ${p}% kecocokan gejala</li>`;
    });
    listHTML += '</ul>';
    listHTML += `<hr><div><b>Diagnosis sementara (paling tinggi):</b> ${topName.toUpperCase()} — ${topPersen}%</div>`;
    listHTML += `<br><div><b>Saran khusus untuk ${topName.toUpperCase()}:</b><br>${penyakitData[topName].saran}</div>`;
    listHTML += `<br><small>Catatan: Ini adalah evaluasi awal berbasis gejala sederhana. Untuk diagnosis pasti, silakan konsultasi dengan tenaga medis.</small>`;
    listHTML += '</div>';
    hasilHTML = listHTML;
  }

  document.getElementById("hasil").innerHTML = hasilHTML;
  document.getElementById("halamanTes").classList.add("hidden");
  document.getElementById("halamanHasil").classList.remove("hidden");
  window.scrollTo({ top: 0, behavior: "smooth" });
});
</script>

</body>
</html>
