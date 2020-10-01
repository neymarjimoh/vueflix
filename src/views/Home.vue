<template>
  <v-container fluid>
    <Banner />
    <OriginalsRow />
    <Row title="Trending Videos" :fetchUrl="requests.fetchTrending" />
    <Row title="Top Rated" :fetchUrl="requests.fetchTopRated" />
    <Row title="Action Movies" :fetchUrl="requests.fetchActionMovies" />
    <Row title="Comedy Movies" :fetchUrl="requests.fetchComedyMovies" />
    <Row title="Horror Movies" :fetchUrl="requests.fetchHorrorMovies" />
    <Row title="Romance Movies" :fetchUrl="requests.fetchRomanceMovies" />
    <Row title="Documentaries" :fetchUrl="requests.fetchDocumentaries" />
  </v-container>
</template>

<script>
// @ is an alias to /src
import Row from "@/components/Row.vue";
import OriginalsRow from "@/components/OriginalsRow.vue";
import Banner from "@/components/Banner.vue";
import requests from "../requests";

export default {
  name: "Home",
  data() {
    return {
      requests
    }
  },
  components: {
    Row,
    OriginalsRow,
    Banner,
  },
};
</script>

<style scoped></style>
