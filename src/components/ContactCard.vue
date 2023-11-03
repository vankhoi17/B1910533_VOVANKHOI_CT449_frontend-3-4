<script>
export default {
props: {
contact: { type: Object, required: true },
},
};
</script>
<template>
<div>
<div class="p-1">
<strong>Tên: Võ Văn Khởi</strong>
{{ contact.name }}
</div>
<div class="p-1">
<strong>E-mail: khoib1910533@student.ctu.edu.vn</strong>
{{ contact.email }}
</div>
<div class="p-1">
<strong>Địa chỉ: Hoà An Phụng Hiệp Hậu Giang</strong>
{{ contact.address }}
</div>
<div class="p-1">
<strong>Điện thoại: 0773692160</strong>
{{ contact.phone }}
</div>
<div class="p-1">
<strong>Liên hệ yêu thích: 0706723670&nbsp;</strong>
<i v-if="contact.favorite" class="fas fa-check"></i>
<i v-else class="fas fa-times"></i>
</div>
</div>
</template>
