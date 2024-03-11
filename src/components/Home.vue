<script>
export default {
  data() {
    return {
      textToType: ["การใช้ SSH (Secure Shell)","จัดการ BIGDATA","เรียนรู้ IoT (Internet of Things)","ลองทำ AI (Artificial Intelligence)"],
      typedText: "",
      typingSpeed: 100, // Adjust the typing speed (in milliseconds)
    };
  },
  methods: {
    async typeText() {
      while (true) {
        for(let j =0;j<this.textToType.length;j++){
                for (let i = 0; i < this.textToType[j].length; i++) {
                      this.typedText = this.textToType[j].substring(0, i + 1);
                      await this.sleep(this.typingSpeed);
                    }
                    await this.sleep(2000); // Wait for 1 second before clearing the text
                    // this.typedText = " ";
                    await this.sleep(250); // Wait for 0.5 seconds before starting the typing again
        }
      }
    },
    sleep(ms) {
      return new Promise(resolve => setTimeout(resolve, ms));
    },
  },
  mounted() {
    this.typeText();
  },
};
</script>

<template>
  <div class="header">
    <h1 style="margin: 0;font-size: 5vmax;">Uphasia Hack 2024</h1>
    <h3 style="margin: 0;font-size: 2vmax;">ค่ายที่มาพร้อม Hackathon ชิงเงินรางวัลท้ายค่ายรวม 10,000 บาท</h3>
    <h2 style="margin: 0;font-size: 2vmax; color:  #17AA7C;">ในหัวข้อ Cloud for Human wellbeing</h2>
  </div>

  <p id="typedText">
    {{ typedText }}
    <span class="input-cursor">|</span>
  </p>
  <img id="uphasiainfo" src="../assets/uphasiahackinfo.png" alt="uphasiainfo">
</template>
<style scoped>
.read-the-docs {
  color: #888;
}
#typedText {
  font-size: 3vmax;
  
  position: relative; /* Add this line for correct positioning of the cursor */
}
.input-cursor {
  display: inline-block;
  width: 2px;
  height: 42px;
  background-color: white;
  /* margin-left: 8px; */
  position: absolute; /* Use absolute positioning */
}
#uphasiainfo{
  min-width: 350px;
  width: 60%;
  border-radius: 10px;
  box-shadow: 0px 5px 30px rgba(0, 0, 0, 0.177);
  margin: 50px 0;
}
@keyframes blink {
  0% { opacity: 1; }
  40% { opacity: 1; }
  60% { opacity: 0; }
  100% { opacity: 0; }
}
.input-cursor {
  animation: blink 0.6s linear infinite alternate;
}
</style>
