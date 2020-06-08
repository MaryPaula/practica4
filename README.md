-- phpMyAdmin SQL Dump
-- version 5.0.2
-- https://www.phpmyadmin.net/
--
-- Servidor: 127.0.0.1
-- Tiempo de generación: 08-06-2020 a las 04:38:29
-- Versión del servidor: 10.4.11-MariaDB
-- Versión de PHP: 7.2.31

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Base de datos: `registro`
--

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `persona`
--

CREATE TABLE `persona` (
  `Id` int(20) NOT NULL,
  `Nombres` varchar(100) NOT NULL,
  `Correo` varchar(100) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8;

--
-- Volcado de datos para la tabla `persona`
--

INSERT INTO `persona` (`Id`, `Nombres`, `Correo`) VALUES
(1, 'maria', '123456');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `usuario`
--

CREATE TABLE `usuario` (
  `Id_Usuario` int(11) NOT NULL,
  `DNI` text NOT NULL,
  `Nombres` text NOT NULL,
  `Fecha` text NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8;

--
-- Volcado de datos para la tabla `usuario`
--

INSERT INTO `usuario` (`Id_Usuario`, `DNI`, `Nombres`, `Fecha`) VALUES
(19, 'Los sintomas mas habituales de la COVID-19 son la fiebre, la tos seca y el cansancio. Otros sintomas menos frecuentes que afectan a algunos pacientes son los dolores y molestias, la congestion nasal, el dolor de cabeza, la conjuntivitis, el dolor de garganta, la diarrea, la perdida del gusto o el olfato y las erupciones cutaneas o cambios de color en los dedos de las manos o los pies. Estos sintomas suelen ser leves y comienzan gradualmente. Algunas de las personas infectadas solo presentan sintomas levisimos', 'Cuales son los sintomas de la COVID-19', '10/01/2020'),
(20, 'Los antibioticos no son eficaces contra los virus, solo contra las infecciones bacterianas. La COVID 19 esta causada por un virus, de modo que los antibioticos no sirven frente a ella. No se deben usar antibioticos como medio de prevencion o tratamiento de la COVID 19. En los hospitales, los medicos a veces utilizan antibioticos para prevenir o tratar infecciones bacterianas secundarias que pueden ser una complicacion de la COVID 19 en pacientes gravemente enfermos. Solo deben usarse para tratar una infeccion bacteriana siguiendo las indicaciones de un medico.', 'Son eficaces los antibioticos para prevenir o tratar la COVID 19', '18/02/2020'),
(21, 'El aislamiento se produce cuando una persona que tiene fiebre, tos u otros sintomas de COVID 19 se queda en casa y no va al trabajo, a la escuela o a lugares publicos. Lo puede hacer voluntariamente o por recomendacion de su dispensador de atencion de salud. Sin embargo, si vive en una zona con paludismo (malaria) o dengue, es importante que no ignore la fiebre. Busque ayuda medica. Cuando acuda al centro de salud use una mascarilla si es posible, mantengase al menos a un metro de distancia de las demas personas y no toque las superficies con las manos. En caso de que el enfermo sea un nino, ayudelo a seguir este consejo.', 'Que significa aislarse', '26/03/2020');

--
-- Índices para tablas volcadas
--

--
-- Indices de la tabla `persona`
--
ALTER TABLE `persona`
  ADD PRIMARY KEY (`Id`);

--
-- Indices de la tabla `usuario`
--
ALTER TABLE `usuario`
  ADD PRIMARY KEY (`Id_Usuario`);

--
-- AUTO_INCREMENT de las tablas volcadas
--

--
-- AUTO_INCREMENT de la tabla `persona`
--
ALTER TABLE `persona`
  MODIFY `Id` int(20) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=2;

--
-- AUTO_INCREMENT de la tabla `usuario`
--
ALTER TABLE `usuario`
  MODIFY `Id_Usuario` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=22;
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
