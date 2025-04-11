import React from "react";
import { HashRouter } from "react-router-dom";
import { Route, Switch } from "react-router-dom";
import Home from "./components/Home";
import Projects from "./components/Projects";
import Contact from "./components/Contact";
import Navbar from "./components/Navbar";

function App() {
  return (
    <HashRouter>
      <Navbar />
      <Switch>
        <Route path="/" exact component={Home} />
        <Route path="/projects" component={Projects} />
        <Route path="/contact" component={Contact} />
      </Switch>
    </HashRouter>
  );
}

export default App;
