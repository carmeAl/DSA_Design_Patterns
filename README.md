# DSA - Design Patterns
1. I18NManager: Singleton (cache) + ResourceBundle.   I18NManager.getInstance().getText("ca", "l1");
2. FactoryPattern: Factory + Singleton (cache) + Command + LOG4J

Command c = Factory.getInstance().getCommand("C1"); // Classloader (C1)

c.execute();

c = Factory.getInstance().getCommand("C1");  // Cache (C1)

c.execute();
