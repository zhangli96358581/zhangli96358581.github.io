---
title: Spring boot 注解
date: 2022-02-18 02:48:08
tags: Sprin
---

@SpringBootAppliction: 标注这个类是一个springboot的应用

注解

- ```
  @SpringBootConfiguration :springboot的配置
  	Configuration:spring配置类
  	@Compoent：说明这也是一个spring的组件
  
  @EnableAutoConfiguration :自动配置 
  	@AutoConfigurationPackage：自动配置包
  		@Import（AutoCounfigurationPackages.Registrar.class）自动配置`包注册`
  	@Import（AutoCounfigurationImportSelector.class）自动配置导入选择
  ```

  

