<template>
  <q-page>
<<<<<<< HEAD
    <p>Page Todo</p>
    <q-list>
=======
    <q-list bordered separator>
>>>>>>> 77c23b5b239a30d971d737d7d92bdb15861fa51a
      <q-item
        v-for="task in tasks"
        :key="task.id"
        @click="task.completed = !task.completed"
        :class="task.completed ? 'bg-green-1' : 'bg-orange-1'"
        clickable
        v-ripple
      >
        <q-item-section side top>
          <q-checkbox v-model="task.completed" />
        </q-item-section>

        <q-item-section>
<<<<<<< HEAD
          <q-item-label :class="{ 'task-done': task.completed }">
            {{ task.name }}
=======
          <q-item-label
            :class="{ 'task-done' : task.completed}"
          >
            {{task.name}}
>>>>>>> 77c23b5b239a30d971d737d7d92bdb15861fa51a
          </q-item-label>
        </q-item-section>

        <q-item-section side>
          <div class="row">
            <div class="column justify-center">
<<<<<<< HEAD
              <q-icon name="event" size="18px" class="q-mr-xs" />
            </div>

            <div class="column">
              <q-item-label class="row justify-end" caption>
                {{ task.dueDate }}
              </q-item-label>
              <q-item-label class="row justify-end" caption>
                {{ task.dueTime }}
              </q-item-label>
=======
              <q-icon name="event" size="18px" class="q-mr-xs"/>
            </div>
            <div class="column">
                <q-item-label class="row justify-end" caption>
                  {{ task.dueDate }}
                </q-item-label>
                <q-item-label class="row justify-end" caption>
                  {{ task.dueTime }}
                </q-item-label>
>>>>>>> 77c23b5b239a30d971d737d7d92bdb15861fa51a
            </div>
          </div>
        </q-item-section>
      </q-item>
    </q-list>
  </q-page>
</template>

<!--
        -->
<script>
export default {
<<<<<<< HEAD
  name: "PageTodo",
=======
  name: 'PageTodo',
>>>>>>> 77c23b5b239a30d971d737d7d92bdb15861fa51a
  data() {
    return {
      tasks: [
        {
<<<<<<< HEAD
          id: "1",
          name: "tarefa 1",
          dueDate: null,
          dueTime: null,
          completed: false,
        },
        {
          id: "2",
          name: "tarefa 2",
          dueDate: null,
          dueTime: null,
          completed: false,
        },
        {
          id: "3",
          name: "tarefa 3",
          dueDate: null,
          dueTime: null,
          completed: false,
        },
      ],
    };
  },
};
=======
          id: '1',
          name: 'Ir ao shopping',
          dueDate: '22/05/2024',
          dueTime: '18:30',
          completed: false
        },
        {
          id: '2',
          name: 'Comprar bananas',
          dueDate: '22/05/2024',
          dueTime: '19:00',
          completed: false
        },
        {
          id: '3',
          name: 'Comprar maçã',
          dueDate: '22/05/2024',
          dueTime: '19:00',
          completed: false
        }
      ]
    }
  }
}
>>>>>>> 77c23b5b239a30d971d737d7d92bdb15861fa51a
</script>
<style scoped>
.task-done {
  text-decoration: line-through;
}
</style>
