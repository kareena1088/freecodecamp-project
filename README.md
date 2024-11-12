-
-- PostgreSQL database dump
--

-- Dumped from database version 12.17 (Ubuntu 12.17-1.pgdg22.04+1)
-- Dumped by pg_dump version 12.17 (Ubuntu 12.17-1.pgdg22.04+1)

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

DROP DATABASE universe;
--
-- Name: universe; Type: DATABASE; Schema: -; Owner: freecodecamp
--

CREATE DATABASE universe WITH TEMPLATE = template0 ENCODING = 'UTF8' LC_COLLATE = 'C.UTF-8' LC_CTYPE = 'C.UTF-8';


ALTER DATABASE universe OWNER TO freecodecamp;

\connect universe

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

SET default_tablespace = '';

SET default_table_access_method = heap;

--
-- Name: galaxy; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.galaxy (
    galaxy_id numeric NOT NULL,
    name character varying(100),
    age integer NOT NULL,
    height integer NOT NULL,
    adderess text,
    indian boolean
);


ALTER TABLE public.galaxy OWNER TO freecodecamp;

--
-- Name: moon; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.moon (
    moon_id numeric NOT NULL,
    name character varying(100),
    age integer NOT NULL,
    height integer NOT NULL,
    adderess text,
    indian boolean,
    planet_id numeric
);


ALTER TABLE public.moon OWNER TO freecodecamp;

--
-- Name: planet; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.planet (
    planet_id numeric NOT NULL,
    name character varying(100),
    age integer NOT NULL,
    height integer NOT NULL,
    adderess text,
    indian boolean,
    star_id numeric
);


ALTER TABLE public.planet OWNER TO freecodecamp;

--
-- Name: star; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.star (
    star_id numeric NOT NULL,
    name character varying(100),
    age integer NOT NULL,
    height integer NOT NULL,
    address text,
    indian boolean,
    galaxy_id numeric
);


ALTER TABLE public.star OWNER TO freecodecamp;

--
-- Name: sun; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.sun (
    sun_id numeric NOT NULL,
    name character varying(100),
    age integer NOT NULL,
    height integer NOT NULL,
    adderess text,
    indian boolean,
    phone_no numeric
);


ALTER TABLE public.sun OWNER TO freecodecamp;

--
-- Data for Name: galaxy; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.galaxy VALUES (1, 'nbjhh', 16, 15, 'jbuhgh', true);
INSERT INTO public.galaxy VALUES (2, 'aqw', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (3, 'aqr', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (4, 'aqrt', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (5, 'qwe', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (6, 'awse', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (7, 'qwert', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (8, 'vgy', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (9, 'cft', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (10, 'vghy', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (11, 'vgftgh', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (12, 'bhggy', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (13, 'bhgbgu', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (14, 'qewec', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (15, 'ngfyj', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (16, 'tftvg', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (17, 'bjuhjvhg', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (18, 'cfrdtyh', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (19, 'ghvyhui', 19, 134, 'vgfgvgh', true);
INSERT INTO public.galaxy VALUES (20, 'ghsgfg', 19, 134, 'vgfgvgh', true);


--
-- Data for Name: moon; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.moon VALUES (1, 'shuhana', 17, 45, 'qwer', false, 1);
INSERT INTO public.moon VALUES (2, 'shuhana', 17, 45, 'sdfewf', false, 2);
INSERT INTO public.moon VALUES (3, 'shuhana', 17, 45, 'bhvbhj', false, 3);
INSERT INTO public.moon VALUES (4, 'shuhana', 17, 45, 'bhgyuhj', false, 4);
INSERT INTO public.moon VALUES (5, 'shuhana', 17, 45, 'vhgybg', false, 5);
INSERT INTO public.moon VALUES (6, 'shuhana', 17, 45, 'bhgygu', false, 6);
INSERT INTO public.moon VALUES (7, 'shuhana', 17, 45, 'hjhuxdd', false, 7);
INSERT INTO public.moon VALUES (8, 'shuhana', 17, 45, 'vgftvhjb', false, 8);
INSERT INTO public.moon VALUES (9, 'shuhana', 17, 45, 'bhgvgy', false, 9);
INSERT INTO public.moon VALUES (10, 'shuhana', 17, 45, 'vyyhg', false, 10);
INSERT INTO public.moon VALUES (11, 'shuhana', 17, 45, 'bggyj', false, 11);
INSERT INTO public.moon VALUES (12, 'shuhana', 17, 45, 'bhgyhub', false, 12);
INSERT INTO public.moon VALUES (13, 'shuhana', 17, 45, 'vyybhcu', false, 13);
INSERT INTO public.moon VALUES (14, 'shuhana', 17, 45, 'bdschgu', false, 14);
INSERT INTO public.moon VALUES (15, 'shuhana', 17, 45, 'bsuuw', false, 15);
INSERT INTO public.moon VALUES (16, 'shuhana', 17, 45, 'baduhd', false, 16);
INSERT INTO public.moon VALUES (17, 'shuhana', 17, 45, 'bcjhusdj', false, 17);
INSERT INTO public.moon VALUES (18, 'shuhana', 17, 45, 'bjhcuhc', false, 18);
INSERT INTO public.moon VALUES (19, 'shuhana', 17, 45, 'nbsdjchsd', false, 19);
INSERT INTO public.moon VALUES (20, 'shuhana', 17, 45, 'bsuduwedj', false, 20);


--
-- Data for Name: planet; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.planet VALUES (1, 'komal', 18, 1, 'vghyg', true, 1);
INSERT INTO public.planet VALUES (2, 'komal', 18, 2, 'vghyg', true, 2);
INSERT INTO public.planet VALUES (3, 'komal', 18, 3, 'vghyg', true, 3);
INSERT INTO public.planet VALUES (4, 'komal', 18, 4, 'vghyg', true, 4);
INSERT INTO public.planet VALUES (5, 'komal', 18, 5, 'vghyg', true, 5);
INSERT INTO public.planet VALUES (6, 'komal', 18, 6, 'vghyg', true, 6);
INSERT INTO public.planet VALUES (7, 'komal', 18, 7, 'vghyg', true, 7);
INSERT INTO public.planet VALUES (8, 'komal', 18, 8, 'vghyg', true, 8);
INSERT INTO public.planet VALUES (9, 'komal', 18, 9, 'vghyg', true, 9);
INSERT INTO public.planet VALUES (10, 'komal', 18, 10, 'vghyg', true, 10);
INSERT INTO public.planet VALUES (11, 'komal', 18, 11, 'vghyg', true, 11);
INSERT INTO public.planet VALUES (12, 'komal', 18, 12, 'vghyg', true, 12);
INSERT INTO public.planet VALUES (13, 'komal', 18, 13, 'vghyg', true, 13);
INSERT INTO public.planet VALUES (14, 'komal', 18, 14, 'vghyg', true, 14);
INSERT INTO public.planet VALUES (15, 'komal', 18, 15, 'vghyg', true, 15);
INSERT INTO public.planet VALUES (16, 'komal', 18, 16, 'vghyg', true, 16);
INSERT INTO public.planet VALUES (17, 'komal', 18, 17, 'vghyg', true, 17);
INSERT INTO public.planet VALUES (18, 'komal', 18, 18, 'vghyg', true, 18);
INSERT INTO public.planet VALUES (19, 'komal', 18, 19, 'vghyg', true, 19);
INSERT INTO public.planet VALUES (20, 'komal', 18, 20, 'vghyg', true, 20);


--
-- Data for Name: star; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.star VALUES (1, 'kareena', 1, 456, 'gfygy', false, 1);
INSERT INTO public.star VALUES (2, 'kareena', 2, 12, 'hgy', true, 2);
INSERT INTO public.star VALUES (3, 'kareena', 3, 12, 'hgy', true, 3);
INSERT INTO public.star VALUES (4, 'kareena', 4, 12, 'hgy', true, 4);
INSERT INTO public.star VALUES (5, 'kareena', 5, 12, 'hgy', true, 5);
INSERT INTO public.star VALUES (6, 'kareena', 6, 12, 'hgy', true, 6);
INSERT INTO public.star VALUES (7, 'kareena', 7, 12, 'hgy', true, 7);
INSERT INTO public.star VALUES (8, 'kareena', 8, 12, 'hgy', true, 8);
INSERT INTO public.star VALUES (9, 'kareena', 9, 12, 'hgy', true, 9);
INSERT INTO public.star VALUES (10, 'kareena', 10, 12, 'hgy', true, 10);
INSERT INTO public.star VALUES (11, 'kareena', 11, 12, 'hgy', true, 11);
INSERT INTO public.star VALUES (12, 'kareena', 12, 12, 'hgy', true, 12);
INSERT INTO public.star VALUES (13, 'kareena', 13, 12, 'hgy', true, 13);
INSERT INTO public.star VALUES (14, 'kareena', 14, 12, 'hgy', true, 14);
INSERT INTO public.star VALUES (15, 'kareena', 15, 12, 'hgy', true, 15);
INSERT INTO public.star VALUES (16, 'kareena', 16, 12, 'hgy', true, 16);
INSERT INTO public.star VALUES (17, 'kareena', 17, 12, 'hgy', true, 17);
INSERT INTO public.star VALUES (18, 'kareena', 18, 12, 'hgy', true, 18);
INSERT INTO public.star VALUES (19, 'kareena', 19, 12, 'hgy', true, 19);
INSERT INTO public.star VALUES (20, 'kareena', 20, 12, 'hgy', true, 20);


--
-- Data for Name: sun; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.sun VALUES (1, 'lucky', 19, 34, 'sgchsgh', false, 1234);
INSERT INTO public.sun VALUES (2, 'lucky', 19, 34, 'sgchsgh', false, 3456);
INSERT INTO public.sun VALUES (3, 'lucky', 19, 34, 'sgchsgh', false, 5678);


--
-- Name: galaxy galaxy_name_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_name_key UNIQUE (name);


--
-- Name: galaxy galaxy_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_pkey PRIMARY KEY (galaxy_id);


--
-- Name: moon moon_adderess_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_adderess_key UNIQUE (adderess);


--
-- Name: moon moon_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_pkey PRIMARY KEY (moon_id);


--
-- Name: planet planet_height_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_height_key UNIQUE (height);


--
-- Name: planet planet_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_pkey PRIMARY KEY (planet_id);


--
-- Name: star star_age_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_age_key UNIQUE (age);


--
-- Name: star star_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_pkey PRIMARY KEY (star_id);


--
-- Name: sun sun_phone_no_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.sun
    ADD CONSTRAINT sun_phone_no_key UNIQUE (phone_no);


--
-- Name: sun sun_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.sun
    ADD CONSTRAINT sun_pkey PRIMARY KEY (sun_id);


--
-- Name: moon fkmoon; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT fkmoon FOREIGN KEY (planet_id) REFERENCES public.planet(planet_id);


--
-- Name: planet fkplanet; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT fkplanet FOREIGN KEY (star_id) REFERENCES public.star(star_id);


--
-- Name: star fkstar; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT fkstar FOREIGN KEY (galaxy_id) REFERENCES public.galaxy(galaxy_id);


--
-- PostgreSQL database dump complete
--

