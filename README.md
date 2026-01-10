-- phpMyAdmin SQL Dump
-- version 5.2.1
-- https://www.phpmyadmin.net/
--
-- Host: 127.0.0.1
-- Creato il: Set 14, 2025 alle 18:31
-- Versione del server: 10.4.32-MariaDB
-- Versione PHP: 8.2.12

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";

--
-- Database: `museo`
--

-- --------------------------------------------------------

--
-- Struttura della tabella `aggiunta`
--

CREATE TABLE `aggiunta` (
  `codServizio` int(11) NOT NULL,
  `idBiglietto` int(200) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

--
-- Dump dei dati per la tabella `aggiunta`
--

INSERT INTO `aggiunta` (`codServizio`, `idBiglietto`) VALUES
(2, 110),
(2, 165),
(2, 181),
(2, 193),
(2, 213),
(2, 215),
(2, 218),
(2, 225),
(3, 130),
(3, 150),
(3, 215);

-- --------------------------------------------------------

--
-- Struttura della tabella `biglietto`
--

CREATE TABLE `biglietto` (
  `idBiglietto` int(11) NOT NULL,
  `prezzo` float NOT NULL,
  `dataValidita` date NOT NULL,
  `utente` varchar(40) DEFAULT NULL,
  `idVisita` varchar(15) DEFAULT NULL,
  `codTransazione` int(11) DEFAULT NULL,
  `codCategoria` int(11) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

--
-- Dump dei dati per la tabella `biglietto`
--

INSERT INTO `biglietto` (`idBiglietto`, `prezzo`, `dataValidita`, `utente`, `idVisita`, `codTransazione`, `codCategoria`) VALUES
(110, 15, '2024-06-06', 'aaaaaaaaa', '2', 71, 1),
(111, 20, '2024-06-08', 'aaaaaaaaa', '3', 72, 1),
(112, 20, '2024-06-08', 'aaaaaaaaa', '3', 72, 1),
(113, 20, '2024-06-08', 'aaaaaaaaa', '3', 72, 1),
(114, 20, '2024-06-08', 'aaaaaaaaa', '3', 72, 1),
(115, 20, '2024-06-08', 'aaaaaaaaa', '3', 72, 1),
(116, 20, '2024-06-08', 'aaaaaaaaa', '3', 72, 1),
(117, 20, '2024-06-08', 'aaaaaaaaa', '3', 72, 1),
(118, 20, '2024-06-08', 'aaaaaaaaa', '3', 72, 1),
(119, 20, '2024-06-08', 'aaaaaaaaa', '3', 72, 1),
(120, 20, '2024-06-08', 'aaaaaaaaa', '3', 72, 1),
(121, 16, '2024-06-08', 'aaaaaaaaa', '3', 72, 2),
(122, 16, '2024-06-08', 'aaaaaaaaa', '3', 72, 2),
(123, 16, '2024-06-08', 'aaaaaaaaa', '3', 72, 2),
(124, 16, '2024-06-08', 'aaaaaaaaa', '3', 72, 2),
(125, 16, '2024-06-08', 'aaaaaaaaa', '3', 72, 2),
(126, 16, '2024-06-08', 'aaaaaaaaa', '3', 72, 2),
(127, 16, '2024-06-08', 'aaaaaaaaa', '3', 72, 2),
(128, 16, '2024-06-08', 'aaaaaaaaa', '3', 72, 2),
(129, 16, '2024-06-08', 'aaaaaaaaa', '3', 72, 2),
(130, 16, '2024-06-08', 'aaaaaaaaa', '3', 72, 2),
(131, 20, '2024-06-08', 'aaaaaaaaa', '3', 73, 1),
(132, 20, '2024-06-08', 'aaaaaaaaa', '3', 73, 1),
(133, 20, '2024-06-08', 'aaaaaaaaa', '3', 73, 1),
(134, 20, '2024-06-08', 'aaaaaaaaa', '3', 73, 1),
(135, 20, '2024-06-08', 'aaaaaaaaa', '3', 73, 1),
(136, 20, '2024-06-08', 'aaaaaaaaa', '3', 73, 1),
(137, 20, '2024-06-08', 'aaaaaaaaa', '3', 73, 1),
(138, 20, '2024-06-08', 'aaaaaaaaa', '3', 73, 1),
(139, 20, '2024-06-08', 'aaaaaaaaa', '3', 73, 1),
(140, 20, '2024-06-08', 'aaaaaaaaa', '3', 73, 1),
(141, 16, '2024-06-08', 'aaaaaaaaa', '3', 73, 2),
(142, 16, '2024-06-08', 'aaaaaaaaa', '3', 73, 2),
(143, 16, '2024-06-08', 'aaaaaaaaa', '3', 73, 2),
(144, 16, '2024-06-08', 'aaaaaaaaa', '3', 73, 2),
(145, 16, '2024-06-08', 'aaaaaaaaa', '3', 73, 2),
(146, 16, '2024-06-08', 'aaaaaaaaa', '3', 73, 2),
(147, 16, '2024-06-08', 'aaaaaaaaa', '3', 73, 2),
(148, 16, '2024-06-08', 'aaaaaaaaa', '3', 73, 2),
(149, 16, '2024-06-08', 'aaaaaaaaa', '3', 73, 2),
(150, 16, '2024-06-08', 'aaaaaaaaa', '3', 73, 2),
(151, 15, '0000-00-00', 'aaaaaaaaa', '2', 74, 1),
(152, 15, '0000-00-00', 'aaaaaaaaa', '2', 74, 1),
(153, 15, '0000-00-00', 'aaaaaaaaa', '2', 74, 1),
(154, 15, '0000-00-00', 'aaaaaaaaa', '2', 74, 1),
(155, 15, '0000-00-00', 'aaaaaaaaa', '2', 74, 1),
(156, 12, '0000-00-00', 'aaaaaaaaa', '2', 74, 2),
(157, 12, '0000-00-00', 'aaaaaaaaa', '2', 74, 2),
(158, 12, '0000-00-00', 'aaaaaaaaa', '2', 74, 2),
(159, 12, '0000-00-00', 'aaaaaaaaa', '2', 74, 2),
(160, 12, '0000-00-00', 'aaaaaaaaa', '2', 74, 2),
(161, 12, '0000-00-00', 'aaaaaaaaa', '2', 74, 2),
(162, 12, '0000-00-00', 'aaaaaaaaa', '2', 74, 2),
(163, 12, '0000-00-00', 'aaaaaaaaa', '2', 74, 2),
(164, 12, '0000-00-00', 'aaaaaaaaa', '2', 74, 2),
(165, 12, '0000-00-00', 'aaaaaaaaa', '2', 74, 2),
(166, 15, '0000-00-00', 'aaaaaaaaa', '2', 75, 1),
(167, 15, '0000-00-00', 'aaaaaaaaa', '2', 75, 1),
(168, 15, '0000-00-00', 'aaaaaaaaa', '2', 75, 1),
(169, 15, '0000-00-00', 'aaaaaaaaa', '2', 75, 1),
(170, 15, '0000-00-00', 'aaaaaaaaa', '2', 75, 1),
(171, 15, '0000-00-00', 'aaaaaaaaa', '2', 75, 1),
(172, 12, '0000-00-00', 'aaaaaaaaa', '2', 75, 2),
(173, 12, '0000-00-00', 'aaaaaaaaa', '2', 75, 2),
(174, 12, '0000-00-00', 'aaaaaaaaa', '2', 75, 2),
(175, 12, '0000-00-00', 'aaaaaaaaa', '2', 75, 2),
(176, 12, '0000-00-00', 'aaaaaaaaa', '2', 75, 2),
(177, 12, '0000-00-00', 'aaaaaaaaa', '2', 75, 2),
(178, 12, '0000-00-00', 'aaaaaaaaa', '2', 75, 2),
(179, 12, '0000-00-00', 'aaaaaaaaa', '2', 75, 2),
(180, 12, '0000-00-00', 'aaaaaaaaa', '2', 75, 2),
(181, 12, '0000-00-00', 'aaaaaaaaa', '2', 75, 2),
(182, 15, '0000-00-00', 'aaaaaaaaa', '2', 76, 1),
(183, 15, '0000-00-00', 'aaaaaaaaa', '2', 76, 1),
(184, 15, '0000-00-00', 'aaaaaaaaa', '2', 76, 1),
(185, 15, '0000-00-00', 'aaaaaaaaa', '2', 76, 1),
(186, 15, '0000-00-00', 'aaaaaaaaa', '2', 76, 1),
(187, 15, '0000-00-00', 'aaaaaaaaa', '2', 76, 1),
(188, 15, '0000-00-00', 'aaaaaaaaa', '2', 76, 1),
(189, 12, '0000-00-00', 'aaaaaaaaa', '2', 76, 2),
(190, 12, '0000-00-00', 'aaaaaaaaa', '2', 76, 2),
(191, 12, '0000-00-00', 'aaaaaaaaa', '2', 76, 2),
(192, 12, '0000-00-00', 'aaaaaaaaa', '2', 76, 2),
(193, 12, '0000-00-00', 'aaaaaaaaa', '2', 76, 2),
(194, 15, '0000-00-00', 'aaaaaaaaa', '2', 77, 1),
(195, 15, '0000-00-00', 'aaaaaaaaa', '2', 77, 1),
(196, 15, '0000-00-00', 'aaaaaaaaa', '2', 77, 1),
(197, 15, '0000-00-00', 'aaaaaaaaa', '2', 77, 1),
(198, 15, '0000-00-00', 'aaaaaaaaa', '2', 77, 1),
(199, 15, '0000-00-00', 'aaaaaaaaa', '2', 77, 1),
(200, 15, '0000-00-00', 'aaaaaaaaa', '2', 77, 1),
(201, 15, '0000-00-00', 'aaaaaaaaa', '2', 77, 1),
(202, 15, '0000-00-00', 'aaaaaaaaa', '2', 77, 1),
(203, 15, '0000-00-00', 'aaaaaaaaa', '2', 77, 1),
(204, 12, '0000-00-00', 'aaaaaaaaa', '2', 77, 2),
(205, 12, '0000-00-00', 'aaaaaaaaa', '2', 77, 2),
(206, 12, '0000-00-00', 'aaaaaaaaa', '2', 77, 2),
(207, 12, '0000-00-00', 'aaaaaaaaa', '2', 77, 2),
(208, 12, '0000-00-00', 'aaaaaaaaa', '2', 77, 2),
(209, 12, '0000-00-00', 'aaaaaaaaa', '2', 77, 2),
(210, 12, '0000-00-00', 'aaaaaaaaa', '2', 77, 2),
(211, 12, '0000-00-00', 'aaaaaaaaa', '2', 77, 2),
(212, 12, '0000-00-00', 'aaaaaaaaa', '2', 77, 2),
(213, 12, '0000-00-00', 'aaaaaaaaa', '2', 77, 2),
(214, 16, '2024-06-06', 'bb', '3', 78, 2),
(215, 16, '2024-06-06', 'bb', '3', 78, 2),
(216, 15, '0000-00-00', 'bb', '2', 82, 1),
(217, 15, '0000-00-00', 'bb', '2', 82, 1),
(218, 12, '0000-00-00', 'bb', '2', 82, 2),
(219, 15, '0000-00-00', 'bb', '2', 83, 1),
(220, 15, '0000-00-00', 'bb', '2', 83, 1),
(221, 12, '0000-00-00', 'bb', '2', 83, 2),
(222, 12, '0000-00-00', 'bb', '2', 83, 2),
(223, 12, '0000-00-00', 'bb', '2', 83, 2),
(224, 12, '0000-00-00', 'bb', '2', 83, 2),
(225, 12, '0000-00-00', 'bb', '2', 83, 2),
(226, 15, '2024-07-04', 'bb', '2', 84, 1),
(227, 15, '2024-07-04', 'bb', '2', 84, 1);

-- --------------------------------------------------------

--
-- Struttura della tabella `carta`
--

CREATE TABLE `carta` (
  `numCarta` varchar(16) NOT NULL,
  `nome` varchar(255) NOT NULL,
  `cognome` varchar(255) NOT NULL,
  `tipoCarta` varchar(50) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

--
-- Dump dei dati per la tabella `carta`
--

INSERT INTO `carta` (`numCarta`, `nome`, `cognome`, `tipoCarta`) VALUES
('00000000000000', 'mio', 'padre', 'patata'),
('0000000000000000', 'jjjjjjjjjjjjjjjj', 'jjjjjjjj', 'patata'),
('1111111111111111', '1111', '1111', 'patata'),
('111111111111767', 'grdut', 'jhgjhg', 'patata'),
('1111222233334444', 'Laura', 'Bianchi', 'Visa'),
('121212122121212', '1212', '1212', 'patata'),
('1234123412341234', 'aaaaaaaa', 'aaaaaaaa', 'patata'),
('1234123443214321', 'asfasfasd', 'asdfasdfasd', 'patata'),
('1234123456785678', 'qweqw', 'qweqwe', 'patata'),
('1234567890123456', 'Mario', 'Rossi', 'Visa'),
('150150150150150', '1051', '1051', 'patata'),
('2222222222222222', '2222', '22222', 'patata'),
('3333333333333', 'gaga', 'gagga', 'patata'),
('3444444444444', 'frw', 'werwer', 'patata'),
('55555555555555', '11', '15555', 'patata'),
('5555666677778888', 'Giovanni', 'Verdi', 'Mastercard'),
('76597976', 'PPoldoo', 'Cognome', 'VIAS'),
('7777777777777777', 'oiuyouyi', 'iuiyu', 'patata'),
('8787878787878778', 'jkjk', 'kjkjkj', 'patata'),
('8888888888888', 'jkjkjkjkjkj', 'lklklklklk', 'patata'),
('88888888888888', 'baobao', 'baba', 'patata'),
('8888888888899', 'jnkkhj', 'jyguy', 'patata'),
('9876543210987654', 'Giulia', 'Verdi', 'Mastercard'),
('9999999999999999', 'sono ', 'la prova', 'patata');

-- --------------------------------------------------------

--
-- Struttura della tabella `categoria`
--

CREATE TABLE `categoria` (
  `codCategoria` int(11) NOT NULL,
  `nome` varchar(255) NOT NULL,
  `tipoDocumento` varchar(255) NOT NULL,
  `sconto` float NOT NULL,
  `descrizione` varchar(255) DEFAULT NULL,
  `tipoCategoria` varchar(255) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

--
-- Dump dei dati per la tabella `categoria`
--

INSERT INTO `categoria` (`codCategoria`, `nome`, `tipoDocumento`, `sconto`, `descrizione`, `tipoCategoria`) VALUES
(1, 'Adulti', 'Documento d\'identita\'', 0, 'Categoria standard per adulti', 'standard'),
(2, 'Studenti', 'Carta studenti', 0.2, 'Sconto per studenti su presentazione della carta', 'ridotto'),
(3, 'Senior', 'Documento d\'identità', 0.3, 'Sconto per anziani sopra i 65 anni', 'ridotto'),
(4, 'Bambini', 'Certificato di nascita', 0.5, 'Sconto per bambini sotto i 12 anni', 'ridotto');

-- --------------------------------------------------------

--
-- Struttura della tabella `gallery`
--

CREATE TABLE `gallery` (
  `idFoto` int(11) NOT NULL,
  `descrizione` varchar(255) DEFAULT NULL,
  `idVisita` varchar(40) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

--
-- Dump dei dati per la tabella `gallery`
--

INSERT INTO `gallery` (`idFoto`, `descrizione`, `idVisita`) VALUES
(1, 'Foto delle opere d\'arte', '1'),
(2, 'Scatti dell\'evento di apertura', '2'),
(3, 'Foto della visita notturna', '3'),
(4, 'Immagini del tour enogastronomico', '4');

-- --------------------------------------------------------

--
-- Struttura della tabella `offerta`
--

CREATE TABLE `offerta` (
  `codServizio` int(11) NOT NULL,
  `idVisita` varchar(15) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

--
-- Dump dei dati per la tabella `offerta`
--

INSERT INTO `offerta` (`codServizio`, `idVisita`) VALUES
(1, '1'),
(2, '2'),
(3, '3'),
(4, '4');

-- --------------------------------------------------------

--
-- Struttura della tabella `servizio`
--

CREATE TABLE `servizio` (
  `codServizio` int(11) NOT NULL,
  `descrizione` varchar(255) DEFAULT NULL,
  `prezzoAPersona` float NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

--
-- Dump dei dati per la tabella `servizio`
--

INSERT INTO `servizio` (`codServizio`, `descrizione`, `prezzoAPersona`) VALUES
(1, 'Tour guidato', 20),
(2, 'Visita multimediale', 15),
(3, 'Noleggio audio guida', 5),
(4, 'Visita notturna', 25),
(5, 'Visita guidata speciale', 30),
(6, 'Noleggio audioguida avanzato', 7.5);

-- --------------------------------------------------------

--
-- Struttura della tabella `transazione`
--

CREATE TABLE `transazione` (
  `codTransazione` int(11) NOT NULL,
  `utente` varchar(40) DEFAULT NULL,
  `numCarta` varchar(16) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

--
-- Dump dei dati per la tabella `transazione`
--

INSERT INTO `transazione` (`codTransazione`, `utente`, `numCarta`) VALUES
(1, 'user1', '1234567890123456'),
(2, 'admin1', '9876543210987654'),
(3, 'user2', '1111222233334444'),
(4, 'admin2', '5555666677778888'),
(5, 'aaaaaaaa', '12387987234'),
(6, 'aaaaaaaa', '293873428374'),
(7, 'aaaaaaaa', '29387342'),
(8, 'aaaaaaaa', '2938734'),
(47, 'aaaaaaaaa', '1234123412341234'),
(48, 'aaaaaaaaa', '1234123443214321'),
(49, 'aaaaaaaaa', '1234123443214321'),
(50, 'dfdf', 'efe'),
(51, 'aaaaaaaaa', '1111111111111111'),
(52, 'aaaaaaaaa', '2222222222222222'),
(53, 'aaaaaaaaa', '2222222222222222'),
(54, 'aaaaaaaaa', '2222222222222222'),
(55, 'aaaaaaaaa', '1234123456785678'),
(56, 'dfdf', 'efe'),
(57, 'dfdf', 'efe'),
(58, 'aaaaaaaaa', '1234123412341234'),
(59, 'aaaaaaaaa', '0000000000000000'),
(60, 'aaaaaaaaa', '0000000000000000'),
(61, 'aaaaaaaaa', '0000000000000000'),
(62, 'aaaaaaaaa', '0000000000000000'),
(63, 'aaaaaaaaa', '0000000000000000'),
(64, 'aaaaaaaaa', '0000000000000000'),
(65, 'aaaaaaaaa', '0000000000000000'),
(66, 'aaaaaaaaa', '0000000000000000'),
(67, 'aaaaaaaaa', '9999999999999999'),
(68, 'aaaaaaaaa', '3333333333333'),
(69, 'aaaaaaaaa', '55555555555555'),
(70, 'aaaaaaaaa', '55555555555555'),
(71, 'aaaaaaaaa', '1234123412341234'),
(72, 'aaaaaaaaa', '9999999999999999'),
(73, 'aaaaaaaaa', '9999999999999999'),
(74, 'aaaaaaaaa', '00000000000000'),
(75, 'aaaaaaaaa', '8787878787878778'),
(76, 'aaaaaaaaa', '111111111111767'),
(77, 'aaaaaaaaa', '7777777777777777'),
(78, 'bb', '1111111111111111'),
(79, 'bb', '3444444444444'),
(80, 'bb', '88888888888888'),
(81, 'bb', '8888888888888'),
(82, 'bb', '8888888888899'),
(83, 'bb', '150150150150150'),
(84, 'bb', '121212122121212');

-- --------------------------------------------------------

--
-- Struttura della tabella `utente`
--

CREATE TABLE `utente` (
  `username` varchar(40) NOT NULL,
  `nome` varchar(50) NOT NULL,
  `cognome` varchar(50) NOT NULL,
  `mail` varchar(255) NOT NULL,
  `passw` varchar(255) NOT NULL,
  `tipoUtente` varchar(255) NOT NULL CHECK (`tipoUtente` in ('user','admin'))
) ENGINE=InnoDB DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

--
-- Dump dei dati per la tabella `utente`
--

INSERT INTO `utente` (`username`, `nome`, `cognome`, `mail`, `passw`, `tipoUtente`) VALUES
('aa', 'aa', 'aa', 'aa@aa.aa', '$2y$10$2.XGqSoxMxBk/P6y7I7D9ueXOqtvdoEmoPJlyy3TBqp2cxeST5g1.', 'user'),
('aaaaaaaa', 'aaaaaaaaa', 'aaaaaaaaa', 'aaaaaaaaa@', '$2y$10$BSepb466LftP51KVdSQ9BelivIxNk8Yj4UoRsvsygZYbleJNNNUsy', 'user'),
('aaaaaaaaa', 'aaaaaaaa', 'aaaaaaaa', 'aaaaaaaa@', '$2y$10$XrOZ1L2c2UBX4RGKd/4uL.7b87K5IX87ytwTu0ycWXNzwM5tpYsZO', 'user'),
('admin1', 'Admin', 'Admin', 'admin@email.com', 'adminpasswordhash1', 'admin'),
('admin2', 'Super', 'Admin', 'superadmin@email.com', 'superadminpasswordhash1', 'admin'),
('bb', 'bb', 'baba', 'bababa@gmail.com', '$2y$10$2w9KDsrWzX32R9GuBYWZW.CxLvcmHlNYX2eGrwAKFCc/NbL8Ty8yy', 'user'),
('bbe', 'sdfsdfsfs\\i', 'jkhkjh', 'iuihuih@', '$2y$10$8KcDQiHRWIvzHg0iVBCF0edSnCm04BXINWhmn2l.p3JuPO4IMDj6O', 'user'),
('user1', 'Mario', 'Rossi', 'mario@email.com', 'passwordhash1', 'user'),
('user2', 'Laura', 'Bianchi', 'laura@email.com', 'passwordhash2', 'user');

-- --------------------------------------------------------

--
-- Struttura della tabella `variazione`
--

CREATE TABLE `variazione` (
  `idVisita` varchar(15) NOT NULL,
  `codCategoria` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

--
-- Dump dei dati per la tabella `variazione`
--

INSERT INTO `variazione` (`idVisita`, `codCategoria`) VALUES
('1', 1),
('2', 1),
('3', 1),
('4', 1),
('2', 2),
('3', 2);

-- --------------------------------------------------------

--
-- Struttura della tabella `visita`
--

CREATE TABLE `visita` (
  `idVisita` int(11) NOT NULL,
  `titolo` varchar(50) NOT NULL,
  `descrizione` varchar(255) DEFAULT NULL,
  `tariffa` float NOT NULL,
  `tipoVisita` varchar(50) NOT NULL CHECK (`tipoVisita` in ('evento','standard')),
  `dataInizio` date DEFAULT NULL,
  `dataFine` date DEFAULT NULL,
  `maxBiglietti` int(11) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1 COLLATE=latin1_swedish_ci;

--
-- Dump dei dati per la tabella `visita`
--

INSERT INTO `visita` (`idVisita`, `titolo`, `descrizione`, `tariffa`, `tipoVisita`, `dataInizio`, `dataFine`, `maxBiglietti`) VALUES
(1, 'Visita guidata al museo', 'Esplora le opere d\'arte con una guida esperta.', 10, 'standard', '2024-05-01', '2024-06-01', 100),
(2, 'Mostra temporanea: Impressionismo', 'Scopri i capolavori impressionisti in esposizione per un periodo limitato.', 15, 'evento', '2024-07-01', '2024-07-15', 50),
(3, 'Visita notturna al museo', 'Esplora il museo sotto la luce delle stelle.', 20, 'evento', '2024-08-01', '2024-08-15', 50),
(4, 'Tour enogastronomico', 'Un tour che ti guida attraverso le prelibatezze culinarie della regione.', 35, 'evento', '2024-09-01', '2024-09-30', 30);

--
-- Indici per le tabelle scaricate
--

--
-- Indici per le tabelle `aggiunta`
--
ALTER TABLE `aggiunta`
  ADD PRIMARY KEY (`codServizio`,`idBiglietto`);

--
-- Indici per le tabelle `biglietto`
--
ALTER TABLE `biglietto`
  ADD PRIMARY KEY (`idBiglietto`);

--
-- Indici per le tabelle `carta`
--
ALTER TABLE `carta`
  ADD PRIMARY KEY (`numCarta`);

--
-- Indici per le tabelle `categoria`
--
ALTER TABLE `categoria`
  ADD PRIMARY KEY (`codCategoria`);

--
-- Indici per le tabelle `gallery`
--
ALTER TABLE `gallery`
  ADD PRIMARY KEY (`idFoto`);

--
-- Indici per le tabelle `offerta`
--
ALTER TABLE `offerta`
  ADD PRIMARY KEY (`codServizio`,`idVisita`);

--
-- Indici per le tabelle `servizio`
--
ALTER TABLE `servizio`
  ADD PRIMARY KEY (`codServizio`);

--
-- Indici per le tabelle `transazione`
--
ALTER TABLE `transazione`
  ADD PRIMARY KEY (`codTransazione`);

--
-- Indici per le tabelle `utente`
--
ALTER TABLE `utente`
  ADD PRIMARY KEY (`username`);

--
-- Indici per le tabelle `variazione`
--
ALTER TABLE `variazione`
  ADD PRIMARY KEY (`codCategoria`,`idVisita`);

--
-- Indici per le tabelle `visita`
--
ALTER TABLE `visita`
  ADD PRIMARY KEY (`idVisita`);

--
-- AUTO_INCREMENT per le tabelle scaricate
--

--
-- AUTO_INCREMENT per la tabella `biglietto`
--
ALTER TABLE `biglietto`
  MODIFY `idBiglietto` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=228;

--
-- AUTO_INCREMENT per la tabella `categoria`
--
ALTER TABLE `categoria`
  MODIFY `codCategoria` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=5;

--
-- AUTO_INCREMENT per la tabella `gallery`
--
ALTER TABLE `gallery`
  MODIFY `idFoto` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=5;

--
-- AUTO_INCREMENT per la tabella `servizio`
--
ALTER TABLE `servizio`
  MODIFY `codServizio` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=7;

--
-- AUTO_INCREMENT per la tabella `transazione`
--
ALTER TABLE `transazione`
  MODIFY `codTransazione` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=85;

--
-- AUTO_INCREMENT per la tabella `visita`
--
ALTER TABLE `visita`
  MODIFY `idVisita` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=5;
COMMIT;
