function Gmaildata() {

  var ss = SpreadsheetApp.getActiveSheet();
 // var sheet = ss.getSheets()[0];

  var label = GmailApp.getUserLabelByName("Tradingview Alerts");
  var threads = label.getThreads();

  for (var i=0; i<threads.length; i++)
  {
var messages = threads[i].getMessages();

for (var j=0; j<messages.length; j++)
{
  var msg = messages[j].getBody().replace(/<.*?>/g, '\n').replace(/^\s*\n/gm, '').replace(/^\s*/gm, '').replace(/\s*\n/gm, '\n');
  var sub = messages[j].getSubject();
  var dat = messages[j].getDate();

  sheet.appendRow([dat, msg])
}
  threads[i].removeLabel(label);
  }
}



function splitColumn() {
  
   var ss = SpreadsheetApp.getActiveSpreadsheet();
  // ss is now the spreadsheet the script is associated with
  var sheet = ss.getSheets()[0];
  var sheet2 =  ss.getSheets()[1];
  
  var active_range = sheet.getActiveRange();
  
  var lastRow = sheet.getLastRow();
  var lastRow2 = sheet2.getLastRow();
var lastColumn = sheet.getLastColumn();
var lastCell = sheet.getRange(lastRow, lastColumn);
Logger.log(lastCell.getValue());
  
var bullspowerln = 0;
var bearspowerln =0;
var trendpower =0;
var rangepower =0;

var bullspowersh = 0;
var bearspowersh =0;

  
  
  Logger.log(sheet.getMaxRows());
  
  for(var i = 2; i <= lastRow; i++){
    
	 var col2 = sheet.getRange(i, 2).getValue();
	 var updatedText = col2.toString()
     var splitMyText = updatedText.split(",")
     
	 sheet.getRange(i, 3).setValue(splitMyText[0]);
	 sheet.getRange(i, 4).setValue(splitMyText[1]);
	 sheet.getRange(i, 5).setValue(splitMyText[2]);
	 sheet.getRange(i, 6).setValue(splitMyText[3]);
	 sheet.getRange(i, 7).setValue(splitMyText[4]);
	 sheet.getRange(i, 8).setValue(splitMyText[5]);
	 sheet.getRange(i, 9).setValue(splitMyText[6]);
    
     
     var vol = sheet.getRange(i, 9).getValue();
    var vol1 = Number(vol);
    var vol2 = vol1/100
    sheet.getRange(i, 10).setValue(vol2);

    sheet.getRange(i, 11).setValue(1);
    sheet.getRange(i, 12).setValue(1);
    sheet.getRange(i, 13).setValue(1);
    sheet.getRange(i, 14).setValue(1);
    sheet.getRange(i, 15).setValue(1);
    sheet.getRange(i, 16).setValue(0);
    sheet.getRange(i, 17).setValue(0);
    sheet.getRange(i, 18).setValue(0);
    sheet.getRange(i, 19).setValue(0);
    sheet.getRange(i, 20).setValue(0); 
    sheet.getRange(i, 21).setValue(0); 
    sheet.getRange(i, 22).setValue(0); 
    sheet.getRange(i, 23).setValue(0); 
    
  }
  
     
    var col1 =new Date( sheet.getRange(lastRow, 1).getValue());
    var col1inms = col1.getTime();
    var subhr = 2 * 60 * 60 * 1000; // 43200000 = 12 hours in milliseconds
    var subday= 3 * 24 * 60 * 60 * 1000;
    
    var twohoursearly = col1inms - subhr;
    var threedaysearly = col1inms - subday;
    
    var newtime = new Date(twohoursearly);
    var newdate = new Date(threedaysearly); 
  
  // sheet.getRange(2, 20).setValue(newtime);
  // sheet.getRange(2, 21).setValue(newdate);
  
 
  for(var i = lastRow ; i>=2; i--){
    
    var col1data = new Date (sheet.getRange(i, 1).getValue());
     
    if(col1data < newdate)
    sheet.deleteRow(i); 
    
  }
    
  
  
for(var i = lastRow ; i>=2; i--){
  
  var j= i-1;
  var volcalnew = sheet.getRange(i, 10).getValue();
  var volcallast = sheet.getRange(j, 10).getValue();
  if(i==2)
    volcallast=0;
  var volcalupdate = volcalnew - volcallast
  sheet.getRange(i, 11).setValue(volcalupdate);
  
}
  
  for(var i = lastRow ; i>=2; i--){
    
    var instrument = sheet.getRange(i, 3).getValue();
    if(instrument = "XBTUSD"){
    
    var timeframe = sheet.getRange(i, 4).getValue();
    var indicator = sheet.getRange(i, 5).getValue();
    var properties = sheet.getRange(i, 6).getValue();
    var signal = sheet.getRange(i, 7).getValue();
    var price = sheet.getRange(i, 8).getValue();
    var volper = sheet.getRange(i, 10).getValue();
    
    
    for(var j = lastRow2 ; j>=1; j--){
      
       var timeframe2 = sheet2.getRange(j, 1).getValue();  
       var indicator2 = sheet2.getRange(j, 3).getValue();
       var properties2 = sheet2.getRange(j, 5).getValue();
       var signal2 = sheet2.getRange(j, 7).getValue();  
           
       var timeframepriority = sheet2.getRange(j, 2).getValue();  
       var indicatorpriority = sheet2.getRange(j, 4).getValue();
       var propertiespriority = sheet2.getRange(j, 6).getValue();
       var signalpriority = sheet2.getRange(j, 8).getValue(); 
        
    if(timeframe == timeframe2)
       sheet.getRange(i, 12).setValue(timeframepriority);
    if(indicator==indicator2)
       sheet.getRange(i, 13).setValue(indicatorpriority);
    if(properties==properties2)
       sheet.getRange(i, 14).setValue(propertiespriority);
    if(signal==signal2)
       sheet.getRange(i, 15).setValue(signalpriority);
      
    }
      
   var timeframescore = sheet.getRange(i, 12).getValue();
   var indicatorscore = sheet.getRange(i, 13).getValue();
   var propertiesscore = sheet.getRange(i, 14).getValue();
   var signalscore = sheet.getRange(i, 15).getValue();
   var volumeper = sheet.getRange(i, 10).getValue();
         
   var score = timeframescore * indicatorscore *  propertiesscore * signalscore * volumeper ;  
      if(propertiesscore < 0){
        if(signalscore < 0){        
          var score = score * -1
        }
      }
    
      if(score>0){
        var bullscore = score;
        sheet.getRange(i, 16).setValue(bullscore);
      }
      if(score<0){
        var bearscore =score;
        sheet.getRange(i, 17).setValue(bearscore);
      }
      
      var volcalc = sheet.getRange(i, 11).getValue();
      if(volcalc >0)
        sheet.getRange(i, 18).setValue(volcalc);
      if(volcalc<0)
        sheet.getRange(i, 19).setValue(volcalc);
    }
    
    else if(instrument == "BVOL" || "BVOLUSD"){

      var prices = sheet.getRange(i, 8).getValue();
      sheet.getRange(i, 24).setValue(prices);
      
      for(var i = lastRow ; i>=2; i--){
        var j= i-1;
        var bpricenew = sheet.getRange(i, 24).getValue();
        var bpricelast = sheet.getRange(j, 24).getValue();
        if(i==2)
          bpricelast=0;
        var bpriceupdate = bpricenew - bpricelast
        //sheet.getRange(i, 11).setValue(volcalupdate);
   
      
    // var bprice = sheet.getRange(i, 8).getValue();
      if(bpriceupdate >0)
     sheet.getRange(i, 18).setValue(bpriceupdate);
      if(bpriceupdate <0 )
       sheet.getRange(i, 19).setValue(bpriceupdate);
  
      
    }
    }    
    
  }
  
 for(var i = lastRow ; i>=2; i--){
    
      var timefr = sheet.getRange(i, 4).getValue();
      var bullscore = sheet.getRange(i, 16).getValue();
      var bearscore = sheet.getRange(i, 17).getValue();
      var col2data = new Date (sheet.getRange(i, 1).getValue());
   

   if ( timefr < 60){
        sheet.getRange(i, 20).setValue(bullscore);
        sheet.getRange(i, 21).setValue(bearscore);
   }
   
    if ( timefr > 60){
        sheet.getRange(i, 22).setValue(bullscore);
        sheet.getRange(i, 23).setValue(bearscore);
   }
   
   
   if ( col2data > newtime ){
     
     var bullspowerln = bullspowerln + sheet.getRange(i, 22).getValue();
     var bearspowerln =bearspowerln + sheet.getRange(i, 23).getValue();
    
     var trendpower = trendpower + sheet.getRange(i, 18).getValue();
     var rangepower = rangepower +  sheet.getRange(i, 19).getValue();

     var bullspowersh = bullspowersh + sheet.getRange(i, 20).getValue();
     var bearspowersh = bearspowersh + sheet.getRange(i, 21).getValue();
     
     
   } 
 }
   
  bearspowerln =bearspowerln * -1;
  bearspowersh = bearspowersh * -1;
  rangepower = rangepower * -1;
  
  var bullmomentum = bullspowersh / (bullspowersh + bearspowersh);
  var bearmomentum = bearspowersh / (bullspowersh + bearspowersh);
  
  var bulltrend = bullspowerln / (bullspowerln + bearspowerln );
  var beartrend = bearspowerln / (bullspowerln + bearspowerln );
  
  var trending = trendpower / (trendpower + rangepower);
  var ranging = rangepower / (trendpower + rangepower);
  
  sheet2.getRange(2, 11).setValue(bullmomentum);
  sheet2.getRange(2, 12).setValue(bearmomentum);
  sheet2.getRange(3, 11).setValue(bulltrend);
  sheet2.getRange(3, 12).setValue(beartrend);
  sheet2.getRange(5, 11).setValue(trending);
  sheet2.getRange(5, 12).setValue(ranging);
  
  if( bullmomentum > bearmomentum)
  { sheet2.getRange(2, 14).setValue("Bullish Momentum");
   if( bullmomentum > 0.75)
     sheet2.getRange(2, 13).setValue("Strong");
  }
  else{
    sheet2.getRange(2, 14).setValue("Bearish Momentum");
    if(bearmomentum > 0.75)
      sheet2.getRange(2, 13).setValue("Strong");
  }
  if( bulltrend > beartrend){
    sheet2.getRange(3, 14).setValue("Bullish Trend");
  if(bulltrend > 0.75 )
    sheet2.getRange(3, 13).setValue("Strong");
  }
    else{ 
    sheet2.getRange(3, 14).setValue("Bearish Trend");
      if(beartrend > 0.75)
        sheet2.getRange(3, 13).setValue("Strong");
  }
  
  if( trending > ranging){
    sheet2.getRange(5, 14).setValue("Trending");
    if(trending > 0.75)
      sheet2.getRange(5, 13).setValue("Strong");
  }
  else{
    sheet2.getRange(5, 14).setValue("Flat");
    if(ranging > 0.75)
    sheet2.getRange(5, 14).setValue("Strong");
  }
  
  for(i=5;i>=2;i--)
  { 
    if( sheet2.getRange(i, 13).getValue() == "Strong")
    {   var display =  sheet2.getRange(i, 15).getValue();
        sheet2.getRange(i, 16).setValue(display);
    }
  }
   

}
   