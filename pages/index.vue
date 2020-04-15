<template>
  <div class="container">
    <div class="inner_container">
      <div class="form">
        <h1 class="form_option">Discover</h1>
        <select name="Genre" id="genre">
          <option v-for="genre in genres">{{ genre }}</option>
        </select>
        <h1 class="form_option">From</h1>
        <select name="County" id="county">
          <option v-for="county in counties">{{ county }}</option>
        </select>
      </div>
      <div class="playlist">
        <iframe
          src="https://open.spotify.com/embed/playlist/2jRcgzF55Zfcj7UDZMi7cm"
          width="300"
          height="300"
          frameborder="0"
          allowtransparency="true"
          allow="encrypted-media"
        ></iframe>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      genres: [
        'All Music',
        'Electronic/Dance Music',
        'Folk/Acoustic Music',
        'Pop Music',
        'Rap/Hiphop Music',
        'Rock/Metal Music',
        'Trad Music'
      ],
      counties: [
        'Ireland',
        'Antrim',
        'Armagh',
        'Carlow',
        'Cavan',
        'Clare',
        'Cork',
        'Derry',
        'Donegal',
        'Down',
        'Dublin',
        'Fermanagh',
        'Galway',
        'Kerry',
        'Kildare',
        'Kilkenny',
        'Laois',
        'Leitrim',
        'Limerick',
        'Longford',
        'Louth',
        'Mayo',
        'Meath',
        'Monaghan',
        'Offaly',
        'Roscommon',
        'Sligo',
        'Tipperary',
        'Tyrone',
        'Waterford',
        'Westmeath',
        'Wexford',
        'Wicklow'
      ]
    }
  }
}
</script>

<style>
html {
  background-color: #39b982;
}

.container {
  width: 100%;
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.inner_container {
  margin: 0 auto;
}

.form {
  margin-bottom: 30px;
}

.form_option {
  margin: 10px;
}

.playlist {
  margin-top: 30px;
}

select {
  width: 95%;
  height: 52px;
  padding: 0 24px 0 10px;
  vertical-align: middle;
  background: #39b982
    url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 4 5'%3E%3Cpath fill='%23343a40' d='M2 0L0 2h4zm0 5L0 3h4z'/%3E%3C/svg%3E")
    no-repeat right 12px center;
  background-size: 8px 10px;
  border: solid 0px rgba(128, 74, 74, 0.4);
  border-radius: 10px;
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  font-size: 1.4em;
  text-decoration: underline;
  text-align-last: center;
}

select:focus {
  border-color: #39b982;
  outline: 0;
}

select:focus::ms-value {
  color: #000;
  background: #fff;
}

select::ms-expand {
  opacity: 0;
}
</style>
