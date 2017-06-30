# test
测试文档
<?php 
namespace Home\Controller;
use Think\Controller;
class JobController extends Controller {
	public function job(){
		//创建对象
		// echo "<meta http-equiv='Content-Type'' content='text/html; charset=utf-8'>";
		$Job = M("Job"); 
	    $Jobs=$Job->select(); 

		//变量解析
		$this->assign('jobs',$Jobs);
		//解析模板
		$this->display();
	}

	



 }
?>
