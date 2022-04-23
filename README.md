# JarVersionChanger ou Trocador de versão de jar
Uma ferramenta cli _(linha de comando)_ para alterar a versão do arquivo jar .**Observe que esta ferramenta altera apenas o byte relacionado à versão e não altera nenhuma outra parte do arquivo de classe . Esta ferramenta não suporta nenhum bytecode.** Esta ferramenta é praticamente inútil, exceto em algumas raras ocasiões, como se você quiser executar um arquivo jar ___java 11___ e tiver o ___JRE 8___ (isso funcionaria na maioria dos casos, pois a maioria dos os recursos da linguagem são implementados no nível do compilador java. Se ele usar pacotes introduzidos no java 8+, **não funcionará**.).

### Como Usar
```
java -jar jar_version_changer-all.jar path_of_jar -major 52
```

### Compilação e uso
```
cd path_of_project
./gradlew shadowJar 
java -jar  app/build/libs/app-all.jar some_jar_file.jar --major  52
```
