<template>
    <div class="auth-page">
      <div class="container mx-auto h-screen flex justify-center items-center">
        <div class="w-full lg:w-1/3 px-10 lg:px-0">
          <div class="flex justify-center items-center mx-auto mb-4 w-40">
            <div class="relative">
              <a href="/upload-filled">
                <img
                  src="/assets/images/avatar.jpg"
                  alt=""
                  class="rounded-full border-white border-4"
                />
                <img
                  src="/assets/images/icon-avatar-add.svg"
                  alt=""
                  class="absolute right-0 bottom-0 pb-2"
                />
              </a>
            </div>
          </div>
          <h2 class="font-normal mb-3 text-3xl text-white text-center">
            Hi, Aji
          </h2>
          <p class="text-white text-center font-light">
            Please upload your selfie
          </p>
          <div class="mb-4 mt-6">
            <div class="mb-3">
              <button
                @click="$router.push({ path: '/register-success' })"
                class="block w-full bg-orange-500 hover:bg-green-500 text-white font-semibold px-6 py-4 text-lg rounded-full"
              >
                Sign Up Now
              </button>
            </div>
          </div>
          <div>
            <div class="mb-4">
              <button
                @click="$router.push({ path: '/register-success' })"
                class="block w-full bg-transparent border-white border hover:bg-white hover:bg-opacity-25 text-white font-light px-6 py-4 text-lg rounded-full"
              >
                Skip
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>

</template>

<style lang="scss" scoped>
.auth-background {
  background-image: url('/assets/images/sign-in-background.jpg');
  background-position: center;
  background-size: cover;
}
</style>