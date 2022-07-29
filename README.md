# telaCriarPerfil
Uma tela criada em react-native js

import React,{useState} from 'react';
import { Text, View, StyleSheet, TextInput, TouchableOpacity } from 'react-native';


export default function App() {
  const [alignSelf, setAlignSelf] = useState("stretch");

  return (
    <View style={styles.container}>
        <View>
          <Text style={styles.textheader}>
            Criar Perfil
        </Text>
       </View>
       <View>
          <View style={styles.pessoal}>
            <TextInput
              style={styles.inputs}
              placeholder="Nome Completo"
              keyboardType="text"
            />
            <TextInput
              style={styles.inputs}
              placeholder="telefone"
              keyboardType="text"
              />
              <TextInput
              style={styles.inputs}
              placeholder="email"
              keyboardType="text"
              />
              <TextInput
              style={styles.inputs}
              placeholder="linkedin"
              keyboardType="text"
              />
              <TextInput
              style={styles.inputs}
              placeholder="git hub"
              keyboardType="text"
              />
          </View>
          
          <View style={styles.caixaEndereco}>
              <Text style={styles.textcaixas}>Endereco</Text>
              <TextInput
              style={styles.inputs}
              placeholder="Logradouro"
              keyboardType="text"
              />
              <TextInput
              style={styles.inputs}
              placeholder="Bairro"
              keyboardType="text"
              />
               <Text>Numero</Text>
              <TextInput
              style={styles.inputNumero}
              keyboardType="text"
              />
              <TextInput
              style={styles.inputCidade}
              placeholder="Cidade"
              keyboardType="text"

              />
              <TextInput
              style={styles.inputEstado}
              placeholder="Estado"
              keyboardType="text"

              />
          </View>
          <View style={styles.caixaformacao}>
              <Text style={styles.textcaixas}>Formações</Text>
              <TextInput
              style={styles.inputs}
              placeholder="ex: Ensino Medio, bacharelado em Direito"
              keyboardType="text"
              />
              <TouchableOpacity
                  style={styles.btnAdiocionar}
              ><Text style={{color:"white"}}>Adicionar +</Text></TouchableOpacity>
              <TextInput
              style={styles.cursoAdicionados}
              multiline
              numberOfLines={4}
              keyboardType="text"
              />
              
          </View>
          <View style={styles.caixaCursos}>
              <Text style={styles.textcaixas}>Cursos</Text>
              <TextInput
              style={styles.inputs}
              placeholder="Cursos"
              keyboardType="text"
              />
              <TouchableOpacity
                  style={styles.btnAdiocionar}
              ><Text style={{color:"white"}}>Adicionar +</Text></TouchableOpacity>
              <TextInput
              style={styles.cursoAdicionados}
              multiline
              numberOfLines={4}
              keyboardType="text"
              />
              
          </View>
          <View style={styles.experiencias}>
              <Text style={styles.textcaixas}>Experiencias</Text>
              <TextInput
              style={styles.inputs}
              placeholder="Empresa"
              keyboardType="text"
              />
              <TextInput
              style={styles.inputs}
              placeholder="Cargo"
              keyboardType="text"
              />
              <TextInput
              style={styles.inputs}
              placeholder="Data de inicio"
              keyboardType="text"
              />
              <TextInput
              style={styles.inputs}
              placeholder="Data de Saida"
              keyboardType="text"
              />
              <TouchableOpacity
                  style={styles.btnAdiocionar}
              ><Text style={{color:"white"}}>Adicionar +</Text></TouchableOpacity>
              <TextInput
              style={styles.cursoAdicionados}
              multiline
              numberOfLines={4}
              keyboardType="text"
              />
              
          </View>
          <View style={styles.objetivos}>
              <Text style={styles.textcaixas}>Objetivos</Text>
              
              <TextInput
              style={styles.cursoAdicionados}
              multiline
              numberOfLines={4}
              keyboardType="text"
              />
              
          </View>
          
          
       </View>
       <TouchableOpacity
            style={styles.btnCriar}
          > <Text style={{color:"white",textAlign:"center",fontWeight:"bold",marginTop:3}}>Criar</Text>
          </TouchableOpacity>
     
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#ecf0f1',
    alignItems:"center"
  },
  pessoal:{
    margin:5,
    textAlign:"center",
    alignItems: "center"
  },
  textheader: {
    margin: 24,
    fontSize: 18,
    fontWeight: 'bold',
    textAlign: 'center',
  },
  inputs:{
    margin:5,
    borderWidth: 1,
    height:22,
    width:300,
    paddingLeft:10,
    fontSize:12
  },
  inputNumero:{
    borderWidth: 1,
    height:22,
    width:30,
    textAlign:"center"
    
  },
  caixaEndereco:{
    margin:5,
    textAlign:"center",
    alignItems: "center",
    
  },
  caixaformacao:{
    margin:5,
    textAlign:"center",
    alignItems: "center"
  },
  caixaCursos:{
    margin:5,
    textAlign:"center",
    alignItems: "center"
  },
  textcaixas:{
    textAlign:"center",
    fontWeight:"bold",
  },
  btnAdiocionar:{
    margin:5,
    height:20,
    width:80,
    backgroundColor:"green",
    borderRadius:3
  },
  cursoAdicionados:{
    height:150,
    width:300,
    borderWidth:1,
  },
  inputCidade:{
    margin:10,
    borderWidth: 1,
    height:20,
    width:70,
    paddingLeft:10,
    fontSize:12
  },
  inputEstado:{
    margin:10,
    borderWidth: 1,
    height:22,
    width:70,
    paddingLeft:10,
    fontSize:12
  },
  experiencias:{
    margin:5,
    textAlign:"center",
    alignItems: "center"
  },
  btnCriar:{
    height:30,
    width:150,
    backgroundColor:"green",
    margin:30,
    borderWidth:2,
    borderRadius:3
  },
  objetivos:{
    margin:5,
    textAlign:"center",
    alignItems: "center"
  }

});
