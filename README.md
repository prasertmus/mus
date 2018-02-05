<?php

require_once './vendor/autoload.php';

$token = '02LpztAggKB3ktzOLz27BkXh85YvpRN8ZFXudJ79wTh';
$ln = new KS\Line\LineNotify($token);

$text = ' '; // Line Notify บังคับให้ใส่ข้อความ แต่อยากส่งแแต่รูปภาพเลยใส่ space ไว้
$image_path = '/tmp/test_line.jpg'; //Line notify allow only jpeg and png file
$ln->send($text, $image_path);
