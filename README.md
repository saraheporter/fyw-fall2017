# fyw-fall2017

Documentation for the different elements and attributes in the remiXML schema. 

## Elements:

**\<analysis\>** under the "original" element, the analysis element indicates the text you chose to mark up is the text you will analyze under the "play" element. In the "play" element, you write our your analysis of the particular moment you marked up.

**\<doc-title\>** the title of the remixed XML document; I encourage you to be more creative than "Remix of Original Title." Think about the main ways you have chosen to remix the text; what moments did you choose and why? How did you remix them?

**\<expand\>** under the "original" element, the expand element indicates the text you chose to mark up is the text you will expand under the "play" element. In the "play" element, you write our your expansion of the particular moment you marked up.

**\<metadata\>** the first main tag that contains information about yourself, the document name, the original writer, and more

**\<original\>** the second main tag that contains the original text to be marked-up 

**\<original-title\>** the title of the original text

**\<p\>** to indicate a paragraph break

**\<play\>** the third main tag that consists of content created as the original text is being read and marked-up

**\<question\>** under the "original" element, the question element indicates the text you chose to mark up is the text you will ask a question about under the "play" element. In the "play" element, you write our your question of the particular moment you marked up.

**\<remiXML\>** the root element; this is the tag that surroungs the metadata, original, and play elements

**\<transform\>** under the "original" element, the transform element indicates the text you chose to mark up is the text you will transform under the "play" element. In the "play" element, you write our your transformation of the particular moment you marked up. You may base these transformations off those we read in "Restorying in Self"

## Attributes:

**ID** The ID attribute will be used in two elements: the **\<original-writer\>** and the **\<remixer\>** element. The attribute value of the ID will be the unique identifier for the original writer (IF the original writer is yourself) and the remixer (whether the remixer is yourself or your peer). Use your initials and number as the ID: my ID is CM1

**remixerID** This is the same remixer ID that you used in the ID attribute in <remixer>. This will help to diferentiate who has marked up the text, especially if it is a peer engaging with another peers' work

**playID** In the **\<original\>** text, this attribute will signal that moment in the text you have decided to wrap in an element (analysis, expand, question, transform) and label it. This ID must be the same ID you use in the **\<play\>** section. For example, if you mark up a particular section in the original text for analysis, in the play section, be sure your analysis has the same ID. This will link your analysis to the moment in the original text.

**playREF** In the **\<play\>** section, this attribute (playREF stands for play reference, indicating that you are referencing something from the original text) will be the same as the playID you used to markup the particular moment you want to play with. Example: in the \<original\> section, you decide to mark up a moment you want to expand. This moment as a playID. In the <play> section, you use the \<expand\> element in which you will actually write the expansion; for the "playREF" attribute of this expand element, you will use the same ID number (for example: playID="EX1" and playREF="EX2").

## Breakdown:

    \<metadata\>

      \<original-title\>
    
      \<doc-title\>
    
      \<original-writer\>
    
          ID
     \<remixer\>
    
         ID
        
    \<original\>

      \<p\>
    
         \<analysis\>
        
              playID
            
             remixerID
            
          \<expand\>
        
              playID
            
              remixerID
            
          \<question\>
        
              playID
             
             remixerID
            
         \<transform\>
        
              playID
            
             remixerID
            
    \<play\>

       \<analysis\>
     
          playREF
        
       \<expand\>
     
         playREF
         
       \<question\>
     
          playREF
        
      \<transform\>
     
         playREF

