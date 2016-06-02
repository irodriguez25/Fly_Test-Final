#_Fly_Test-Final
public_class_FlyTest_{
	public_static_void_main(String[]_args){
		Flyer_Bird_=_new_Flyer_(10,_3);
		Flyer_Airplane_=_new_Flyer_(450,_50);
		Flyer_JetPlane_=_new_Flyer_(1000,_120);
		Flyer_Missile_=_new_Flyer_(2500,_800);
		Flyer_Superman_=_new_Flyer_(3500,_500);
			
		Runnable_BirdThread_=_new_FlyThread_(Bird);
		Runnable_AirplaneThread_=_new_FlyThread_(Airplane);
		Runnable_JetPlaneThread_=_new_FlyThread_(JetPlane);
		Runnable_MissileThread_=_new_FlyThread_(Missile);
		Runnable_SupermanThread_=_new_FlyThread_(Superman);
		
		Thread_BirdWorker_=_new_Thread_(BirdThread);
		Thread_AirplaneWorker_=_new_Thread_(AirplaneThread);
		Thread_JetPlaneWorker_=_new_Thread_(JetPlaneThread);
		Thread_MissileWorker_=_new_Thread_(MissileThread);
		Thread_SupermanWorker_=_new_Thread_(SupermanThread);
		
		BirdWorker.setName_("Bird");
		AirplaneWorker.setName_("Airplane");
		JetPlaneWorker.setName_("JetPlane");
		MissileWorker.setName_("Missile");
		SupermanWorker.setName_("Superman");
		
		BirdWorker.start();
		AirplaneWorker.start();
		JetPlaneWorker.start();
		MissileWorker.start();
		SupermanWorker.start();
		
	}
}
