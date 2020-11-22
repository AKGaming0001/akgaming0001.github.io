displayAds = true;

function noAds() {
    console.log("AdBlock detected!");
    displayAds = false;
    
    let adContainers = document.getElementsByClassName("adContainer"),
        footer = document.getElementById("footer"),
        paypalContainer = document.createElement("div"),
        paypalTable = document.createElement("table"),
        paypalTableRow = document.createElement("tr"),
        paypalTableCell1 = document.createElement("td"),
        paypalTableCell2 = document.createElement("td"),
        paypalButton = `<form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_blank" style="display:inline-block"><input type="hidden" name="cmd" value="_s-xclick"/><input type="hidden" name="hosted_button_id" value="C5CLJ64PC83ES"/><input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" border="0" name="submit" title="PayPal - The safer, easier way to pay online!" alt="Donate with PayPal button"/><img alt="" border="0" src="https://www.paypal.com/en_US/i/scr/pixel.gif" width="1" height="1"/></form>`,
        paypalMessage = `<strong>No ads? No problem!</strong> You can support the Master Nest by <a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=C5CLJ64PC83ES&source=url">donating through PayPal</a>. Thanks for visiting us!`;
    paypalTableCell1.innerHTML = paypalButton;
    paypalTableCell2.innerHTML = paypalMessage;
    paypalTableRow.innerHTML = paypalTableCell1.outerHTML + paypalTableCell2.outerHTML;
    paypalTable.innerHTML = paypalTableRow.outerHTML;
    paypalTable.style.width = "100%";
    paypalContainer.setAttribute("class", "paypalContainer");
    paypalContainer.innerHTML = paypalTable.outerHTML;
    footer.style.marginBottom = 0;
    
    for (let i = 0; i < adContainers.length; i++) {
        adContainers[i].innerHTML = paypalContainer.outerHTML;
    }
}