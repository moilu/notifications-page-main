<template>
    <div class="card">
        <img class="card__avatar" src="../assets/images/avatar-angela-gray.webp" alt="Avatar Picture">
        <div class="card__content">
            <div class="card__content--notification">
                <p class="notification__message"><b>User Name</b> reacted to your recent post<b> My first tournament today!</b></p>
                <div class="notification__status"></div>
            </div>
            <span class="card__content--time">1m ago</span>
        </div>
    </div>
</template>
<script>
export default {
    name: 'NotificationCard',
    data() {
        return {}
    }
}
</script>
<style>
.card {
    background-color: #f7fafd;
    display: grid;
    align-items: center;
    grid-template-columns: 90px 1fr;
}
.card__avatar {
    height: 70px;
    width: 70px;
}

.card__content {
    display: grid;
}

.card__content--notification {
    display: grid;
    grid-template-columns: 97% 3%;
    text-align: left;
}

.notification__status {
    background-color: red;
    border-radius: 50%;
    height: 10px;
    justify-self: end;
    width: 10px;
}
</style>