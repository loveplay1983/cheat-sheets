## Event Listenser
- 调试listenser

		$ php bin/console debug:container session

		Information for Service "session"
		=================================
		
		 ------------------ --------------------------------------------------
		  Option             Value
		 ------------------ --------------------------------------------------
		  Service ID         session
		  Class              Symfony\Component\HttpFoundation\Session\Session
		  Tags               -
		  Public             yes
		  Synthetic          no
		  Lazy               no
		  Shared             yes
		  Abstract           no
		  Autowired          no
		  Autowiring Types   -
		 ------------------ --------------------------------------------------
- [Login Listener](LoginListener.md) 登录的事件监听
- [Enable Filter Listener](EnableFilterListener.md) 开启过滤器监听
- [Guzzle Listener](GuzzleListener.md) GuzzleHttp请求相关监听
- [API version](ApiVersion.md) API版本控制监听
- [kernel view](kernel.view.md) 模板层监听
