<?php

header("Access-Control-Allow-Origin: *");
header('Access-Control-Allow-Credentials: true');
header('Access-Control-Allow-Methods: PUT, GET, POST, DELETE, OPTIONS');
header("Access-Control-Allow-Headers: X-Requested-With");
header('Content-Type: text/html; charset=utf-8');
header('P3P: CP="IDC DSP COR CURa ADMa OUR IND PHY ONL COM STA"');

include_once '../include/Config.php';

require '../libs/Slim/Slim/Slim.php';
\Slim\Slim::registerAutoloader();
$app = new \Slim\Slim();


$app->setName('Calendar 2019-2020');
$name = $app->getName();

        $app->get('/:id/:year/:month', function ($id,$year, $month) {

                $id0=606;
                $url="";
            switch($id)
            {
                case 122: $id0=606;
                break;
                case 123: $id0=611;
                break;
                case 124: $id0=616;
                break;
                case 125: $id0=621;
                break;
                case 126: $id0=626;
                break;
                case 127:$id0=631;
                break;
                case 128:$id0=636;
                break;
                case 129:$id0=641;
                break;
                case 130:$id0=646;
                break;
                case 131:$id0=651;
                break;
                case 132:$id0=656;
                break;
                case 133:$id0=661;
                break;
                case 134:$id0=666;
                break;
                case 135:$id0=671;
                break;
                case 136:$id0=676;
                break;
                case 137:$id0=681;
                break;
                case 138:$id0=686;
                break;
                default: echo "Does not exit the id of Route!!";
                break;
            }

            if($year<2019 || $year >2020 )
            {
                echo "The Year is out of range! , try with 2019 and 2020";
            }
            else
            {
                if ( $month < 1 || $month > 12)
                {
                   echo "Month out of Range !";
                }
                else
                {
                    //$url = 'https://disponibilidad.net.pe/cal/'.$id.'/'.$id0.'/data?'.$month.'=10&year='.$year.'&h=undefined';

                    $url = 'https://disponibilidad.net.pe/cal/'.$id.'/'.$id0.'/data?month='.$month.'&year='.$year.'&h=undefined';

                    $json = file_get_contents($url);
                    echo $json;
                }
            }
        });



/* corremos la aplicación */
$app->run();

/*********************** USEFULL FUNCTIONS **************************************/

    /**
    * Verificando los parametros requeridos en el metodo o endpoint
    */
    function verifyRequiredParams($required_fields) {
      $error = false;
      $error_fields = "";
      $request_params = array();
      $request_params = $_REQUEST;
      // Handling PUT request params
      if ($_SERVER['REQUEST_METHOD'] == 'PUT') {
      $app = \Slim\Slim::getInstance();
      parse_str($app->request()->getBody(), $request_params);
      }
      foreach ($required_fields as $field) {
      if (!isset($request_params[$field]) || strlen(trim($request_params[$field])) <= 0) {
      $error = true;
      $error_fields .= $field . ', ';
      }
    }

    if ($error) {

    $response = array();
    $app = \Slim\Slim::getInstance();
    $response["error"] = true;
    $response["message"] = 'Required field(s) ' . substr($error_fields, 0, -2) . ' is missing or empty';
    echoResponse(400, $response);

    $app->stop();
    }
    }



/**
* Mostrando la respuesta en formato json al cliente o navegador
* @param String $status_code Http response code
* @param Int $response Json response
*/
function echoResponse($status_code, $response) {
$app = \Slim\Slim::getInstance();
// Http response code
$app->status($status_code);

// setting response content type to json
$app->contentType('application/json');

echo json_encode($response);
}

/**
* Agregando un leyer intermedio e autenticación para uno o todos los metodos, usar segun necesidad
* Revisa si la consulta contiene un Header "Authorization" para validar
*/
function authenticate(\Slim\Route $route) {
// Getting request headers
$headers = apache_request_headers();
$response = array();
$app = \Slim\Slim::getInstance();

// Verifying Authorization Header
if (isset($headers['Authorization'])) {
//$db = new DbHandler(); //utilizar para manejar autenticacion contra base de datos

// get the api key
$token = $headers['Authorization'];

// validating api key
if (!($token == API_KEY)) { //API_KEY declarada en Config.php

// api key is not present in users table
$response["error"] = true;
$response["message"] = "Acceso denegado. Token inválido";
echoResponse(401, $response);

$app->stop(); //Detenemos la ejecución del programa al no validar

} else {
//procede utilizar el recurso o metodo del llamado
}
} else {
// api key is missing in header
$response["error"] = true;
$response["message"] = "Falta token de autorización";
echoResponse(400, $response);

$app->stop();
}
}
?>
