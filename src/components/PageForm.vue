<template>
  <div class="customers-support bg-[#006B6E]">
    <div
      class="customers-support-container px-8 lg:px-0 w-full lg:w-3/4 mx-auto pt-[100px] pb-44"
    >
      <div class="content text-white">
        <h1 class="text-3xl font-bold">
          Customs Support - Take the load off your mind
        </h1>
        <hr class="w-14 h-[3px] bg-[#059CB6] border-none my-9" />
        <div class="wrapper-form flex flex-col gap-10 md:gap-0 md:flex-row">
          <div
            class="text-white w-full pr-0 md:w-[70%] md:border-r border-gray-400 md:pr-14"
          >
            <div class="get-in-touch mb-12">
              <h2 class="text-base font-bold">
                Get in touch with one of our customs experts!
              </h2>
              <p class="font-normal text-base pt-1">
                Fill in the contact form or use the chat function on the
                website.
              </p>
            </div>
            <div class="new-customer mb-7">
              <h2 class="text-[14px] md:text-base font-bold mb-5">
                Are you a new or returning customer? *
              </h2>
              <div class="radio flex">
                <div class="mr-6 flex">
                  <input
                    type="radio"
                    id="new"
                    value=""
                    name="inline-radio-group"
                    class="h-5 w-5"
                  />
                  <label for="new" class="ml-2">New</label>
                </div>
                <div class="flex">
                  <input
                    type="radio"
                    id="returninig"
                    value=""
                    name="inline-radio-group"
                    class="h-5 w-5"
                  />
                  <label for="returning" class="ml-2">Returning</label>
                </div>
              </div>
            </div>
            <div class="select">
              <select
                id="countries"
                class="bg-gray-50 h-[50px] border border-gray-300 text-gray-900 text-sm rounded focus:outline-none block w-full p-2.5"
              >
                <option selected="">Choice of service *</option>
                <option value="US">United States</option>
                <option value="CA">Canada</option>
                <option value="FR">France</option>
                <option value="DE">Germany</option>
              </select>
            </div>
            <hr class="my-8 border border-gray-400" />

            <form>
              <div class="grid gap-6 mb-6 md:grid-cols-2">
                <div>
                  <input
                    type="text"
                    id="first_name"
                    class="bg-gray-50 h-[50px] border border-gray-300 text-gray-900 text-sm rounded focus:outline-none block w-full p-2.5 placeholder-[#3D4D62]"
                    placeholder="First Name*"
                    required=""
                  />
                </div>
                <div>
                  <input
                    type="text"
                    id="last_name"
                    class="bg-gray-50 h-[50px] border border-gray-300 text-gray-900 text-sm rounded focus:outline-none block w-full p-2.5 placeholder-[#3D4D62]"
                    placeholder="Last Name*"
                    required=""
                  />
                </div>
                <div>
                  <input
                    type="text"
                    id="Company*"
                    class="bg-gray-50 h-[50px] border border-gray-300 text-gray-900 text-sm rounded focus:outline-none block w-full p-2.5 placeholder-[#3D4D62]"
                    placeholder="Company"
                    required=""
                  />
                </div>
                <div>
                  <input
                    type="email"
                    id="phone"
                    class="bg-gray-50 h-[50px] border border-gray-300 text-gray-900 text-sm rounded focus:outline-none block w-full p-2.5 placeholder-[#3D4D62]"
                    placeholder="E-Mail*"
                    required=""
                  />
                </div>
                <div>
                  <div class="flex relative">
                    <span
                      class="inline-flex items-center px-3 text-sm bg-white rounded border text-[#3D4D62] absolute inset-y-0 left-0 pl-2 border-r"
                    >
                      <img
                        src="../assets/Gruppe maskieren 8@2x.png"
                        alt="flag"
                        class="h-[20px]"
                      />
                      +44
                    </span>
                    <input
                      type="number"
                      id="website-admin"
                      class="rounded pl-[75px] bg-gray-50 h-[50px] border text-gray-900 focus:outline-none block flex-1 min-w-0 w-full text-sm border-gray-300 p-2.5 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
                      placeholder="Phone number *"
                    />
                  </div>
                </div>
                <div class="select">
                  <select
                    id="countries"
                    class="bg-gray-50 h-[50px] border border-gray-300 text-gray-900 text-sm rounded focus:outline-none block w-full p-2.5"
                  >
                    <option selected="">Country</option>
                    <option value="US">United States</option>
                    <option value="CA">Canada</option>
                    <option value="FR">France</option>
                    <option value="DE">Germany</option>
                  </select>
                </div>
              </div>
            </form>
            <div class="term radio flex justify-between flex-wrap my-8">
              <div class="flex mb-2 md:mb-0">
                <input
                  type="radio"
                  id="new"
                  value=""
                  name="inline-radio-group"
                  class="h-5 w-5 bg-transparent"
                />
                <label
                  for="terms"
                  class="ml-2 text-[14px] md:text-base font-normal"
                  >I agree with the
                  <a href="#" class="underline">Terms and Conditions</a> *
                </label>
              </div>
              <div class="flex">
                <input
                  type="radio"
                  id="returninig"
                  value=""
                  name="inline-radio-group"
                  class="h-5 w-5"
                />
                <label
                  for="newsletter"
                  class="ml-2 text-[14px] md:text-base font-normal"
                  >I want to sign up for the newsletter
                  <i class="far fa-envelope"></i
                ></label>
              </div>
            </div>
            <BaseButton class="w-[300px] h-[50px]">
              <template> Request a quote </template>
            </BaseButton>
          </div>
          <div class="contect-us flex items-center md:pl-14">
            <div class="w-full">
              <h2 class="text-base font-bold">
                You prefer a personal contact?
              </h2>
              <p class="font-normal text-base pt-1 mb-5">
                Please find the phone numbers of our locations below.
              </p>
              <div class="select">
                <select
                  id="support"
                  class="bg-gray-50 h-[50px] border border-gray-300 text-gray-900 text-sm rounded focus:outline-none block w-full p-2.5"
                >
                  <option selected="">Customers Support</option>
                  <option value="US">Admin</option>
                  <option value="CA">Developer</option>
                  <option value="FR">Manager</option>
                </select>
              </div>
              <BaseButton class="mt-5 w-full h-[50px]">
                <template> Go </template>
              </BaseButton>
              <hr class="my-8 border border-gray-400" />
              <div class="profile">
                <p
                  class="text-[25px] text-center md:text-start font-medium text-white"
                >
                  „Let’s grow together!“
                </p>
                <span
                  class="flex flex-col text-center items-center md:flex-row space-x-4 mt-5 md:text-start"
                >
                  <!-- Icon -->
                  <img
                    class="w-[81px] h-[81px] rounded-full mb-3 md:mb-0"
                    src="../assets/Gruppe 482@2x.png"
                    alt="profile picture"
                  />
                  <p class="flex flex-col justify-center">
                    <span class="text-baseleading-tight text-[white] font-bold"
                      >Integration help
                    </span>
                    Customer Support Lead CSG
                  </p>
                </span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import BaseButton from "./Base/BaseButton.vue";
export default {
  name: "PageForm",
  components: {
    BaseButton,
  },
};
</script>
<style lang="css" scoped></style>
