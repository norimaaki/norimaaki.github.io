<?php

// ファイルの指定
$dataFile = 'datafile.dat';

//エスケープする関数
function h($s){
return htmlspecialchars($s,ENT_QUOTES,'UTF-8');
}

//name="send_message"のPOST送信があった時
if(isset($_POST["send_message"])){
    //送信されたname="message"とname="user_name"の値を取得する
    $message = trim($_POST['message']);
    $user = trim($_POST['user_name']);

    //messageが空じゃなかったら
    if(!empty($message)){

        //userが空の場合、名無しにする
        if(empty($user)){
          $user = "名無し";
        }
        //日付を取得する
        $postDate = date('Y-m-d H:i:s');
        //ファイルに書き込むメッセージを作成する
        $newData  = $message." / ".$user." / ".$postDate."\n";
        //ファイルを開く
        $fp = fopen($dataFile,'a');
        //ファイルに書き込む
        fwrite($fp,$newData);
        //ファイルを閉じる
        fclose($fp);
    }
}
//一行ずつデータを取り出して配列に入れる
$post_list = file($dataFile,FILE_IGNORE_NEW_LINES);
//逆順に並べ替える
$post_list = array_reverse($post_list);
?>
<!DOCTYPE html>
<html>
<head lang="ja">
<meta charset="utf-8">
<title>PHP簡易掲示板</title>
</head>
<body>
<h1>PHP簡易掲示板</h1>

<!--ここで投稿内容を送信する-->
<form action="" method="post">
    メッセージ:<input type="text" name="message">
    ユーザー名:<input type="text" name="user_name">
    <input type="submit" name="send_message" value="投稿">
</form>

<h2>投稿一覧</h2>
<ul>
<!--post_listがある場合-->
<?php if (!empty($post_list)){ ?>
    <!--post_listの中身をひとつづつ取り出し表示する-->
    <?php foreach ($post_list as $post){ ?>
    <li><?php echo h($post); ?></li>
    <?php } ?>
<?php }else { ?>
    <li>まだ投稿はありません。</li>
<?php } ?>
</ul>
</body>
</html>
