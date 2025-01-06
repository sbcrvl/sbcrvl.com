---
breadcrumbs: ["photos"]
---

<script setup>
const gallery = [
    "./gallery/20241231-01.jpeg",
    "./gallery/20250101-01.jpeg",
    "./gallery/20250101-02.jpeg",
]
</script>

# Photos

## What is this?

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

<div>
    <span v-for="image in gallery.reverse()">
        <img v-bind:src="image" alt="image"/>
    </span>
</div>
