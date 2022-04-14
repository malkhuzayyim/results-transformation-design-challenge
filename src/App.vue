<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <div>Data Transformation & UI Design Challenge</div>
      </div>
    </v-app-bar>

    <v-main>
      <v-container fluid>
        <v-row dense>
          <v-col cols="12">
            <v-card class="ma-6 mx-auto" tile outlined max-width="800px">
              <div class="title pa-4">Challenge Statement</div>
              <v-divider></v-divider>
              <div class="pa-4 body-2">
                Design a view that shows the corresponding accounts report in
                the provided "reportResults" array.
              </div>
              <div class="px-4 pb-4 body-2">
                As you can see when browsing the data, the array is comprised of
                an accounts heirarchy that was provided in a flattened format,
                with a "level" property that indicates the level of the node.
              </div>
              <div class="px-4 pb-4 body-2">
                Each account has a total of its own, when presenting the data,
                the presented total should also include the total of all the
                children (or subaccounts) of that account.
              </div>
              <div class="px-4 pb-4 caption">
                Challenge context: in accounting, accounts with type 1 are
                typically the assets, 2 are the liabilities, and 3 are the
                equity. Keep in mind, the "currentBalance" property of each of
                each account in the report results is in halala's, not SAR.
              </div>
              <div class="px-4 pb-4 caption">
                Hint: The primary concern of this challenge is how you manage
                transforming the data. Designing a tree representation of the
                array in the UI is not required, any UI design that clearly
                shows each accounts level and parent/children would suffice.
              </div>
            </v-card>
          </v-col>
          <v-col cols="12">
            <!--  -->
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import { reportResults } from "@/assets/reportResults.js";

export default {
  name: "App",

  components: {
    //
  },

  data: () => ({
    //
    reportResults,
  }),
};
</script>
