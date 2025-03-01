---
type: worker
worker: sifter
layout: worker
---
{% capture content %}
The Sifter is a part of your colony's production line. The Sifter will sift through materials to find hidden ores, seeds, and other useful items and ingredients. When they do this, the materials they are sifting will disappear.

The default materials that can be sifted are:
<ul>
  <li>Dirt</li>
  <li>Sand</li>
  <li>Gravel</li>
  <li>Soul Sand</li>
</ul>

However, you can change this in the [config file](../../source/misc/configfile). This also works with modded items. Anything can be added here, it is up to the player (or the server owner).

The Sifter can only sift a certain amount of materials per day, depending on their hut level. The higher the Sifter's Strength level, the faster they'll sift.

| Hut Level | Daily Max |
| --------- | --------- |
| 1         | 64        |
| 2         | 256       |
| 3         | 576       |
| 4         | 1024      |
| 5         | Unlimited |

The Sifter can use 4 different meshes. The higher levels of meshes will find more items of better quality, as will a higher Focus level of the Sifter. Meshes are only made by other workers.

| Mesh    | Worker     |
| ------- | ---------- |
| String  | Fletcher   |
| Flint   | Stonemason |
| Iron    | Blacksmith |
| Diamond | Mechanic   |

**Note:** Meshes and blocks to be sifted must be added to the Minimum Stock tab in the Sifter's Hut in order for the Sifter to work.
{% endcapture %}
{% capture infobox %}
{% include infobox/worker.html %}
{% endcapture %}
{% include infobox/wrapper.html content=content infobox=infobox %}
