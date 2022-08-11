# Proyecto-de-calidad-del-sotware-
Proyecto de calidad del software Eclipse java seleniunWebDriver Proyecto de testeo de un pagina sobre una clinica Herramientas Visual Studio 2019 Developer
Microsoft Visual Studio es un entorno de desarrollo integrado para 
Windows, Linux y macOS. Es compatible con múltiples lenguajes de 
programación, tales como C++, C#, Visual Basic.

//Pruebas de testeo del software clinica

La extension de selenium webDriver
[Uploading chromedriver.exe…]()

//Depencias de eclipce con maven
 <properties>
  <maven.compiler.source>1.7</maven.compiler.source>
  <maven.compiler.target>1.7</maven.compiler.target>
  </properties>
  
  <dependencies>
  <dependency>
            <groupId>org.seleniumhq.selenium</groupId>
            <artifactId>selenium-java</artifactId>
            <version>3.141.59</version>
            <scope>test</scope>
        </dependency>

        <dependency>
            <groupId>junit</groupId>
            <artifactId>junit</artifactId>
            <version>4.13.2</version>
            <scope>test</scope>
        </dependency>
  </dependencies>
  
//Comienzo de pruebas
1//    Registro depacientes


        Thread.sleep(2000);
        driver.findElement(registerPacienteLinkLocator).click();
        Thread.sleep(2000);
        WebElement buscar2 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtNroDocumento"));
        buscar2.sendKeys("117990801");
        Thread.sleep(2000);
        WebElement buscar3 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtNombres"));
        buscar3.sendKeys("angelo");
        Thread.sleep(2000);
        WebElement buscar4 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtApPaterno"));
        buscar4.sendKeys("sanchez");
        Thread.sleep(1000);
        WebElement buscar5 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtApMaterno"));
        buscar5.sendKeys("castro");
        Thread.sleep(1000);
        WebElement buscar6 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$ddlSexo"));
        buscar6.click();;
        Thread.sleep(2000);
     
        WebElement buscar8 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtEdad"));
        buscar8.sendKeys("24");
        Thread.sleep(1000);
        WebElement buscar9 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtTelefono"));
        buscar9.sendKeys("8625516232");
        Thread.sleep(1000);
        WebElement buscar10 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtDireccion"));
        buscar10.sendKeys("brasil la flor");
        Thread.sleep(1000);
        WebElement buscar11 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnRegistrar"));
        buscar11.click();
        Thread.sleep(1000);
        
        
        
    }
    @After
    public void turdown() {
        driver.quit();
    }
	
}

//2	Registro medico

@Test
    public void testGooglepage() throws InterruptedException {
        WebElement buscar = driver.findElement(By.name("LoginUser$UserName"));
        buscar.sendKeys("security");
        WebElement buscar1 = driver.findElement(By.name("LoginUser$Password"));
        buscar1.sendKeys("security");
        Thread.sleep(1500);
        WebElement btnbuscar = driver.findElement(By.name("LoginUser$btnIngresar"));
        btnbuscar.click();
        Thread.sleep(1500);
        
        
        driver.findElement(registerLinkLocator).click();
        Thread.sleep(2000);
        driver.findElement(registerMedicosLinkLocator).click();
        Thread.sleep(2000);
        WebElement buscar2 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtNroDocumento"));
        buscar2.sendKeys("11855010");
        Thread.sleep(2000);
        WebElement buscar3 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtNombres"));
        buscar3.sendKeys("david");
        Thread.sleep(2000);
        WebElement buscar4 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtApPaterno"));
        buscar4.sendKeys("soto");
        Thread.sleep(1000);
        WebElement buscar5 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtApMaterno"));
        buscar5.sendKeys("vargas");
        Thread.sleep(1000);
        WebElement buscar11 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnRegistrar"));
        buscar11.click();
        Thread.sleep(1000);
        
        
    }
    @After
    public void turdown() {
        driver.quit();
    }
	
}

// 3 Registro de enfermeras


@Test
    public void testGooglepage() throws InterruptedException {
        WebElement buscar = driver.findElement(By.name("LoginUser$UserName"));
        buscar.sendKeys("security");
        WebElement buscar1 = driver.findElement(By.name("LoginUser$Password"));
        buscar1.sendKeys("security");
        Thread.sleep(1500);
        WebElement btnbuscar = driver.findElement(By.name("LoginUser$btnIngresar"));
        btnbuscar.click();
        Thread.sleep(1500);
        
        driver.findElement(registerLinkLocator).click();

        Thread.sleep(2000);
        driver.findElement(registerEnfermerasLinkLocator).click();
        Thread.sleep(2000);
        WebElement buscar2 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtNroDocumento"));
        buscar2.sendKeys("11514766");
        Thread.sleep(2000);
        WebElement buscar3 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtNombres"));
        buscar3.sendKeys("daniela");
        Thread.sleep(2000);
        WebElement buscar4 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtApPaterno"));
        buscar4.sendKeys("castro");
        Thread.sleep(1000);
        WebElement buscar5 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtApMaterno"));
        buscar5.sendKeys("mora");
        Thread.sleep(1000);
        WebElement buscar11 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnRegistrar"));
        buscar11.click();
        Thread.sleep(1000);
        
        
    }
    @After
    public void turdown() {
        driver.quit();
    }
	
}

// 4 Registro Usuario 


	@Test
    public void testGooglepage() throws InterruptedException {
        WebElement buscar = driver.findElement(By.name("LoginUser$UserName"));
        buscar.sendKeys("security");
        WebElement buscar1 = driver.findElement(By.name("LoginUser$Password"));
        buscar1.sendKeys("security");
        Thread.sleep(1500);
        WebElement btnbuscar = driver.findElement(By.name("LoginUser$btnIngresar"));
        btnbuscar.click();
        Thread.sleep(1500);
        
       
        driver.findElement(registerLinkLocator).click();
        Thread.sleep(2000);
   driver.findElement(registerUsuariosLinkLocator).click();
        Thread.sleep(2000);
        WebElement buscar2 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtDNI"));
        buscar2.sendKeys("11855010");
        Thread.sleep(2000);
        WebElement buscar6 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnBuscar"));
        buscar6.click();
        Thread.sleep(2000);
        WebElement buscar3 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtUsuario"));
        buscar3.sendKeys("david");
        Thread.sleep(2000);
        WebElement buscar4 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtContraseña"));
        buscar4.sendKeys("david3322");
        Thread.sleep(1000);
        WebElement buscar11 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnRegistrar"));
        buscar11.click();
        Thread.sleep(1000);
        
    }
    @After
    public void turdown() {
        driver.quit();
    }
	
}

//Registro citas


  // 5 Registro citas

	@Test
    public void testGooglepage() throws InterruptedException {
        WebElement buscar = driver.findElement(By.name("LoginUser$UserName"));
        buscar.sendKeys("security");
        WebElement buscar1 = driver.findElement(By.name("LoginUser$Password"));
        buscar1.sendKeys("security");
        Thread.sleep(1500);
        WebElement btnbuscar = driver.findElement(By.name("LoginUser$btnIngresar"));
        btnbuscar.click();
        Thread.sleep(1500);
        
       
        driver.findElement(registerReservadeCitasLinkLocator).click();
        Thread.sleep(2000);
        WebElement buscar2 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtDNI"));
        buscar2.sendKeys("11799080");
        Thread.sleep(2000);
        WebElement buscar11 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnBuscar"));
        buscar11.click();
        Thread.sleep(1000);
        WebElement buscar4 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnBuscarHorario"));
        buscar4.click();
        Thread.sleep(1000);
        WebElement buscar5 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$grdHorariosAtencion$ctl02$chkSeleccionar"));
        buscar5.click();
        Thread.sleep(1000);
        WebElement buscar12 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnBuscar"));
        buscar12.click();
        Thread.sleep(1000);
        
        WebElement buscar6 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnReservarCita"));

        buscar6.click();

        Thread.sleep(1000);
        
        
        
    }
    @After
    public void turdown() {
        driver.quit();
    }
	
}


// 6 Atencion acitas 
	@Test
    public void testGooglepage() throws InterruptedException {
        WebElement buscar = driver.findElement(By.name("LoginUser$UserName"));
        buscar.sendKeys("security");
        WebElement buscar1 = driver.findElement(By.name("LoginUser$Password"));
        buscar1.sendKeys("security");
        Thread.sleep(1500);
        WebElement btnbuscar = driver.findElement(By.name("LoginUser$btnIngresar"));
        btnbuscar.click();
        Thread.sleep(1500);   
        driver.findElement(registerAtencióndeCitasLinkLocator).click();
        Thread.sleep(2000);
        WebElement buscar8 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$dlAtencionMedica$ctl00$btnAtencion"));
        buscar8.click();
        Thread.sleep(2000);
        WebElement buscar2 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtDiagnostico"));
        buscar2.sendKeys("Presenta huesos fracturados");
        Thread.sleep(2000);
        WebElement buscar10 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtObservaciones"));
        buscar10.sendKeys("Paracetamol");
        Thread.sleep(2000);
        WebElement buscar11 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnRegistrar"));
        buscar11.click();
        Thread.sleep(1000);
        
    }
    
    
    
    @After
    public void turdown() {
        driver.quit();
    }
	
}

// 7 HORARIO MEDICOS



By HoraiosLinkLocator = By.linkText("Horarios");
	By registerHorariosMedicosLinkLocator = By.linkText("Horarios Medicos");
	By registerAgregarHorarioLinkLocator = By.linkText("Agregar Horario");
	


WebElement buscar = driver.findElement(By.name("LoginUser$UserName"));

		buscar.sendKeys("security");
		
		WebElement buscar1 = driver.findElement(By.name("LoginUser$Password"));
		
		buscar1.sendKeys("security");

		Thread.sleep(1500);
		
		WebElement btnbuscar = driver.findElement(By.name("LoginUser$btnIngresar"));
		
		btnbuscar.click();
		
		Thread.sleep(1500);
		


		driver.findElement(HoraiosLinkLocator).click();

		Thread.sleep(2000);
		
		driver.findElement(registerHorariosMedicosLinkLocator).click();
		Thread.sleep(2000);
		
		
		Thread.sleep(2000);
		
		WebElement buscar2 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtDNI"));

		buscar2.sendKeys("11799080");
		
		Thread.sleep(2000);
		
		WebElement buscar11 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnBuscar"));

		buscar11.click();
		
		Thread.sleep(1000);
		
		driver.findElement(registerAgregarHorarioLinkLocator).click();

		Thread.sleep(2000);
		WebElement buscar6 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtFecha"));

		buscar6.sendKeys("1272020");
		Thread.sleep(2000);
		
		WebElement buscar8 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtHoraInicio"));
		buscar8.clear();
		
		Thread.sleep(2000);
		
		buscar8.sendKeys("10:00");
		Thread.sleep(2000);
		
		WebElement buscar13 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnAgregar"));

		buscar13.click();






// 8 Horario Enfermeras

driver.findElement(HoraiosLinkLocator).click();

		Thread.sleep(2000);
		
		driver.findElement(registerHorariosEnfermerasLinkLocator).click();
		Thread.sleep(2000);
WebElement buscar2 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtDNI"));

		buscar2.sendKeys("11799080");
		
		Thread.sleep(2000);

WebElement buscar14 = driver.findElement(By.name("agregarhorario"));

		buscar14.click();
WebElement buscar6 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$txtFecha"));

		buscar6.sendKeys("1272020");
		Thread.sleep(2000);

WebElement buscar13 = driver.findElement(By.name("ctl00$ContentPlaceHolder1$btnAgregar"));

		buscar13.click();


