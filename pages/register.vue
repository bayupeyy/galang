<template>
    <div class="auth-page">
      <div class="h-screen flex justify-center items-center">
        <div
          class="hidden md:block lg:w-1/3 bg-white h-full auth-background rounded-tr-lg rounded-br-lg"
        ></div>
        <div class="w-auto md:w-2/4 lg:w-2/3 flex justify-center items-center">
          <div class="w-full lg:w-1/2 px-10 lg:px-0">
            <h2 class="font-normal mb-6 text-3xl text-white">
              Sign Up Account
            </h2>
            <div class="mb-6">
              <div class="mb-4">
                <label class="font-normal text-lg text-white block mb-3"
                  >Full Name</label
                >
                <input
                    type="text"
                    class="auth-form focus:outline-none focus:bg-purple-hover focus:shadow-outline focus:border-purple-hover-stroke focus:text-black-10"
                    placeholder="Julia Keeva Hanna"
                    onfocus="this.placeholder = ''"
                    onblur="if (this.value == '') {this.placeholder = 'Julia Keeva Hanna';}"
                />

              </div>
            </div>
            <div class="mb-6">
              <div class="mb-4">
                <label class="font-normal text-lg text-white block mb-3"
                  >Occupation</label
                >
                <input
                  type="text"
                  class="auth-form focus:outline-none focus:bg-purple-hover focus:shadow-outline focus:border-purple-hover-stroke focus:text-black-10"
                  placeholder="Write your occupation here"
                  onblur="if (this.value == '') {this.placeholder = 'Graphic Designer';}"
                />
              </div>
            </div>
            <div class="mb-6">
              <div class="mb-4">
                <label class="font-normal text-lg text-white block mb-3"
                  >Email Address</label
                >
                <input
                  type="email"
                  class="auth-form focus:outline-none focus:bg-purple-hover focus:shadow-outline focus:border-purple-hover-stroke focus:text-gray-100"
                  placeholder="Write your email address here"
                  onblur="if(this.value == ''){this.placeholder = 'julia.keeva@gmail.com';}"
                />
              </div>
            </div>
            <div class="mb-6">
              <div class="mb-4">
                <label class="font-normal text-lg text-white block mb-3"
                  >Password</label
                >
                <input
                    type="password"
                    class="auth-form focus:outline-none focus:bg-purple-hover focus:shadow-outline focus:border-purple-hover-stroke focus:text-black-10"
                    placeholder="Password"
                    onfocus="this.placeholder = ''"
                    onblur="if (this.value == '') {this.placeholder = 'Password';}"
                />

              </div>
            </div>
            <div class="mb-6">
              <div class="mb-4">
                <button
                  @click="$router.push({ path: '/upload' })"
                  class="block w-full bg-orange-500 hover:bg-green-500 text-white font-semibold px-6 py-4 text-lg rounded-full"
                >
                  Continue Sign Up
                </button>
              </div>
            </div>
            <div class="text-center">
              <p class="text-white text-md">
                Already have account?
                <nuxt-link to ="/login" class="no-underline text-orange-500"
                  >Sign In</nuxt-link>.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>

</template>

<style lang="scss" scoped>
.auth-background {
  background-image: url('/assets/images/sign-up-background.jpg');
  background-position: center;
  background-size: cover;
}
</style>