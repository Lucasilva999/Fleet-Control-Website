<template>
    <v-footer dark>
        <div style="width: 100%" v-if="$vuetify.breakpoint.smAndUp" class="d-flex justify-space-between">
        <span class="caption">LLPG Soluções ®</span>
        <span class="caption">Áreas Metropolitanas: 9999-9999  |  Demais localidades: 0800-999-9999</span>
        <span class="caption">&copy; 2019</span>
        </div>
        <div style="width: 100%" v-else class="d-flex justify-center">
        <span class="caption">LLPG Soluções ®</span>
        </div>
    </v-footer>
</template>