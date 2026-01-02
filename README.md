/* =========================
   GENEL
   ========================= */
* { box-sizing: border-box; }

.search-th{
  text-align:center;
  vertical-align: middle;
}

.search-input{
  margin: 0 auto;
  width: clamp(7rem, 10vw, 10rem); /* 120px yerine */
  height: 1.6rem;                  /* 24px yerine */
  text-align:center;
}

/* =========================
   INFO POPUP
   ========================= */
.info-box {
  position: relative;
  display: inline-block;
}

.info-popup {
  position:absolute;
  top:0;
  left:0;
  display:none;
  background:white;
  border:1px solid #ccc;

  width: min(26rem, 90vw);   /* 400px yerine */
  height: auto;              /* 238px yerine */
  max-height: 14rem;         /* taşarsa scroll */
  overflow: auto;

  padding:0;
  line-height: 1;
  z-index: 1000;
  vertical-align: middle;
}

.info-popup table{
  border-collapse:collapse;
  border-spacing:0;
  width:100%;
  table-layout: fixed;
  margin:0;
}

/* =========================
   BOŞ KAYIT ALANLARI
   ========================= */
.no-records,
.no-records-efficiency{
  min-height: 12.5rem;       /* 200/207px yerine */
  vertical-align: middle;
  font-size: 1.2rem;
  color: #6c757d;
}

/* =========================
   TEXT TRUNCATE
   ========================= */
.truncate{
  max-width: 12.5rem;        /* 200px yerine */
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.truncate-cell{
  max-width: 12.5rem;
  white-space: nowrap;       /* sende nokta yanlış yazılmış: white-space.nowrap */
  overflow:hidden;
  text-overflow: ellipsis;
  display: inline-block;
  vertical-align: middle;
}

/* =========================
   TABLO SCROLL + STICKY HEADER
   ========================= */
.emir{
  display:block;
  max-height: none;          /* 250px kilidini aç */
  overflow-y:auto;
  min-height: 0;
}

thead th {
  position: sticky;
  top:0;
  z-index:1;
}

/* =========================
   PAGE LAYOUT (EN KRİTİK)
   ========================= */
.container {
  padding: 1.25rem;          /* 20px -> rem */
  display: flex;
  flex-direction: column;
  gap: 1.25rem;              /* 20px -> rem */
  min-height: 0;
}

/* header sabit olmasın; içerik büyürse genişleyebilsin */
.header-box {
  min-height: 3.75rem;       /* 60px -> min-height */
  height: auto;
}

/* DPI artınca sığmazsa alt satıra geçsin */
.grid-row {
  display: flex;
  gap: 0.75rem;              /* 10px -> rem */
  flex-wrap: wrap;
  min-width: 0;
}

.grid-7-col > div {
  flex: 1 1 10rem;           /* sabit 80px yerine esnek */
  min-height: 5rem;          /* 80px -> min-height */
}

/* alt satır */
.lower-row {
  display: flex;
  gap: 0.75rem;
  margin-top: 0.75rem;
  flex-wrap: wrap;
  min-width: 0;
}

/* tablo kutusu: sabit height yok */
.table-box {
  flex: 1 1 0;
  height: auto;              /* 250px kilidi kaldır */
  min-height: 12rem;         /* taban yükseklik */
  min-width: 0;
  min-height: 0;
}

/* 50vh KİLİDİNİ AÇTIK: zoom’da içerik sığmazsa büyüsün */
.half {
  display: flex;
  width: 100%;
  gap: 0.75rem;
  height: auto;              /* 50vh yerine */
  min-height: 0;
  flex-wrap: wrap;           /* yan yana sığmazsa alt satıra */
}

/* kutular */
.box {
  flex: 1 1 20rem;           /* sığmazsa kır */
  margin: 0.75rem;
  border: none;
  max-height: none;          /* 278px kilidi kaldır */
  min-width: 0;
  min-height: 0;
}

/* scroll alanı: kutunun içinde scroll, px kilidi yok */
.scroll{
  display:block;
  overflow: auto;
  max-height: none;          /* 278px kilidi kaldır */
  min-height: 0;
}

/* =========================
   DİĞER
   ========================= */
.pointer { cursor:pointer; }

.square-big {
  font-size:300%;
  font-weight:bold;
}

.square {
  font-size:200%;
  font-weight:bold;
}

.box-title {
  flex: 1;
  margin-right: 0.75rem;
  margin-left: 0.75rem;
  margin-top: 0.75rem;
}

.ratio-box {
  flex: 1;
  margin: 0.75rem;
}

.no-hover:hover{
  background-color: #c8e6ec !important;
  box-shadow: #c8e6ec !important;
  border-color: #c8e6ec !important;
}

/* =========================
   STATUS BADGE
   ========================= */
.status-badge{
  display:inline-block;
  padding: 0.25rem 0.625rem; /* 4px 10px -> rem */
  border-radius: 0.75rem;
  font-size:0.85rem;
  font-weight:600;
  border: 1.5px solid;
  min-width: 5.6rem;         /* 90px -> rem */
  text-align:center;
}

.status-done {
  color: #155724;
  background-color:rgb(201, 249, 214);
  border-color:rgb(159, 215, 176);
}

.status-pending {
  color: #856404;
  background-color: #fff9e6;
  border-color: #ffe8a1;
}

.status-error {
  color:rgb(103, 23, 30);
  background-color:rgb(249, 194, 198);
  border-color: #f1b0b7;
}
