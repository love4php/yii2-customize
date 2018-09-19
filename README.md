"# yii2-customize" 

Mysql Schema : 
return [
    'class' => 'yii\db\Connection',
    'dsn' => 'pgsql:host=localhost;dbname=db_name', 
    'username' => 'db_username',
    'password' => 'db_password',
    'charset' => 'utf8',
    'schemaMap' => [
      'pgsql'=> [
        'class'=>'love4php\yii2_customize\db\mysql\Schema',
        'defaultSchema' => 'public' //specify your schema here
      ]
    ], // PostgreSQL
];
