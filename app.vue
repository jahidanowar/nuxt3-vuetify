<template>
  <div>
    <v-card max-width="448" class="mx-auto" color="grey-lighten-3">
      <v-layout>
        <v-app-bar
          color="teal-darken-4"
          image="https://picsum.photos/1920/1080?random"
        >
          <v-app-bar-title>Title</v-app-bar-title>

          <v-spacer></v-spacer>

          <v-btn icon>
            <v-icon>mdi-magnify</v-icon>
          </v-btn>

          <v-btn icon>
            <v-icon>mdi-heart</v-icon>
          </v-btn>

          <v-btn icon>
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </v-app-bar>

        <v-main>
          <v-container fluid>
            <v-row dense>
              <v-col v-for="n in 4" :key="n" cols="12">
                <v-card
                  :title="`Content ${n}`"
                  :subtitle="`Subtitle for Content ${n}`"
                  text="Lorem ipsum dolor sit amet consectetur, adipisicing elit.?"
                ></v-card>
              </v-col>
            </v-row>
          </v-container>
        </v-main>
      </v-layout>
    </v-card>
  </div>
</template>
