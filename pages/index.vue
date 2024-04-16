<template>
    <div class="mb-8">
        <NavBar />
    </div>

    <v-container>
        <div class="card">
            <div class="card-header">
                <h4>Student List
                    <NuxtLink to="/students/create" class="btn btn-primary float-end">Add Student</NuxtLink>
                </h4>
            </div>
            <div class="card-body">
                
            </div>
        </div>
    </v-container>
</template>

<script setup>
// definePageMeta({
//     middleware: ["auth-check"]
// })
</script>

<style lang="scss" scoped></style>