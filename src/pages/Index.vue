<template>
  <q-page class="bg-blue">
    <!-- Pictures row -->
    <div class="row q-pa-xl q-col-gutter-lg bg-yellow">
      <div class="col-12 col-lg-6" v-for="address of picturesAddress">
        <q-card class="shadow-6 bg-white q-pa-sm">
          <q-item>
            <q-item-section>
              <q-item-label>{{ address.description }}</q-item-label>
              <q-item-label caption>{{ address.rating }}</q-item-label>
            </q-item-section>
          </q-item>
          <div class="row q-col-gutter-sm">
            <img class="col-6" v-for="pic of address.photo" :src="pic" />
          </div>
        </q-card>
      </div>
    </div>
    <!-- End of pictures row  -->
  </q-page>
</template>

<script>
export default {
  name: "PageIndex",
  data() {
    return {
      picturesAddress: [
        {
          photo: [
            "https://fi.realself.com/org498/340/3bbac558a7a2505008bcba8d3caebf0a/c/9/a/Breast-Reduction-before-2762601-2642364.JPG",

            "https://fi.realself.com/org498/340/3bbac558a7a2505008bcba8d3caebf0a/7/e/4/Breast-Reduction-after-2762601-2642365.JPG"
          ],

          description:
            "35-44 woman treated with breast reduction. No implants.",
          rating: "10/10"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/bda7e6e6dcb2dcaff10597ef1cc7fc73/6/3/6/Breast-Lift-with-Implants-before-1606704-2173206.JPG",
            "https://fi.realself.com/org498/340/bda7e6e6dcb2dcaff10597ef1cc7fc73/2/a/4/Breast-Lift-with-Implants-after-1606704-2173207.JPG",
            "https://fi.realself.com/org498/340/bda7e6e6dcb2dcaff10597ef1cc7fc73/e/b/d/1606704-2173210.JPG",
            "https://fi.realself.com/org498/340/bda7e6e6dcb2dcaff10597ef1cc7fc73/d/6/b/1606704-2173211.JPG"
          ],
          description:
            "35-44 yr old woman treated with breast lift and implants. Bilateral mastopexy with moderate plus profile silicon implants 400cc bilaterally.Beautiful shape and fullness. Size is not too big.",
          rating: "10/10"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/1901aaa0ef0ea1167262071bb01fbabe/e/e/9/Mommy-Makeover-before-2267542-2472996.png",
            "https://fi.realself.com/org498/340/1901aaa0ef0ea1167262071bb01fbabe/e/8/9/Mommy-Makeover-after-2267542-2472997.png"
          ],
          description:
            "32 year old lift with augmentation. 375cc moderate plus profile silicone implants.",
          rating: "8/10"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/ad59dea89d40bbe637eee34ceb169919/0/4/d/Mommy-Makeover-before-703086-914631.JPG",
            "https://fi.realself.com/org498/340/ad59dea89d40bbe637eee34ceb169919/c/c/6/Mommy-Makeover-after-703086-914632.JPG"
          ],
          description: "34 year old breast lift. No implants.",
          rating: "7/10"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/4afd2a77d52187f2922ac5a4d4fcc839/9/3/6/Mommy-Makeover-before-9144855-4180430.png",
            "https://fi.realself.com/org498/340/eb15699e80aaae39da1a8100f24ec5ae/9/5/6/Mommy-Makeover-after-9144855-4180431.png"
          ],
          description: "35-44 year old breast lift. No implants",
          rating: "8/10"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/1b7e9cea6a8097dce1d5ce3d480a140b/a/e/a/Mommy-Makeover-before-1203627-1949215.jpg",
            "https://fi.realself.com/org498/340/1b7e9cea6a8097dce1d5ce3d480a140b/d/2/6/Mommy-Makeover-after-1203627-1949216.jpg"
          ],
          description:
            "30 year old silicone implants under muscle. Slightly bigger than I'd like. Very nice shape.",
          rating: "7/10"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/631b8816aa71ef8b82075d61743efbd3/e/d/7/Breast-Lift-with-Implants-before-2502405-2559360.jpg",
            "https://fi.realself.com/org498/340/631b8816aa71ef8b82075d61743efbd3/7/5/5/Breast-Lift-with-Implants-after-2502405-2559362.JPG"
          ],
          description:
            "35-44 year old breast lift with silicone implants. Nice, natural look. Similar breast shape and before tummy.",
          rating: "7/10"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/8e30a659c31b53017073692309ab0da1/c/7/5/Breast-Reduction-before-260534.jpg",
            "https://fi.realself.com/org498/340/8e30a659c31b53017073692309ab0da1/6/d/8/Breast-Reduction-after-260534.jpg"
          ],
          description:
            "Breast reduction, no implants. Nice size, good shape for non implant.",
          rating: "8/10"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/516ac44bdf7bb0506efc9c49414d530a/2/2/c/Breast-Lift-before-267726.jpg",
            "https://fi.realself.com/org498/340/516ac44bdf7bb0506efc9c49414d530a/1/b/4/Breast-Lift-after-267726.jpg"
          ],
          description:
            "Breast lift with implant. Dual-plane, subpectoral augmentation.",
          rating: "8/10"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/4d87020804ff23ac50e1b2be5037ed13/1/c/3/Breast-Lift-with-Implants-before-2611022-3751341.png",
            "https://fi.realself.com/org498/340/4d87020804ff23ac50e1b2be5037ed13/2/f/d/Breast-Lift-with-Implants-after-2611022-3751342.png"
          ],
          description:
            "35-44 year old Mastopexy with 492cc silicone implants, sub-muscular.",
          rating: "7/10"
        },
        {
          photo: [
            "https://fi.realself.com/340/cba20b74e2f55b9884afddfa0cb0f1dc/a/4/0/Mommy-Makeover-before-6900952-3502048.png",
            "https://fi.realself.com/org498/340/9ee6564d9645d9daaa2fedee03dc95a1/a/2/0/Mommy-Makeover-after-6900952-3502049.png"
          ],
          description:
            "I wanted to discuss the areola in this picture.  They seem to be set inside the breast somehow.",
          rating: "n/a"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/8e30a659c31b53017073692309ab0da1/7/b/9/Mommy-makeover-before-578646-627474.JPG",
            "https://fi.realself.com/org498/340/8e30a659c31b53017073692309ab0da1/9/b/b/Mommy-makeover-after-578646-627475.JPG",
            "https://fi.realself.com/org498/340/8e30a659c31b53017073692309ab0da1/c/7/4/578646-627476.JPG",
            "https://fi.realself.com/org498/340/8e30a659c31b53017073692309ab0da1/f/a/2/578646-627477.JPG"
          ],
          description:
            "I wanted to point out the very high scar placement in this surgery. My preference would be for a lower placement over removing more skin.",
          rating: "n/a"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/8e30a659c31b53017073692309ab0da1/2/b/8/Mommy-Makeover-before-257840.jpg",
            "https://fi.realself.com/org498/340/8e30a659c31b53017073692309ab0da1/a/0/f/Mommy-Makeover-after-257840.jpg"
          ],
          description:
            "I don't care for the contouring that this patient has had on her stomach. It doesn't have a natural look, it seems quite narrow and odd.",
          rating: "n/a"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/b2a1ce270fe460702fdcf7b6ad0ca2a4/3/d/b/5285772-4022257.jpg",
            "https://fi.realself.com/org498/340/97e9fc92146a638873e9ebe0ba76de8e/0/0/d/5285772-4022256.jpg"
          ],
          description:
            "It's kind of hard to tell what this patient's shape is from the photo, but I wanted to discuss the body shape of a very narrow waist and very large bum.  I'm not going for that Kardashian look.",
          rating: "n/a"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/5feb465af6608575c98d150ee92c734d/9/6/a/Tummy-Tuck-before-1294081-2000976.jpg",
            "https://fi.realself.com/org498/340/5feb465af6608575c98d150ee92c734d/c/5/3/Tummy-Tuck-after-1294081-2000977.jpg",
            "https://fi.realself.com/org498/340/5feb465af6608575c98d150ee92c734d/c/4/b/1294081-2000978.jpg",
            "https://fi.realself.com/org498/340/5feb465af6608575c98d150ee92c734d/f/9/d/1294081-2000979.jpg"
          ],
          description:
            "This reduction without implants has a square sort of shape.",
          rating: "n/a"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/dd1079cf0399156d989684a9ed4f1798/7/f/5/Mommy-Makeover-after-1084949-1885227.jpg",
            "https://fi.realself.com/org498/340/dd1079cf0399156d989684a9ed4f1798/7/9/5/Mommy-Makeover-before-1084949-1885226.jpg",
            "https://fi.realself.com/org498/340/dd1079cf0399156d989684a9ed4f1798/6/b/8/1084949-1885228.jpg",
            "https://fi.realself.com/org498/340/dd1079cf0399156d989684a9ed4f1798/5/6/e/1084949-1885229.jpg"
          ],
          description:
            "I wanted to bring this picture so we could discuss belly button placement more and the vertical incision ",
          rating: "n/a"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/763161bd217632d8a60ab3f5968baa2d/e/6/f/Breast-Reduction-before-994007-1815322.jpg",
            "https://fi.realself.com/org498/340/763161bd217632d8a60ab3f5968baa2d/3/2/0/Breast-Reduction-after-994007-1815323.jpg",
            "https://fi.realself.com/org498/340/763161bd217632d8a60ab3f5968baa2d/1/1/0/994007-1815324.jpg",
            "https://fi.realself.com/org498/340/763161bd217632d8a60ab3f5968baa2d/2/c/6/994007-1815325.jpg"
          ],
          description: "Square shaped reduction.",
          rating: "n/a"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/81ce795c867fb4966fdcdb5a13e9cae5/a/f/2/Mommy-Makeover-before-3489964-2795370.jpg",
            "https://fi.realself.com/org498/340/81ce795c867fb4966fdcdb5a13e9cae5/a/9/2/Mommy-Makeover-after-3489964-2795371.jpg"
          ],
          description: "Did not like these results, odd shape.",
          rating: "n/a"
        },
        {
          photo: [
            "https://fi.realself.com/org498/340/5b0fd4be378db3598ccb3f5a567a6519/3/0/5/Mommy-Makeover-before-9495624-4345242.png",
            "https://fi.realself.com/org498/340/9b70ff491861074bb9a82af3192c6ea8/8/4/7/Mommy-Makeover-after-9495624-4345244.png"
          ],
          description:
            "Interested to hear what your thoughts are on this tummy tuck. Is it still just swollen from surgery? Looks very full around the incision site.",
          rating: "n/a"
        }
      ]
    };
  }
};
</script>
