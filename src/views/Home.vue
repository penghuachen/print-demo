<template>
  <div class="home">
    <div class="no-print">
      <h1>網頁列印測試範例</h1>
      <el-button type="success" @click="print">點擊開啟列印模式</el-button>
      <p class="tip">以下為列印的範圍</p>
      <hr>
      <el-row :gutter="30">
        <h2>一些商品的介紹</h2>
        <el-col :span="8" v-for="o in 3" :key="o">
          <el-card
            :body-style="{ padding: '0px' }"
            >
            <img src="https://shadow.elemecdn.com/app/element/hamburger.9cf7b091-55e9-11e9-a976-7f4d0b07eef6.png" class="image">
            <div class="card-content" style="padding: 14px;">
              <span>好吃的漢堡</span>
              <div class="bottom clearfix">
                <time class="time">{{ currentDate }}</time>
              </div>
            </div>
          </el-card>
        </el-col>
      </el-row>
      <div class="table-container">
        <h2>一個簡單的列表</h2>
        <el-table
          :data="tableData"
          stripe
          style="width: 100%">
          <el-table-column
            prop="date"
            label="日期"
            >
          </el-table-column>
          <el-table-column
            prop="name"
            label="姓名"
            >
          </el-table-column>
          <el-table-column
            prop="age"
            label="年齡"
            >
          </el-table-column>
          <el-table-column
            prop="habbit"
            label="興趣"
            >
          </el-table-column>
          <el-table-column
            prop="address"
            label="地址">
          </el-table-column>
        </el-table>
      </div>
    </div>
    <div class="print">
      <el-row :gutter="30">
        <h2>一些商品的介紹</h2>
        <el-col :span="24" v-for="o in 3" :key="o">
          <el-card
            :body-style="{ padding: '0px' }"
            class="custom-card"
            >
            <img src="https://shadow.elemecdn.com/app/element/hamburger.9cf7b091-55e9-11e9-a976-7f4d0b07eef6.png" class="image">
            <div class="card-content" style="padding: 14px;">
              <span>好吃的漢堡</span>
              <div class="bottom clearfix">
                <time class="time">{{ currentDate }}</time>
              </div>
            </div>
          </el-card>
        </el-col>
      </el-row>
      <div class="table-container">
        <h2 class="title">一個簡單的列表</h2>
        <el-table
          :data="tableData"
          stripe
          style="width: 100%;">
          <el-table-column
            prop="date"
            label="日期"
            width="125px"
            >
          </el-table-column>
          <el-table-column
            prop="name"
            label="姓名"
            width="125px"
            >
          </el-table-column>
          <el-table-column
            prop="age"
            label="年齡"
            width="100px"
            >
          </el-table-column>
          <el-table-column
            prop="habbit"
            label="興趣"
            width="125px"
            >
          </el-table-column>
          <el-table-column
            prop="address"
            label="地址"
            width="175px"
            >
          </el-table-column>
        </el-table>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data() {
    return {
      currentDate: new Date(),
      tableData: [
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
        {
          date: '2016-05-02',
          name: '王小名',
          age: 17,
          habbit: '看漫畫',
          address: '火星市火星街火星路1號'
        },
      ]
    }
  },
  methods: {
    print() {
      this.isPrint = true;
      window.print();
    }
  },
}
</script>


<style lang="scss" scoped>
h1 {
  font-size: 48px;
}

.tip {
  color: #f00;
  font-weight: 600;
}

.print {
  display: none;
}

.card-content {
  background: #fafafa;
}

.table-container {
  margin-top: 60px;
}

@media print { 
  @page {
    margin: 0.5cm;
    size: A4 portrait;
  }

  .print {
    display: block;
  }

  .no-print {
    display: none;
  }

  .title {
    padding: 30px 0;
  }

  ::v-deep .el-col {
    margin-bottom: 20px;
  }

  .custom-card {
    ::v-deep .el-card__body {
      display: flex;
      height: 300px;
      img {
        width: 50%;
      }
      .card-content {
        text-align: left;
      }
    }
  }

  ::v-deep .el-table {
    .el-table__row {
      page-break-inside: avoid;
    }
  }
	.table-container,.card-content { 
		-webkit-print-color-adjust: exact; 
	} 
}
</style>


<!-- element ui style -->
<style>
.time {
  font-size: 13px;
  color: #999;
}

.bottom {
  margin-top: 13px;
  line-height: 12px;
}

.button {
  padding: 0;
  float: right;
}

.image {
  width: 100%;
  display: block;
}

.clearfix:before,
.clearfix:after {
    display: table;
    content: "";
}

.clearfix:after {
    clear: both
}

.el-table--striped .el-table__body tr.el-table__row--striped td {
  background: #67C23A !important;
}

.el-table .cell {
  font-weight: 600;
}
</style>