* {
  box-sizing: border-box;
}

.search-th{
  text-align:center;
  vertical-align: middle;
}

.search-input{
  margin: 0 auto;
  width: clamp(7rem, 10vw, 10rem);
  height: 1.6rem;
  text-align:center;
}

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
  width: min(26rem, 90vw);
  max-height: 14rem;
  overflow: auto;
  padding:0;
  line-height: 1;
  z-index: 1000;
}

.info-popup table{
  border-collapse:collapse;
  width:100%;
  table-layout: fixed;
}

.no-records,
.no-records-efficiency{
  min-height: 8rem;
  font-size: 1.1rem;
  color: #6c757d;
  display:flex;
  align-items:center;
  justify-content:center;
}

.truncate,
.truncate-cell{
  max-width: 12.5rem;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  display:inline-block;
  vertical-align: middle;
}

.container {
  padding: 0.75rem;
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  min-height: 0;
}

.header-box {
  min-height: 3rem;
}

.grid-row,
.lower-row {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
  min-width: 0;
}

.grid-7-col > div {
  flex: 1 1 10rem;
  min-height: 4.5rem;
}

.half {
  display: flex;
  width: 100%;
  gap: 0.5rem;
  flex-wrap: wrap;
  min-height: 0;
}

.box {
  flex: 1 1 20rem;
  border: none;
  margin: 0.25rem;
  min-width: 0;
  min-height: 0;
}

.scroll,
.emir{
  overflow-y: auto;
  overflow-x: auto;
  max-height: clamp(9rem, 26vh, 15rem);
  min-height: 0;
}

thead th {
  position: sticky;
  top: 0;
  z-index: 2;
  background: #fff;
}

.pointer {
  cursor:pointer;
}

.square-big {
  font-size:300%;
  font-weight:bold;
}

.square {
  font-size:200%;
  font-weight:bold;
}

.box-title,
.ratio-box {
  margin: 0.25rem;
  flex: 1;
}

.no-hover:hover{
  background-color: #c8e6ec !important;
  border-color: #c8e6ec !important;
}

.status-badge{
  display:inline-block;
  padding: 0.25rem 0.6rem;
  border-radius: 0.75rem;
  font-size:0.85rem;
  font-weight:600;
  border: 1.5px solid;
  min-width: 5.5rem;
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
