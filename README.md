# elvis.vhr

2019-8-6日
main方法可以启动，放到tomcat下不能运行，没有报错，很奇怪，请教同学，
告知：
在tomcat里启动是需要配置一下的，需要实现SpringBootServletInitializer

public class HrserverApplication extends SpringBootServletInitializer {

	@Override
	protected SpringApplicationBuilder configure(SpringApplicationBuilder application) {
		return application.sources(HrserverApplication.class);
	}

	public static void main(String[] args) {
		SpringApplication.run(HrserverApplication.class, args);
	}
}

记录一下！
