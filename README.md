# site-psicologia
desenvolvimento de um site para atendimento psicológico
import React from "react";
import { FaWhatsapp, FaInstagram, FaUserMd, FaComments, FaBookOpen } from "react-icons/fa";

const Home = () => {
  return (
    <div className="min-h-screen bg-gradient-to-r from-blue-100 to-blue-300 flex flex-col items-center justify-center text-center p-6">
      <div className="bg-white shadow-xl rounded-3xl p-10 max-w-lg text-gray-700">
        <h1 className="text-4xl font-extrabold text-blue-800">Renata Ruiz</h1>
        <p className="text-lg font-medium mt-2">🧠 Psicóloga Clínica</p>
        <p className="text-md text-gray-600 font-semibold">CRP: 06/211363</p>
        <p className="text-md mt-4 leading-relaxed">
          Ajudo você a fortalecer sua identidade e buscar seu propósito por meio do autodesenvolvimento.
        </p>
        <p className="text-md mt-4 leading-relaxed">
          Bem-vindo ao espaço de acolhimento psicológico. Cuide da sua saúde mental com um atendimento profissional e humanizado.
        </p>
        <div className="mt-6 flex justify-center space-x-4">
          <a
            href="https://wa.me/5599999999999"
            target="_blank"
            rel="noopener noreferrer"
            className="inline-flex items-center px-6 py-3 bg-green-500 text-white font-bold rounded-full shadow-lg hover:bg-green-600 transition-all text-lg"
          >
            <FaWhatsapp className="mr-2 text-xl" /> Agende sua consulta
          </a>
          <a
            href="https://www.instagram.com/renataruizpsicologa/"
            target="_blank"
            rel="noopener noreferrer"
            className="inline-flex items-center px-6 py-3 bg-pink-500 text-white font-bold rounded-full shadow-lg hover:bg-pink-600 transition-all text-lg"
          >
            <FaInstagram className="mr-2 text-xl" /> Instagram
          </a>
        </div>
      </div>
    </div>
  );
};

const Services = () => {
  return (
    <div className="min-h-screen bg-white flex flex-col items-center text-center p-10">
      <h2 className="text-3xl font-bold text-blue-800">Serviços</h2>
      <div className="mt-6 grid gap-6 sm:grid-cols-2 lg:grid-cols-3">
        <div className="p-6 bg-blue-100 rounded-xl shadow-md">
          <FaUserMd className="text-3xl text-blue-700 mb-2" />
          <h3 className="text-xl font-semibold">Atendimento Clínico</h3>
          <p className="text-sm text-gray-600">Sessões individuais para promover o bem-estar emocional.</p>
        </div>
        <div className="p-6 bg-blue-100 rounded-xl shadow-md">
          <FaComments className="text-3xl text-blue-700 mb-2" />
          <h3 className="text-xl font-semibold">Terapia de Casal</h3>
          <p className="text-sm text-gray-600">Ajuda para fortalecer relações e melhorar a comunicação.</p>
        </div>
        <div className="p-6 bg-blue-100 rounded-xl shadow-md">
          <FaBookOpen className="text-3xl text-blue-700 mb-2" />
          <h3 className="text-xl font-semibold">Palestras e Workshops</h3>
          <p className="text-sm text-gray-600">Conteúdos sobre saúde mental para grupos e empresas.</p>
        </div>
      </div>
    </div>
  );
};

const App = () => {
  return (
    <>
      <Home />
      <Services />
    </>
  );
};

export default App;
