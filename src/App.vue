<template>
  <div class="m-20">
    <div class="card lg:card-side bg-base-300 shadow-xl">
      <figure class="w-24 m-10"><img :src="crownImage" alt="Album"/></figure>
      <div class="card-body">
        <h2 class="card-title">Страница курса JavaPro 23/24!</h2>
        <p>
          На этой странице Вы можете контролировать, какие домашние задания вы сделали, а какие - нет.
        </p>
        <p>
          У задач существует четыре статуса - задача сдана и принята, задача сдана на проверку и ее еще не проверили,
          задачу проверили и есть комментарии, которые надо исправить, и четвертый статус - задачи нет вообще.
        </p>
      </div>
    </div>
  </div>

  <div class="card bg-base-300 shadow-xl m-20">
    <div class="card-body">
      <div class="overflow-x-auto">
        <table class="table text-center">
          <!-- head -->
          <thead>
          <tr>
            <th></th>
            <th class="text-white">Гвоздева Ирина</th>
            <th class="text-white">Защелкин Егор</th>
            <th class="text-white">Казарников Сергей</th>
            <th class="text-white">Григорьев Алексей</th>
            <th class="text-white">Гатиятуллин Эдуард</th>
            <th class="text-white">Константин Ноэль</th>
            <th class="text-white">Александр Завадский</th>
          </tr>
          </thead>
          <tbody>

          <tr class="hover">
            <th>HW5</th>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><ChatBubbleOvalLeftEllipsisIcon class="h-6 w-6 mx-auto text-warning" /></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
          </tr>

          <tr class="hover">
            <th>HW4</th>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
            <td><ChatBubbleOvalLeftEllipsisIcon class="h-6 w-6 mx-auto text-warning" /></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
            <td><ChatBubbleOvalLeftEllipsisIcon class="h-6 w-6 mx-auto text-warning" /></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
          </tr>

          <tr class="hover">
            <th>HW3</th>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
            <td><ChatBubbleOvalLeftEllipsisIcon class="h-6 w-6 mx-auto text-warning" /></td>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
          </tr>

          <tr class="hover">
            <th>HW2</th>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
          </tr>

          <tr class="hover">
            <th>HW1</th>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><CheckCircleIcon class="h-6 w-6 mx-auto text-success"/></td>
            <td><XCircleIcon class="h-6 w-6 mx-auto text-error" /></td>
          </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>

<script>
import crownImage from "/src/static/crow.png"
import {CheckCircleIcon, XCircleIcon, ClockIcon, ChatBubbleOvalLeftEllipsisIcon} from "@heroicons/vue/24/outline";

export default {
  components: {
    CheckCircleIcon, XCircleIcon, ClockIcon, ChatBubbleOvalLeftEllipsisIcon
  },
  data() {
    return {
      crownImage: crownImage
    }
  }
}
</script>