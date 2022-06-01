<template>
  <div class="wrapper">
    <p-header />
    <div class="layout">
      <div>
        <p-site-menu />
      </div>

      <div v-if="this.$route.params.book === 'about'">
        <h1>About Dan Trotter</h1>
        <p>An ex-lawyer, I have been a college professor of Business Administration in the USA and in China. My ministry interests are home church (in the USA and in China), personal evangelism and discipleship in China, and teaching. For fourteen years I helped sponsor the annual Southern House Church Conference.  I hold degrees from the University of South Carolina (BA History, BA Economics, JD-MBA, PhD in Business Administration) and a MA in Church History (Trinity Evangelical Divinity School.) I have been married to my wife Linda since November 26, 1975, and have three children and six grandchildren. My interests outside of studying the Bible are history, baseball, basketball, and politics.</p>
      </div>

      <div v-else-if="this.$route.params.book === 'doctrinal-statement'">
        <h1>Doctrinal Statement</h1>
        <ol class="doctrinal-statement">
          <li>
            <h2>God</h2> 
            <p>We believe in one God, Creator of all things, holy, infinitely perfect, and eternally existing in a loving unity of three equally divine Persons: the Father, the Son and the Holy Spirit. Having limitless knowledge and sovereign power, God has graciously purposed from eternity to redeem a people for Himself and to make all things new for His own glory.</p>
          </li>
          <li>
            <h2>The Bible</h2> 
            <p>We believe that God has spoken in the Scriptures, both Old and New Testaments, through the words of human authors. As the verbally inspired Word of God, the Bible is without error in the original writings, the complete revelation of His will for salvation, and the ultimate authority by which every realm of human knowledge and endeavor should be judged. Therefore, it is to be believed in all that it teaches, obeyed in all that it requires, and trusted in all that it promises.</p>
          </li>
          <li>
            <h2>The Human Condition</h2> 
            <p>We believe that God created Adam and Eve in His image, but they sinned when tempted by Satan. In union with Adam, human beings are sinners by nature and by choice, alienated from God, and under His wrath. Only through God’s saving work in Jesus Christ can we be rescued, reconciled and renewed.</p>
          </li>
          <li>
            <h2>Jesus Christ</h2> 
            <p>We believe that Jesus Christ is God incarnate, fully God and fully man, one Person in two natures. Jesus—Israel's promised Messiah—was conceived through the Holy Spirit and born of the virgin Mary. He lived a sinless life, was crucified under Pontius Pilate, arose bodily from the dead, ascended into heaven and sits at the right hand of God the Father as our High Priest and Advocate.</p>
          </li>
          <li>
            <h2>The Work of Christ</h2> 
            <p>We believe that Jesus Christ, as our representative and substitute, shed His blood on the cross as the perfect, all-sufficient sacrifice for our sins. His atoning death and victorious resurrection constitute the only ground for salvation.</p>
          </li>
          <li>
            <h2>The Holy Spirit</h2> 
            <p>We believe that the Holy Spirit, in all that He does, glorifies the Lord Jesus Christ. He convicts the world of its guilt. He regenerates sinners, and in Him they are baptized into union with Christ and adopted as heirs in the family of God. He also indwells, illuminates, guides, equips and empowers believers for Christ-like living and service.</p>
          </li>
          <li>
            <h2>The Church</h2> 
            <p>We believe that the true church comprises all who have been justified by God’s grace through faith alone in Christ alone. They are united by the Holy Spirit in the body of Christ, of which He is the Head. The true church is manifest in local churches, whose membership should be composed only of believers. The Lord Jesus mandated two ordinances, baptism and the Lord’s Supper, which visibly and tangibly express the gospel. Though they are not the means of salvation, when celebrated by the church in genuine faith, these ordinances confirm and nourish the believer.</p>
          </li>
          <li>
            <h2>Christian Living</h2> 
            <p>We believe that God’s justifying grace must not be separated from His sanctifying power and purpose. God commands us to love Him supremely and others sacrificially, and to live out our faith with care for one another, compassion toward the poor and justice for the oppressed. With God’s Word, the Spirit’s power, and fervent prayer in Christ’s name, we are to combat the spiritual forces of evil. In obedience to Christ’s commission, we are to make disciples among all people, always bearing witness to the gospel in word and deed.</p>
          </li>
          <li>
            <h2>Christ’s Return</h2> 
            <p>We believe in the personal, bodily and glorious return of our Lord Jesus Christ. The coming of Christ, at a time known only to God, demands constant expectancy and, as our blessed hope, motivates the believer to godly living, sacrificial service and energetic mission.</p>
          </li>
          <li>
            <h2>Response and Eternal Destiny</h2> 
            <p>We believe that God commands everyone everywhere to believe the gospel by turning to Him in repentance and receiving the Lord Jesus Christ. We believe that God will raise the dead bodily and judge the world, assigning the unbeliever to condemnation and eternal conscious punishment and the believer to eternal blessedness and joy with the Lord in the new heaven and the new earth, to the praise of His glorious grace. Amen.</p>
          </li>
        </ol>
       
      </div>

      <div v-else-if="this.$route.params.book === 'doctrinal-distinctives'">
        <h1>Doctrinal Distinctives</h1>
        <p>I affirm the following:</p>
        <ul>
          <li>The traditional Augustinian doctrines of grace</li>
          <li>Complementarianism</li>
          <li>Apostolic, NT pattern home church ecclesiology</li>
          <li>ORTHODOX preterist eschatology</li>
          <li>Classical, non-theonomist, non-political post-mil eschatology</li>
          <li>New Covenant Theology</li>
          <li>Inerrancy of the original autographs</li>
        </ul>
        <p>I am irritated by the following:</p>
        <ul>
          <li>Cessationism</li>
          <li>Hyper-faith Copelandhaginism</li>
          <li>The JEDP Documentary Hypothesis</li>
        </ul>
      </div>

      <div v-else-if="this.$route.params.book === 'sources'">
        <h1>Sources Used</h1>
        <p>I have taken extensive notes on every verse of the Bible. I have chiefly relied on these commentators: John Gill, Adam Clark, Jamieson Fausset and Brown, Alfred Barnes, Joseph Benson, The Cambridge Bible for Schools and Colleges, Charles John Ellicott, Keil and Delitzsch, Matthew Poole, The Pulpit Commentary, as well as study notes in an NIV study Bible. Sometimes I would email friends with advance degrees in biblical studies and languages</p>
      </div>

      <div v-else-if="this.$route.params.book === 'target-audience'">
        <h1>Target Audience</h1>
        <p>I am seeking to reach serious students of the Bible who are orthodox Christians. I am aiming at a level somewhere between Adult Sunday School and seminary.</p>
      </div>

      <div v-else-if="this.$route.params.book === 'modus-operandi'">
        <h1>Modus Operandi</h1>
        <p>I try to present all issues presented by a particular passage. I examine textual variants, translation issues, theological issues, geography, chronology, biography, historical background, optional interpretations. I try to put myself into the shoes of all the characters and ask, “Why is this person doing what he is doing?” Often I make application points targeting 21 st century Christians. The The discussion is relatively deep, but I don’t go full bore into many theological issues, because I neither have the time nor the competence to do so.</p>
      </div>

      <div v-else-if="this.$route.params.book === 'controversial-passages'">
        <h1>Controversial Passages</h1>
        <p>I try to present controversial issues objectively, but after I do so, I will give my opinion forthrightly, if I have one. My negative opinions of cessationism, charismania, Copelandhaginism, feminism, dispensationalism, covenant theology, futurist eschatology, and Protestant liberalism may delight some, but will certainly offend others. However, these negative remarks are merely made in passing. My focus is to understand and explain simply what the passage means. In doing so, I present many optional interpretations, some of which are really outside the realm of probability, but which are included for the sake of presenting the listener with all reasonable interpretations.</p>
      </div>

      <div v-else>
        <p-book :name="this.$route.params.book" />
        <a href="https://dantrotter.podbean.com"><img src="~/static/AvailableOnPodbean.png" /></a>
      </div>

      <div>
        <p-social-share :title="title" :url="url" />
        <h2 class="small-header">Comments? Corrections?</h2>
        <a href="mailto:prettygoodbiblestudies@gmail.com">prettygoodbiblestudies@gmail.com</a>
      </div>
    </div>
  </div>
</template>

<script>
import PHeader from '/components/Header.vue';
import PBook from '/components/Book.vue';
import PSiteMenu from '/components/SiteMenu.vue';
import PSocialShare from '/components/SocialShare.vue';

export default {
  name: 'Book',
  components: { PHeader, PBook, PSiteMenu, PSocialShare },
  head() {
    return {
      title: this.title
    };
  },
  data() {
    return {
      title: "PGBS - " + this.$route.params.book.replace(/-/g, ' ').replace(/(^\w|\s\w)/g, w => w.toUpperCase()),
      url: 'url.com/' + this.$route.params.book
    }
  }
}
</script>