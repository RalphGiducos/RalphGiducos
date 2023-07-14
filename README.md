const NFTs= []
function minNFT (_name,_shirtcolor,_capcolor,_theme) {

const NFT = {
    "name":_name,
    "shirtcolor":_shirtcolor,
    "capcolor":_capcolor,
    "theme":_theme
}
NFTs.push(NFT)
console.log("Minted: "+_name)
console.log("---------")
}

/////////////////////////
function listNFTs () {
for(var list = 0; list<NFTs.length;list++){
    console.log("NFT ID Number: \t"+ (list+1));
    console.log("Name: \t"+NFTs[list].name);
    console.log("Shirt Color: \t"+NFTs[list].shirtcolor);
    console.log("Cap Color: \t"+NFTs[list].capcolor);
    console.log("Theme: \t"+NFTs[list].theme);
    console.log("---------")
}
}
/////////////////////////

function getTotalSupply() {
    console.log(NFTs.length);
    console.log("---------")
}
////////////////////


minNFT("Hiro","black","darkblue","casual");
minNFT("Artis","blue","black","superhero");
minNFT("Mina","red","blue","futuristic");
minNFT("Mako","white","gray","plain")

listNFTs();
getTotalSupply();
