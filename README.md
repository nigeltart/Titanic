# Titanic
The classic first Kaggle

Initial thoughts on each field:

    1) PassengerId 891 non-null int64 - Meaningless key: delete
    2) Survived 891 non-null int64 - The Boolean target to predict
    3) Pclass 891 non-null int64 - 1, 2, 3. Proxy for social class, so use as an integer
    4) Name 891 non-null object - Scope for feature engineering a person's title, also Swedish (lots of passengers) names often end in _sen
    5) Sex 891 non-null object - Simple male/female. No non-binary in 1912!
    6) Age 714 non-null float64- 80% present. Worth imputing the missing 20%
    7) SibSp 891 non-null int64 - Explore whether families all die/survive together
    8) Parch 891 non-null int64 - Explore whether families all die/survive together
    9) Ticket 891 non-null object - I can't imagine the ticket code has any importance: delete
    10) Fare 891 non-null float64- Originally LSD, but converted to decimal. Multiples of guineas (£1.05) might show upper class
    11) Cabin 204 non-null object - 23% present. First letter probably shows the deck, ie proximity to lifeboat
    12) Embarked 889 non-null object - Possible discrimination against Irish passengers

