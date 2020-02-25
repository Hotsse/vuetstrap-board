<template>
  <div class="table-responsive">
    <table class="table table-striped table-bordered table-hover">
      <colgroup>
        <col width="5%">
        <col width="*">
        <col width="10%">
        <col width="10%">
        <col width="5%">
      </colgroup>
      <thead>
        <tr class="text-center">
          <th>No.</th>
          <th>제목</th>
          <th>작성자</th>
          <th>작성일시</th>
          <th>조회수</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="list in lists" :key="list">
          <td class="text-center">{{ list.no }}</td>
          <td>{{ list.title }}</td>
          <td class="text-center">{{ list.regNm }}</td>
          <td class="text-center">{{ list.regDt }}</td>
          <td class="text-center">{{ list.readCnt }}</td>
        </tr>
      </tbody>
    </table>
    <div>
      {{ count }}
      <button @click="++count">up</button>
      <button @click="--count">downf</button>
    </div>
  </div>
</template>

<script>
export default {
  scrollToTop: false,
  data: () => {
    return {
      lists: [
        { no: 1, title: '제목제목', regNm: '윤호세', regDt: '2020-02-25 12:00:00', readCnt: 1 },
        { no: 2, title: '제목제목2', regNm: '윤호세', regDt: '2020-02-25 12:00:00', readCnt: 1 },
        { no: 3, title: '제목제목3', regNm: '윤호세', regDt: '2020-02-25 12:00:00', readCnt: 1 },
        { no: 4, title: '제목제목4', regNm: '윤호세', regDt: '2020-02-25 12:00:00', readCnt: 1 },
        { no: 5, title: '제목제목5', regNm: '윤호세', regDt: '2020-02-25 12:00:00', readCnt: 1 },
        { no: 6, title: '제목제목6', regNm: '윤호세', regDt: '2020-02-25 12:00:00', readCnt: 1 },
        { no: 7, title: '제목제목7', regNm: '윤호세', regDt: '2020-02-25 12:00:00', readCnt: 1 }
      ],
      count: 0
    }
  }
}
</script>

<style>
</style>
