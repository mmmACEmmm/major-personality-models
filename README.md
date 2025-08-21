Developing an Advanced Personality Assessment System: Integrating Dynamic, Contextual and Cross-Cultural Insights
Abstract

Existing personality assessments, particularly type-based instruments such as the Myers-Briggs Type Indicator (MBTI) and early versions of the Jungian typology, remain popular in organisational and personal development contexts. However, many instruments rely on dichotomous categories, ignore situational variability, and offer limited cultural generalisability. Recent research in personality psychology emphasises both stability and malleability of traits across the lifespan and across contexts. This project integrates current scientific evidence on trait structure, cross-cultural measurement invariance, situational variation and personality plasticity to design a new assessment system. The deliverables include an academic review of existing models and their limitations, development of a multidimensional theoretical framework with eight continuous dimensions and sub-facets, a psychometric methodology for validating the proposed scales, and an interactive web-based assessment with context-dependent questions and real-time scoring. The new system moves beyond categorical types by using dimensional profiles, capturing trait distributions across work, relationship and leisure contexts, and accounting for temporal stability and change. It explicitly incorporates life events, social influence and cultural context while preserving psychometric rigor. The result is an assessment tool suitable for research, counselling and self-development that bridges the gap between personality science and practical application.

1. Introduction

Personality assessment has long fascinated psychologists, educators and employers because it offers the promise of understanding individual differences in behaviour and predicting performance in different life domains. Instruments like the MBTI and the Big Five Inventory (BFI) are widely used despite debates about their scientific validity. The MBTI divides people into 16 types based on four dichotomies (Extraversion–Introversion, Sensing–Intuition, Thinking–Feeling and Judging–Perceiving). Its popularity stems from the intuitive appeal of type labels and the ease with which non-experts can interpret results. Proponents report reliability coefficients in the .80–.87 range and test–retest coefficients around .81–.86 for Step I scales
myersbriggs.org
, and The Myers-Briggs Company emphasises that updated global forms are based on a common dataset of 16,733 participants and can be administered worldwide
themyersbriggs.com
. Critics, however, note that the MBTI’s forced dichotomies ignore continuous trait distributions, leading to low test–retest stability and poor predictive validity
truity.com
truity.com.

Trait-based models such as the Five-Factor Model (FFM) emerged from lexical and statistical approaches and conceptualise personality along continuous dimensions of Neuroticism, Extraversion, Openness, Agreeableness and Conscientiousness. These models show high genetic and rank-order stability in adulthood and modest mean-level changes over time
pmc.ncbi.nlm.nih.gov
pmc.ncbi.nlm.nih.gov.
Yet self-report inventories remain vulnerable to social desirability and response biases. The standard FFM assumes orthogonal factors, but factor analytic studies sometimes yield correlated factors, raising questions about independence
en.wikipedia.org
. Moreover, the FFM was developed primarily in Western cultures. While cross-cultural projects such as the Personality Profiles of Cultures (PPOC) replicated the five-factor structure in 50 cultures
pmc.ncbi.nlm.nih.gov
and showed that maturational patterns and sex differences appear pancultural
pmc.ncbi.nlm.nih.gov
, critics argue that some culturally specific constructs may be missed
pmc.ncbi.nlm.nih.gov
and that translation and sampling issues can compromise invariance
pmc.ncbi.nlm.nih.gov
. Meta-analyses of the BFI across 57 languages report internal consistency coefficients around .77–.89
bmcpsychology.biomedcentral.com
, yet measurement invariance testing reveals minor noninvariant loadings across languages
pmc.ncbi.nlm.nih.gov.

Alternative models aim to capture nuances beyond the FFM. The HEXACO framework adds Honesty–Humility as a sixth factor and redefines Agreeableness and Emotionality. It offers theoretical advantages, especially in predicting counterproductive behaviour, but replication across cultures is mixed and the Honesty–Humility dimension does not consistently emerge
en.wikipedia.org
. Popular articles note that results can “box people in” and ignore personality change over time
verywellmind.com
. Other taxonomies, such as the Personality Systems Interaction (PSI) theory and the Trait Activation framework, emphasise dynamic interaction between traits, motives and situational cues. Meanwhile, psychometrics has advanced with item response theory, multilevel modelling and network analysis, allowing more sophisticated measurement of trait states and their covariance structures.

Recent developments highlight that personality traits are both stable and malleable. Longitudinal analyses with Mexican-origin adults show rank-order stability coefficients between .66 and .80, but also small linear mean-level decreases across adulthood
pmc.ncbi.nlm.nih.gov
. Experience-sampling studies reveal high within-person variability in trait enactments
pmc.ncbi.nlm.nih.gov
, supporting density distribution models in which traits represent distributions of states rather than fixed points. Situations—work, family, relationships, leisure—induce different trait expressions
pmc.ncbi.nlm.nih.gov
. A systematic review of volitional personality change studies found that simply desiring change had minimal impact, but structured interventions produced small yet durable changes (d≈0.22–0.37)
pmc.ncbi.nlm.nih.gov
. Exposure to extreme life events, such as trauma, leads to increases in Neuroticism and decreases in Agreeableness and Openness
pmc.ncbi.nlm.nih.gov
. These findings challenge the view of fixed “types” and underscore the need for assessments that accommodate variability across contexts, cultures and time.

This project addresses the limitations of existing tools by developing an advanced personality assessment system grounded in contemporary research. It emphasises dimensional measurement, situational specificity, cultural validity and dynamism over time. Section 2 reviews the literature on current personality models. Section 3 introduces a novel theoretical framework with eight primary dimensions and sub-facets. Section 4 outlines the psychometric methodology for validating the system. Section 5 details the design of the multidimensional assessment, including context-specific questions and dynamic scoring. Section 6 discusses applications and ethical considerations. The accompanying interactive tool demonstrates the practical implementation.

2. Literature review
2.1. Myers-Briggs Type Indicator and type-based models

The MBTI remains one of the most widely recognised personality assessments. Its four dichotomies—Extraversion–Introversion, Sensing–Intuition, Thinking–Feeling and Judging–Perceiving—are purported to measure mental functions derived from Jungian theory. The instrument divides individuals into 16 types. Proponents highlight research demonstrating internal consistency and test–retest reliability around .80–.87
myersbriggs.org
and emphasise the instrument’s applicability across cultures through a global data set and unified questionnaire
themyersbriggs.com
. However, much of this evidence is proprietary and rarely published in peer-reviewed journals, limiting independent verification. Meta-analytic reviews find that MBTI scales correlate strongly with corresponding Big Five traits (e.g., Extraversion and Introversion correlate roughly −0.74 with Big Five Extraversion), suggesting construct redundancy. Scores on MBTI dichotomies are normally distributed, undermining the typological assumption. A key criticism is the loss of information when continuous traits are dichotomised: individuals near the scale midpoint may flip types with minimal score changes, reducing test–retest reliability and predictive validity
truity.com.

The MBTI’s face validity and positive language make it appealing for coaching and team-building workshops, but there is scant evidence that it predicts job performance or other life outcomes beyond the FFM. Because the MBTI was not designed as a clinical instrument, misuse in selection contexts raises ethical concerns. Self-report items are susceptible to faking and social desirability. In non-Western cultures, translation and cultural adaptation issues further compromise validity, although the global form attempts to address this by using a common item set
themyersbriggs.com
. Overall, while the MBTI offers a simple introduction to typological thinking, its psychometric limitations call for more sophisticated models.

2.2. Five-Factor Model and derivatives

The Big Five or Five-Factor Model (FFM) emerged from lexical and questionnaire research identifying five orthogonal factors—Neuroticism, Extraversion, Openness to Experience, Agreeableness and Conscientiousness. This model enjoys broad empirical support. Twin and molecular genetic studies estimate that about 50% of variance in the five factors is heritable
pmc.ncbi.nlm.nih.gov
. Rank-order stability correlations around .75 in adulthood
pmc.ncbi.nlm.nih.gov
and cross-decade stability coefficients around .31 over 50 years
pmc.ncbi.nlm.nih.gov
demonstrate enduring individual differences. Longitudinal studies show normative declines in Neuroticism, Extraversion and Openness and increases in Agreeableness and Conscientiousness with age
pmc.ncbi.nlm.nih.gov
, although mean changes are small and cultural differences modulate the trajectories
pmc.ncbi.nlm.nih.gov
. A meta-analysis across 57 languages reports reliability coefficients (Cronbach’s α) for BFI and BFI-2 scales ranging from .73 to .89
bmcpsychology.biomedcentral.com
, indicating acceptable internal consistency.

Despite these strengths, several limitations motivate further development. First, FFM factors are not perfectly orthogonal; correlations among factors occur in many samples, and personality profiles may be better captured by higher-order factors such as Stability and Plasticity. Second, self-report measures suffer from social desirability bias and lack of ecological validity
en.wikipedia.org
. Third, the FFM may be incomplete: important constructs such as honesty–humility, impulse control, creativity or adaptability are not explicitly represented. Fourth, cross-cultural research reveals both universality and specificity. The PPOC project found that the NEO-PI-R factor structure was recognisable in 50 cultures
pmc.ncbi.nlm.nih.gov
, but some cultures emphasise interpersonal harmony or collective responsibilities not captured by the FFM. Gender differences show pancultural patterns—women score higher on facets of Agreeableness and Neuroticism—yet the magnitude of differences varies, being largest in wealthy, individualistic societies
pmc.ncbi.nlm.nih.gov
pmc.ncbi.nlm.nih.gov
. Age differences also show modest, gradual trends across cultures
pmc.ncbi.nlm.nih.gov
. These findings highlight the need for assessments that capture both universal dimensions and culturally specific nuances.
pmc.ncbi.nlm.nih.gov

2.3. HEXACO and extended trait models

The HEXACO model extends the FFM by adding a Honesty–Humility dimension (sincerity, fairness, greed-avoidance and modesty) and redefining Agreeableness and Emotionality. It predicts counterproductive workplace behaviour and exploitative tendencies better than the FFM, as Honesty–Humility is linked to ethical decision-making. However, factor analytic replication is inconsistent; only Extraversion, Agreeableness and Conscientiousness consistently replicate across cultures
en.wikipedia.org
. The Honesty–Humility factor may merge with low Neuroticism or high Conscientiousness in some samples, raising questions about its distinctiveness. Critics argue that the emphasis on lexical derivation might lead to overfitting idiosyncratic item clusters. Practical limitations mirror those of the FFM: self-report biases, limited situational sensitivity, and the risk of reifying traits as fixed labels. Popular articles warn that test results can “box people in” and neglect personality development over time
verywellmind.com.

2.4. Other taxonomies and integrative models

Beyond the FFM and HEXACO, numerous models attempt to integrate traits with motives, values and situational variables. The Personality Systems Interaction (PSI) theory links personality to motivational and volitional systems, emphasising dynamic regulation of behaviour. The Trait Activation model proposes that traits are expressed when situations provide relevant cues. Network models conceptualise traits as networks of behaviours and experiences rather than latent variables. Cross-cultural psychologists also propose emic constructs (e.g., Chinese “interpersonal relatedness”). While these frameworks offer nuanced perspectives, they often lack standardised assessments or have limited empirical validation compared with the FFM.

2.5. Personality stability, plasticity and situational variability

Personality exhibits both stability and change. Longitudinal research on Mexican-origin adults shows high rank-order stability (r≈.66–.80) but small mean-level decreases across adulthood, with few associations to sociodemographic or cultural factors
pmc.ncbi.nlm.nih.gov
. Meta-analyses conclude that all traits show small mean-level changes throughout the lifespan and that people continue to change across decades
pmc.ncbi.nlm.nih.gov
. Young people and older adults show lower rank-order stability than middle-aged adults
pmc.ncbi.nlm.nih.gov
. Situations modulate trait expression. Mischel’s critique of trait consistency highlighted the role of contexts
pmc.ncbi.nlm.nih.gov
, prompting the development of situational taxonomies such as DIAMONDS, Situation Five and CAPTION, which describe social situations along dimensions like Duty, Intellect, Adversity, Mating, pOsitivity, Negativity, Deception and Sociality
pmc.ncbi.nlm.nih.gov
. Empirical studies show that romantic relationships increase Neuroticism and Extraversion whereas work situations increase Agreeableness, Conscientiousness, Openness and Neuroticism
pmc.ncbi.nlm.nih.gov
. Experience-sampling research demonstrates that within-person variability in trait enactments exceeds between-person variability
pmc.ncbi.nlm.nih.gov
. These density distribution models conceptualise traits as distributions of states; the mean of the distribution corresponds to the latent trait level, while variability reflects flexibility or situational responsiveness.

Personality change can be volitional. A systematic review identified 30 longitudinal studies examining self-directed personality change. Merely setting goals to change one’s traits had little effect, but structured interventions (e.g., cognitive behavioural therapy, coaching, mindfulness) produced small yet lasting changes with effect sizes around d = 0.22 and persistence of d ≈ 0.37 at follow-up
pmc.ncbi.nlm.nih.gov
. The authors concluded that personality is malleable when individuals have motivation, believe change is possible, practise new behaviours and receive feedback
pmc.ncbi.nlm.nih.gov
. On the other hand, exposure to extreme life events can induce undesirable changes: an urban longitudinal study found that participants who experienced extremely adverse events within two years showed increases in Neuroticism and decreases in Agreeableness and Openness
pmc.ncbi.nlm.nih.gov
. Baseline low Extraversion and Conscientiousness predicted poorer adjustment after trauma
pmc.ncbi.nlm.nih.gov
. Such findings underscore the need to consider temporal fluctuation, role transitions and life events in personality assessment.

2.6. Cultural validity and measurement invariance

Cross-cultural research asks whether personality constructs derived in Western contexts generalise to other societies. The FFM appears to capture universal personality dimensions: factor replicability of the NEO-PI-R in translations across 50 cultures is high
pmc.ncbi.nlm.nih.gov
, maturational patterns and sex differences show cultural invariance
pmc.ncbi.nlm.nih.gov
, and cross-national mean profiles cluster geographically (e.g., Asian and African cultures cluster together away from Western cultures)
pmc.ncbi.nlm.nih.gov
. However, cultural specifics remain important. Some cultures include constructs such as interpersonal relatedness that are not captured by the FFM; response styles differ across cultures; and many cross-cultural datasets rely on convenience samples or college students
pmc.ncbi.nlm.nih.gov
. Measurement invariance studies of short questionnaires show that factor structures are broadly invariant across Spanish and English speakers, with only minor intercept and loading differences
pmc.ncbi.nlm.nih.gov
. Spanish speakers scored higher on some conscientiousness and openness items whereas English speakers scored higher on certain extraversion and agreeableness items
pmc.ncbi.nlm.nih.gov
. Internalising symptoms (e.g., depression, anxiety) were chiefly related to low emotional stability, and antisocial behaviour was associated with low Agreeableness and Conscientiousness across countries
pmc.ncbi.nlm.nih.gov
. The authors concluded that the short questionnaire is sufficiently invariant across languages and genders for young adults from the USA, Argentina and Spain
pmc.ncbi.nlm.nih.gov.

3. Theoretical framework for an advanced personality model
3.1. Design principles

The limitations discussed above motivate design principles for a new model. First, the model must be dimensional rather than typological. Continuous scales preserve information, improve reliability and allow nuanced descriptions. Second, it must integrate situational context. Traits are enacted differently at work, in relationships and during leisure; an assessment must track these expressions. Third, it should capture both stability and plasticity. People exhibit stable dispositions but also adapt to roles, life events and developmental stages. Fourth, it must be culturally generalisable yet sensitive to cultural variation. This requires measurement invariance testing, translation procedures and inclusion of emic constructs when necessary. Fifth, the model should include ethically relevant dimensions like integrity and adaptability that predict behaviour beyond the FFM.

3.2. Primary dimensions and sub-facets

Based on these principles and empirical evidence, we propose an eight-dimension model: Social Connectivity (SC), Cognitive Exploration (CE), Emotional Regulation (ER), Agreeableness/Empathy (AE), Conscientiousness/Self-Discipline (CS), Integrity/Honesty (IH), Adaptability/Flexibility (AF) and Creativity/Ingenuity (CI). These dimensions are continuous and orthogonal by design but may correlate in samples; higher-order factors (e.g., Stability vs. Plasticity) can be derived. Each dimension contains sub-facets (three to five) informed by the literature.

Social Connectivity reflects quantity and quality of interpersonal interaction. Sub-facets include sociability (desire for company), assertiveness (comfort initiating contact), collaboration (preference for teamwork), networking (ability to develop new relationships) and supportiveness (tendency to provide social support). It expands on FFM Extraversion by distinguishing networking from sociability and by including pro-social aspects not captured by pure energy or dominance. This dimension is sensitive to cultural norms around extraversion; high SC may manifest differently in collectivist cultures where social harmony is valued.
pmc.ncbi.nlm.nih.gov

Cognitive Exploration describes curiosity, openness to new experiences and intellectual engagement. Sub-facets include intellectual curiosity (desire to learn), aesthetic appreciation (sensitivity to art and beauty), divergent thinking (ability to generate novel ideas), critical thinking (willingness to question assumptions) and cognitive flexibility (shifting perspectives). It draws from FFM Openness and incorporates aspects of cognitive reflection and exploratory behaviour. High scores indicate broad interests and a preference for novelty; low scores indicate preference for routine and tradition.

Emotional Regulation measures resilience, stress management and affective balance. Sub-facets include stress tolerance, impulse control, recovery (speed of returning to baseline after stress), emotional awareness (recognition of one’s emotions) and self-soothing (use of strategies to regulate mood). Unlike FFM Neuroticism, which emphasises negative affectivity, ER covers positive coping and adaptive regulation. It addresses findings that trait variability across situations is partly due to affect regulation
pmc.ncbi.nlm.nih.gov
and that emotional stability is associated with well-being
pmc.ncbi.nlm.nih.gov.

Agreeableness/Empathy captures pro-social orientation, empathy and cooperation. Sub-facets include empathic concern (tendency to understand and share others’ feelings), cooperation (willingness to work with others), conflict resolution, gratitude and forgiveness. This dimension combines FFM Agreeableness with aspects of compassion training and emphasises interpersonal warmth and fairness.
pmc.ncbi.nlm.nih.gov
It correlates negatively with antisocial behaviour and predicts relationship satisfaction.

Conscientiousness/Self-Discipline measures organised, goal-directed behaviour. Sub-facets include planning, orderliness, responsibility, perseverance and achievement striving. It aligns with FFM Conscientiousness but emphasises self-discipline as a separate facet. High scores predict academic and occupational success and lower risk of externalising problems.
pmc.ncbi.nlm.nih.gov

Integrity/Honesty reflects moral character, fairness and adherence to principles. Sub-facets include sincerity, fairness, accountability, modesty and ethical courage. This dimension builds on the HEXACO Honesty–Humility factor but broadens it by including accountability and ethical courage. It predicts trustworthiness and resistance to corruption. Cultural differences may influence the behavioural expression of integrity; cross-cultural research shows that honesty is valued across cultures but the form of expression varies
en.wikipedia.org.

Adaptability/Flexibility captures how individuals adjust to changing circumstances, roles and cultures. Sub-facets include situational flexibility (ability to modify behaviour across contexts), learning agility (willingness to acquire new skills), role switching (managing multiple roles), tolerance for ambiguity, and change optimism (seeing change as opportunity). This dimension responds to evidence that personality traits vary across situations
pmc.ncbi.nlm.nih.gov
and that adaptability predicts resilience during life transitions. It is absent from the FFM and HEXACO.

Creativity/Ingenuity measures the tendency to generate novel ideas and approaches. Sub-facets include ideation, problem-solving originality, innovation courage, pattern recognition and boundary breaking. Creativity is partially subsumed under FFM Openness but merits its own dimension given its importance in modern work, entrepreneurship and artistic pursuits. This dimension interacts with Cognitive Exploration and Adaptability; high creative individuals often excel in divergent thinking and adjust their methods when faced with novel problems.

These eight dimensions offer a richer description of personality than four MBTI dichotomies or the FFM’s five factors. The inclusion of Integrity/Honesty and Adaptability acknowledges moral and situational aspects ignored in earlier models. The separation of Emotional Regulation from negative affect emphasises resilience rather than trait neuroticism. Creativity is recognised as a distinct trait relevant to innovation. Each dimension is measured along continuous scales, and sub-facet scores enable finer granularity. Importantly, context-specific measurement captures how these dimensions manifest differently at work, in relationships and during leisure or creative activities.

3.3. Interaction effects and role flexibility

Personality dimensions interact. For example, high Conscientiousness enhances the implementation of Cognitive Exploration and Creativity by providing discipline to pursue complex ideas. High Adaptability may moderate the expression of Social Connectivity when individuals adjust their engagement based on group dynamics. Emotional Regulation facilitates the expression of Agreeableness under stress. To model these interactions, the system will compute multiplicative scores between dimensions and examine cross-situational patterns. Role flexibility refers to an individual’s ability to shift their dominant trait expression depending on context. For instance, a person may exhibit high Social Connectivity and low Emotional Regulation in social settings but moderate those traits during solitary creative work. Assessing role flexibility requires measuring each dimension across contexts and computing variability indices (e.g., within-person standard deviation). High variability indicates flexibility; low variability suggests consistency or rigidity. The inclusion of Adaptability captures this meta-dimension explicitly.

4. Methodology
4.1. Item generation and contextualisation

Items will be developed through a multi-stage process. First, behavioural descriptors for each sub-facet are generated from literature review and qualitative interviews. Second, descriptors are transformed into Likert-scale items referencing specific contexts. The contexts selected—work, relationships and leisure—were identified through pilot interviews where participants listed the most frequent situations in their lives and were grouped into these supra-categories
pmc.ncbi.nlm.nih.gov
. For each dimension, five behavioural statements per context are created, resulting in 15 items per dimension and 120 items overall. Items are phrased in clear language and anchored on a seven-point scale to capture subtle differences
pmc.ncbi.nlm.nih.gov
. Reverse-scored items are included to reduce acquiescence bias; analyses will check for method factors. Cognitive interviews ensure items are interpreted consistently across cultures. Items are translated using forward–backward translation and reviewed by bilingual experts.

4.2. Sampling and data collection

Validation requires large, diverse samples. A planned sample of at least 1,500 participants will be recruited across multiple cultures using stratified sampling to ensure variation in age, gender, socioeconomic status and cultural background. Power analysis (α = .05, power =.80, effect size f = .25) suggests at least 45 participants for each subgroup in a MANOVA
pmc.ncbi.nlm.nih.gov
; the larger sample provides stable estimates for factor analysis and measurement invariance testing. Participants complete the online assessment, providing demographic information, and retake the test after six months to assess test–retest reliability. For cross-cultural validity, translated forms are administered in Spanish, English and other languages; measurement invariance will be assessed using multi-group confirmatory factor analysis.
pmc.ncbi.nlm.nih.gov

4.3. Statistical analysis

Factor structure: Exploratory factor analysis (EFA) will initially test the eight-factor structure using polychoric correlations and parallel analysis. Confirmatory factor analysis (CFA) will then evaluate model fit (CFI, TLI, RMSEA). Bifactor models will examine whether higher-order factors (e.g., Stability vs. Plasticity) improve fit. Reliability will be assessed via Cronbach’s α and McDonald’s ω for each dimension and sub-facet; values above .70 indicate acceptable internal consistency. Test–retest reliability will be computed using intra-class correlation coefficients over the six-month interval. Measurement invariance across languages, sexes and cultures will be evaluated in multiple steps (configural, metric, scalar). Past research shows that only minor intercepts and loadings differ across languages
pmc.ncbi.nlm.nih.gov
. Convergent and discriminant validity will be examined by correlating dimension scores with established instruments (e.g., BFI, HEXACO). We expect moderate correlations with corresponding traits (e.g., Social Connectivity with Extraversion) and lower correlations with unrelated traits. Criterion validity will be tested by correlating dimension scores with external outcomes such as job performance ratings, relationship satisfaction, stress biomarkers and creative achievement. Associations between low Emotional Regulation and internalising symptoms, and between low Agreeableness or low Conscientiousness and antisocial behaviour, are expected based on prior findings
pmc.ncbi.nlm.nih.gov
. Predictive validity for life outcomes (health, educational attainment, resilience to life events) will be assessed using longitudinal data.

4.4. Modeling situational variation and temporal stability

The assessment produces not only trait scores but also indices of situational variability. For each dimension, we compute the standard deviation of responses across contexts; higher variability indicates greater situational flexibility. We also derive a cross-situational variability (CSV) index similar to the Across-Situation Variability (ASV) metric proposed by Nasello and colleagues
pmc.ncbi.nlm.nih.gov
. Persons with high CSV exhibit large differences in trait expression across work, relationships and leisure; low CSV indicates consistency. Correlations between CSV and personality dimensions, especially Conscientiousness and Neuroticism, will be examined to replicate the finding that conscientious individuals show lower variability
pmc.ncbi.nlm.nih.gov
. Temporal stability will be measured using test–retest correlations; changes will be correlated with life events and intervention participation. The volitional change literature suggests small but significant increases in traits targeted by interventions
pmc.ncbi.nlm.nih.gov
. Modeling will use multi-level analyses with observations nested within individuals across time and contexts.

4.5. Handling response biases and social desirability

To reduce social desirability bias, items include neutral phrasing and reversed content. A short social desirability scale (e.g., the Marlowe–Crowne Social Desirability Scale) is included, allowing partial correlation and residualisation of trait scores. Response time can be recorded to detect inattentive responding. Balanced keying and randomised item order further mitigate acquiescence. Factor analyses will examine method factors for reversed items. Online administration includes attention checks (e.g., “Select option three to show you are paying attention”). Participants can review confidentiality information and skip questions they find uncomfortable.

5. Novel personality system design
5.1. Dimensional profiles and classification

Each participant receives a continuous score (0–100) on the eight primary dimensions. Instead of assigning a single type, we classify individuals into one of 64 profiles by trichotomising each dimension (low, moderate or high) based on normative distributions. For eight dimensions, 3^8 = 6,561 possible combinations; however, many patterns are rare or similar. We cluster dimension scores using k-means and hierarchical clustering on a normative sample, selecting 64 clusters that maximise between-cluster distance and interpretability. Each cluster description includes typical strengths, development areas and context-specific patterns. Clusters are labelled descriptively (e.g., “Innovative Connector” for high SC, high CI, moderate CE and high AF; “Structured Supporter” for moderate SC, high CS and high AE). Users can explore how small changes in scores reassign them to different clusters, emphasising dimensional rather than categorical thinking.

5.2. Contextual profiles and role flexibility

For each context, we compute dimension scores, enabling comparison across work, relationships and leisure. This yields a contextual profile that highlights role flexibility. A person may be highly disciplined and conscientious at work but more relaxed during leisure. A variability index quantifies differences. High variability may be adaptive (flexibility) or maladaptive (inconsistency) depending on the dimension. For example, high variability in Emotional Regulation could indicate situational triggers of stress; high variability in Social Connectivity could reflect social anxiety in some contexts but not others. Practitioners can interpret patterns relative to life circumstances and goals. The system encourages users to reflect on how environmental demands and personal values shape their personality expressions.
pmc.ncbi.nlm.nih.gov

5.3. Temporal change indicators

Test–retest data provide change indicators. We compute change scores (difference and residual change) and classify changes as significant using reliable change indices. Users receive feedback on which dimensions increased or decreased. Combined with life event diaries, the system can highlight possible triggers (e.g., a promotion, moving countries). This aligns with research showing that extreme events increase Neuroticism and decrease Agreeableness and Openness
pmc.ncbi.nlm.nih.gov
. Users are cautioned that personality change often occurs slowly and that measurement error can mimic change.

5.4. Dynamic assessment and adaptive testing

The assessment includes an adaptive element. After two items for a dimension are answered, the system computes the average. If the average is very high or very low (≥6 or ≤2), subsequent items in that dimension are skipped to reduce respondent burden—an approach implemented in the accompanying HTML tool. This design follows the dynamic skipping logic described in Section 5 of the implementation. Adaptive testing shortens completion time while maintaining accuracy. The algorithm is calibrated using item response theory to ensure that early items are highly discriminating.

6. Implementation: interactive HTML assessment tool

An interactive web-based assessment demonstrates the proposed system. The tool is built using HTML, CSS and JavaScript and includes 120 context-specific items (15 per dimension). Items are dynamically generated by combining base statements with contextual prefixes (“At work …”, “In my relationships …”, “During leisure time …”). Questions are presented one at a time with a 1–7 response scale. A progress bar shows completion. Dynamic branching skips remaining items in a dimension when early responses indicate extreme scores, reducing respondent fatigue. Upon completion, the tool computes dimension scores by scaling averages from 1–7 to 0–100. It calculates context-specific averages and displays results in a radar chart using Chart.js. A textual summary lists dimension scores, highlights the participant’s strongest and weakest dimensions and provides general development suggestions. The results emphasise that personality is dynamic and encourage retesting during different life phases.

The tool is responsive and works on mobile and desktop browsers. Client-side code avoids storing personal data on servers, preserving privacy. Optionally, responses can be encrypted and uploaded for research with participant consent. The codebase uses modern JavaScript (ES6), separates concerns by modularising question generation and result computation, and comments key functions for maintainability. Accessibility considerations include keyboard navigation, ARIA labels for radio buttons and high-contrast colours for the progress bar.

7. Applications and practical implications
7.1. Career counselling and professional development

Employers often use personality assessments for selection or development. While the MBTI is popular, its predictive validity for job performance is low
truity.com
. The proposed system provides nuanced profiles across eight dimensions relevant to workplace behaviour, such as Conscientiousness/Self-Discipline, Adaptability/Flexibility and Integrity/Honesty. Counselors can use scores to identify strengths (e.g., high Conscientiousness suggests reliability) and areas for growth (e.g., low Adaptability indicates difficulty coping with change). Contextual profiles show whether someone behaves differently at work versus leisure, which can inform interventions like time management training or stress reduction. Because the assessment measures integrity, organisations can use it to support ethics programmes rather than to exclude applicants, avoiding discriminatory use. Development recommendations emphasise personal growth rather than selection decisions.

7.2. Relationship and social applications

Personality shapes relationship satisfaction and conflict. High Agreeableness/Empathy and Emotional Regulation predict positive relationship outcomes, whereas low scores may contribute to conflict. The contextual nature of the assessment allows users to see differences between how they interact with partners and friends versus colleagues. Feedback encourages reflection on empathy, communication and conflict resolution. Couples or family therapists can use results to facilitate discussions about each partner’s strengths and needs. Because personality can change through targeted interventions
pmc.ncbi.nlm.nih.gov
, therapists can set goals for developing empathy or emotional regulation. The system also highlights that high variability across contexts may be adaptive—for example, one can be assertive at work but supportive at home.

7.3. Personal growth and self-awareness

Individuals seeking self-understanding can benefit from an assessment that recognises both stable dispositions and situational flexibility. The tool provides personalised insights and encourages users to track changes over time. Since personality traits are linked to well-being, health and educational attainment
pmc.ncbi.nlm.nih.gov
, understanding one’s profile can inform lifestyle choices. Users may discover that high Creativity/Ingenuity and Cognitive Exploration align with careers in innovation, while high Integrity/Honesty and Conscientiousness support roles requiring trust. Feedback on low Adaptability or Emotional Regulation can motivate skills training or mindfulness practices. Because the system emphasises that personality is dynamic, users are less likely to feel pigeonholed by labels.

7.4. Team building and organisational development

Teams benefit from diversity of traits. By profiling entire teams on the eight dimensions, managers can identify complementary strengths and potential gaps. For instance, a team lacking high Creativity/Ingenuity may struggle to innovate, while a team with low Integrity/Honesty may face ethical challenges. Contextual data show whether team members behave differently under stress (work context) versus informal settings (leisure context). Workshops can use aggregated profiles to discuss communication styles, conflict management and decision-making. Because measurement invariance is assessed across cultures, the tool is suitable for multinational teams.
pmc.ncbi.nlm.nih.gov
Organisations should avoid using the tool for high-stakes selection without considering legal and ethical implications and should focus on development and team cohesion.

7.5. Therapeutic and counselling contexts

Clinicians can use the assessment to inform treatment planning. High Neuroticism (low Emotional Regulation) is associated with internalising disorders; low Agreeableness/Empathy and low Conscientiousness/Self-Discipline relate to externalising disorders
pmc.ncbi.nlm.nih.gov
. Cross-situational variability indices may reveal unstable self-concepts or context-dependent symptoms. Monitoring change over time helps clinicians evaluate therapy effectiveness. The volitional change literature shows that interventions can produce small but meaningful personality changes
pmc.ncbi.nlm.nih.gov
. Integrating personality assessment with clinical work promotes personalised care.

8. Ethical considerations

Personality assessments raise ethical issues. Data privacy is paramount; the tool should anonymise responses and comply with data protection regulations (e.g., GDPR). Informed consent must outline how data are used and stored. The assessment is designed for self-awareness and development, not for screening or selection. Using personality scores to make high-impact decisions (e.g., employment, insurance) risks discrimination and may contravene equal opportunity principles. Practitioners should be trained to interpret scores responsibly and avoid deterministic conclusions. Cultural sensitivity is critical: translation should respect linguistic nuances and avoid imposing Western concepts. Although measurement invariance testing suggests cross-language applicability
pmc.ncbi.nlm.nih.gov
, cultural context may influence interpretation. Users should be informed about the model’s developmental nature and limitations; high variability or low scores do not imply pathology. Continuous research is needed to update norms and ensure fairness across demographics.

9. Conclusion

The present project integrates decades of personality research with advances in psychometrics to create an assessment system that transcends traditional type indicators. The literature review highlighted limitations of typological tools like the MBTI—dichotomous scoring, poor predictive validity and cultural issues—and limitations of trait models such as the FFM and HEXACO, including incomplete coverage of moral and adaptability constructs and reliance on self-report
truity.com
en.wikipedia.org
. Empirical studies demonstrate that personality is both stable and plastic; trait expressions vary across situations, cultures and life events
pmc.ncbi.nlm.nih.gov
pmc.ncbi.nlm.nih.gov
. Volitional changes and interventions can produce meaningful improvements
pmc.ncbi.nlm.nih.gov
. Cross-cultural research supports universality of broad dimensions but also reveals cultural specificity and measurement challenges
pmc.ncbi.nlm.nih.gov
pmc.ncbi.nlm.nih.gov.

Building on these insights, we proposed an eight-dimension model that incorporates Social Connectivity, Cognitive Exploration, Emotional Regulation, Agreeableness/Empathy, Conscientiousness/Self-Discipline, Integrity/Honesty, Adaptability/Flexibility and Creativity/Ingenuity. The model emphasises continuous measurement, situational context and temporal dynamics. A rigorous methodology includes item development, cross-cultural translation, factor analysis, reliability testing and criterion validation. The resulting assessment yields dimensional profiles, contextual variability indices and change indicators. An interactive HTML tool implements the assessment with dynamic branching, real-time scoring and visualisation. Applications span career counselling, relationships, personal growth, team development and clinical contexts. Ethical guidelines underscore privacy, fair use and cultural sensitivity. By integrating dynamic, contextual and cross-cultural perspectives, the proposed system offers a scientifically grounded alternative to existing personality assessments and sets a foundation for future research and practical applications in personality psychology.
