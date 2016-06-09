# calendar-booking-PHP

$calendarModel = new Calendar\CalendarModel();

PHP:
  echo $calendar= $calendarModel->show();

TWIG : 
    {{ calendar|raw }}

for silex: 

 $calendarModel = new Calendar\CalendarModel();
 $calendar= $calendarModel->show($dayToRemove, $numbreOfDayToRemove,$monthToRemove);
 
    private $numbreOfDayToRemove = []; // ['14-6-2016',...] //optionnel
    private $dayToRemove = []; //['Lundi','Mardi','Mercredi','Jeudi','Vendredi','Samedi','Dimanche'] //optionnel
    private $monthToRemove = []; //['01','02','03','04',..] //optionnel
    
    
    I'm currently doing that for now there is juste an echo of it

  return $app['twig']->render('YourDirectory/YourPage.twig', array('calendar' => $calendar));
  
  PS : 
  
  is set in french _createNavi() line 250
