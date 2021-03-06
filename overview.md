---
layout: home
permalink: /overview/
---

<!-- Main Container -->
<div class="container p-3 my-5 border" style="background-color: #f3f4fc;">
    <h5 class="mb-3">Overview</h5>
    <hr class="my-4">
    <p>Here you will find an overview of Seldonian algorithms, the Seldonian framework, and this software library. If you are new to these topics, we recommend reading from the top down, but you are welcome to jump ahead using the links below. The content below is organized into the following topics:</p>
    <ol>
        <li>
            <a href="#need">The need for safe and fair machine learning</a>
        </li>
        <li>
            <a href="#probabilistic">The necessity of <i>probabilistic</i> guarantees</a>
        </li>
        <li>
            <a href="#algorithm">What is a Seldonian algorithm?</a>
        </li>
        <li>
            <a href="#framework">What is the Seldonian framework?</a>
        </li>
        <li>
            <a href="#library">What is this software library?</a>
        </li>
    </ol>
</div>

<div class="container p-3 my-5 border" style="background-color: #f3f4fc;">
        <h5 class="mb-3" id="need"><b>The need for safe and fair machine learning</b></h5>
        <hr class="my-4">
        <p>
            Intelligent machines are everywhere, ranging from simple data analysis and pattern recognition tools used across the sciences, to complex systems that achieve super-human performance on various tasks. Ensuring that these machines are well-behaved&mdash;that they do not, for example, harm humans or act in a racist or sexist way&mdash;is therefore not a hypothetical problem to be dealt with in the future, but a practical one that must be addressed today.
        </p>
        <p>
            Already, intelligent systems have caused harm. They have exhibited racist, sexist, and otherwise unfair behaviors that could reinforce existing social inequalities [<a href="https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing">1</a>, <a href="https://www.ted.com/talks/joy_buolamwini_how_i_m_fighting_bias_in_algorithms">2</a>, <a href="https://www.reuters.com/article/us-amazon-com-jobs-automation-insight/amazon-scraps-secret-ai-recruiting-tool-that-showed-bias-against-women-idUSKCN1MK08G">3</a>, <a href="https://www.scientificamerican.com/article/racial-bias-found-in-a-major-health-care-risk-algorithm/">4</a>, <a href="https://www.technologyreview.com/2019/04/05/1175/facebook-algorithm-discriminates-ai-bias/">5</a>, <a href="https://qz.com/1141122/google-translates-gender-bias-pairs-he-with-hardworking-and-she-with-lazy-and-other-examples/">6</a>, <a href="https://www.bloomberg.com/graphics/2016-amazon-same-day/">7</a>], and have produced dangerous behaviors [<a href="https://www.statnews.com/wp-content/uploads/2018/09/IBMs-Watson-recommended-unsafe-and-incorrect-cancer-treatments-STAT.pdf">1</a>], including behaviors that have caused harm and death [<a href="https://en.wikipedia.org/wiki/Death_of_Elaine_Herzberg">1</a>, <a href="https://www.osha.gov/pls/imis/accidentsearch.search?sic=&sicgroup=&naics=&acc_description=&acc_abstract=&acc_keyword=%22Robot%22&inspnr=&fatal=&officetype=&office=&startmonth=&startday=&startyear=&endmonth=&endday=&endyear=&keyword_list=on&p_start=40&p_finish=45&p_sort=&p_desc=DESC&p_direction=Prev&p_show=40">2</a>]. 
        </p>
        <p>
            Safety is of primary importance in established engineering fields, due to historical disasters that motivated and shaped regulations, education, and professional practice. Though safety is of growing interest in the relatively nascent field of <i>artificial intelligence</i> (AI) and the subfield of <i>machine learning</i> (ML), the primary emphasis in these fields remains on increasing capabilities without sufficient concern for risks, and sometimes without proper scientific evaluation [<a href="https://arxiv.org/pdf/1902.03271.pdf">1</a>]. With the rapid increase of AI and ML applications, the safety and fairness of such systems must become a primary focus if we hope to avoid the historical disasters that shaped established engineering fields. 
        </p>
    </div>

<div class="container p-3 my-5 border" style="background-color: #f3f4fc;">
    <h5 class="mb-3" id="probabilistic"><b>The necessity of <i>probabilistic</i> guarantees</b></h5>
    <hr class="my-4">
    <p>
        There are two possible types of safety and fairness guarantees: <b>deterministic</b> and <b>probabilistic</b> (also called <i>stochastic</i>). Deterministic guarantees hold with certainty. A <i>deterministic</i> guarantee that an ML system will not give a medical treatment that results in a patient dying means that the ML system will <i>never</i> give a medical treatment that results in a patient dying. As another example, Asimov's <a href="https://en.wikipedia.org/wiki/Three_Laws_of_Robotics">three laws of robotics</a> are three proposed deterministic safety constraints for robots.
    </p>
    <p>
        Unlike deterministic guarantees, probabilistic guarantees only hold with some probability (typically a "high probability"). This high probability is typically written in math as \(1-\delta\), where \(\delta\in(0,1)\) is a (typically small) constant. Common values of \(\delta\) include 0.1, 0.05, and 0.01, resulting in guarantees that hold with probability 0.9, 0.95, or 0.99, respectively. So, a \(1-\delta\) probability guarantee that an ML system will not give a medical treatment that results in a patient dying means that the probability that the ML system gives a medical treatment that results in the patiend dying will be at most \(1-\delta\).
    </p>
    <p>
        Obviously we prefer determistic guarantees over probabilistic guarantees. However, often deterministic guarantees are not possible, particularly when an ML systems must include data when reasoning about a guarantee. To really drive this point home, we provide multiple examples.
    </p>
    <ol>
        <li>
            <b>Sepsis treatment.</b> <a href="https://en.wikipedia.org/wiki/Sepsis">Sepsis</a> is a potentially life-threatening condition that arises when the body's response to infection damages its own tissues, and which is responsible for roughly <a href="https://www.who.int/news-room/fact-sheets/detail/sepsis">one in five deaths worldwide</a>. 
        </li>
        <li>
            <b>Loan approval.</b>
            TODO.
        </li>
        <li>
            <b>Warning systems.</b>
            Asdf.
        </li>
        <li>
            <b>Predicting violent recidivism.</b>
            Asdf.
        </li>
        <li>
            <b>Automated governance.</b>
            Asdf.
        </li>
    </ol>
</div>

<div class="container p-3 my-5 border" style="background-color: #f3f4fc;">
    <h5 class="mb-3" id="algorithm"><b>What is a Seldonian algorithm?</b></h5>
    <hr class="my-4">
    <p>TODO</p>
</div>

<div class="container p-3 my-5 border" style="background-color: #f3f4fc;">
    <h5 class="mb-3" id="framework"><b>What is the Seldonian framework?</b></h5>
    <hr class="my-4">
    <p>TODO</p>
</div>

<div class="container p-3 my-5 border" style="background-color: #f3f4fc;">
    <h5 class="mb-3" id="library"><b>What is this software library?</b></h5>
    <hr class="my-4">
    <p>TODO</p>
</div>

