<template>
    <div>
        <div class="title">八皇后问题</div>
        <div class="gird" v-for="(row, r_index) in grids" :key="r_index">
            <div class="cell" v-for="cell in row" :key="cell.key">
                <div v-if="cell.ok">Q</div>
            </div>
        </div>
    </div>
</template>

<script>
const grids = new Array(8).fill(1).map((_, r) => {
    return new Array(8).fill(1).map((_, c) => {
        return {
            key: `key-${r * 8 + c}`,
            ok: false,
        }
    })
})
export default {
    data() {
        return {
            grids
        }
    },
    methods: {
        change() {
            console.log(2);
            console.log(1);
        }
    },
    // render() {
    //     return (
    //         <div class="grid">
    //             {this.grids.map((row, r_index) => (
    //                 <div class="row" key={r_index}>
    //                     {row.map(item => (
    //                         <div class="cell" key={item.key}>
    //                             {item.ok ? <div>Q</div> : ""}
    //                         </div>
    //                     ))}
    //                 </div>
    //             ))}
    //         </div>
    //     )
    // }
}
</script>