# Spring-Boot-DI  
Demostración de **Inyección de Dependencias** con Spring Boot en 5 minutos

## 🚀 ¿Qué aprenderás aquí?
- Cómo Spring Boot administra tus beans automáticamente.  
- Diferencias entre `@Component`, `@Service`, `@Repository` y `@Controller`.  
- Inyección por constructor (recomendada) y por campo.  
- Hot-reload con DevTools para ver los cambios sin reiniciar.

## 📦 Stack
| Tecnología | Versión |
|------------|---------|
| Spring Boot | 2.1.3 |
| Java | 11 |
| Thymeleaf | (vista rápida) |
| Maven | 3.x+ |

## ▶️ Arranque rápido
```bash
git clone https://github.com/AliciaJava/spring-boot-di.git
cd spring-boot-di
mvn spring-boot:run
```
Visita [http://localhost:8080](http://localhost:8080) y observa cómo se inyectan los componentes.

## 📁 Estructura clave
```
src/main/java/com.bolsadeideas.springboot.di
├── SpringBootDiApplication.java   # @SpringBootApplication
├── controller
│   └── IndexController.java       # @Controller + inyección por constructor
├── service
│   └── MiServicio.java            # @Service (lógica de negocio)
└── repository
    └── MiRepository.java          # @Repository (acceso a datos fake)
```
Todos los beans se registran y se inyectan **sin XML**.

## 🔧 Hot-reload
1. Arranca con `mvn spring-boot:run`.  
2. Edita cualquier clase anotada con `@Component`.  
3. Actualiza el navegador → **cambios aplicados al instante**.

## ✅ Prueba rápida
```bash
mvn test
```
Verifica que los contextos de Spring se levantan y los beans se inyectan correctamente.

## 📚 Recursos
- [Spring DI Official Guide](https://spring.io/guides/gs/injecting-dependencies)  
- [Spring Boot Reference](https://docs.spring.io/spring-boot/docs/2.1.3.RELEASE/reference/htmlsingle/)

**¿Dudas?** Ábrete un issue o únete a la comunidad en Telegram.  
Si el repo te sirve, **dale una ⭐** y compártelo.
