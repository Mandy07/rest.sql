-- phpMyAdmin SQL Dump
-- version 3.3.9
-- http://www.phpmyadmin.net
--
-- Host: localhost
-- Generation Time: Sep 07, 2015 at 01:20 PM
-- Server version: 5.5.8
-- PHP Version: 5.3.5

SET SQL_MODE="NO_AUTO_VALUE_ON_ZERO";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8 */;

--
-- Database: `rest`
--

-- --------------------------------------------------------

--
-- Table structure for table `booking`
--

CREATE TABLE IF NOT EXISTS `booking` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `rname` varchar(50) NOT NULL,
  `people` varchar(50) NOT NULL,
  `date` varchar(50) NOT NULL,
  `time` varchar(50) NOT NULL,
  `mob` varchar(11) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB  DEFAULT CHARSET=latin1 AUTO_INCREMENT=2 ;

--
-- Dumping data for table `booking`
--

INSERT INTO `booking` (`id`, `rname`, `people`, `date`, `time`, `mob`) VALUES
(1, 'Samrat', '2', '2015-09-08', '10A', '7838982079');

-- --------------------------------------------------------

--
-- Table structure for table `login`
--

CREATE TABLE IF NOT EXISTS `login` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `email` varchar(50) NOT NULL,
  `password` varchar(50) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB  DEFAULT CHARSET=latin1 AUTO_INCREMENT=5 ;

--
-- Dumping data for table `login`
--

INSERT INTO `login` (`id`, `email`, `password`) VALUES
(1, 'mandeepsingh0805@gmail.com', 'mandeepsingh'),
(2, 'mandeep_singh0172@yahoo.com', 'mandy07');

-- --------------------------------------------------------

--
-- Table structure for table `register`
--

CREATE TABLE IF NOT EXISTS `register` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `fname` varchar(50) NOT NULL,
  `lname` varchar(50) NOT NULL,
  `gender` varchar(50) NOT NULL,
  `mobile` varchar(11) NOT NULL,
  `email` varchar(50) NOT NULL,
  `password` varchar(50) NOT NULL,
  `confirmpassword` varchar(50) NOT NULL,
  `Address` varchar(100) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB  DEFAULT CHARSET=latin1 AUTO_INCREMENT=3 ;

--
-- Dumping data for table `register`
--

INSERT INTO `register` (`id`, `fname`, `lname`, `gender`, `mobile`, `email`, `password`, `confirmpassword`, `Address`) VALUES
(1, 'Mandeep ', 'Singh', 'MALE', '7838982079', 'mandeepsingh0805@gmail.com', 'mandeepsingh', 'mandeepsingh', 'santnagr'),
(2, 'Mandeep ', 'Singh', 'MALE', '7838982079', 'mandeep_singh0172@yahoo.com', 'mandy07', 'mandy07', 'gandhi vihar');

-- --------------------------------------------------------

--
-- Table structure for table `restdetails`
--

CREATE TABLE IF NOT EXISTS `restdetails` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `name` varchar(50) NOT NULL,
  `add` varchar(50) NOT NULL,
  `mob` varchar(11) NOT NULL,
  `pno` varchar(11) NOT NULL,
  `email` varchar(50) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB  DEFAULT CHARSET=latin1 AUTO_INCREMENT=2 ;

--
-- Dumping data for table `restdetails`
--

INSERT INTO `restdetails` (`id`, `name`, `add`, `mob`, `pno`, `email`) VALUES
(1, 'Samrat', 'GTB Nagar', '7838982079', '27616905', 'mandeepsingh0805@gmail.com');
