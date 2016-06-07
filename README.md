# calendar-booking-PHP

$calendarModel = new Calendar\CalendarModel();

PHP:
  echo $calendar= $calendarModel->show();

TWIG : 
    {{ calendar|raw }}

for silex: 

 $calendarModel = new Calendar\CalendarModel();
 $calendar= $calendarModel->show();

  return $app['twig']->render('YourDirectory/YourPage.twig', array('calendar' => $calendar));
