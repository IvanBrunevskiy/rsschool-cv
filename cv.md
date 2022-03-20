### CV

#### Ivan Brunevskiy

**Contacts:**
- Phone: +37529-572-32-28
- Skipe: live:.cid.dc0462b70d758d0e
- Telegram: Ivan Brunevskiy

**About me:**
My goal is to constantly improve my level of knowledge. My strengths are my quick wit and flexible thinking. I have experience in PHP. Now my goal is to learn JS.

**Skills:**
- PHP
- Laravel
- Drupal
- MySql
- Git
- phpshtorm


***

```php
  public function createPairs() {

    $team = $this->team;
    if (count($team) % 2 != 0) {
      $team[] = 'break';
    }
    $team_days = [];
    for ($x = 0; $x < (count($team) - 1); $x++) {
      $sec = array_key_last($team);
      $one_day_team = [];
      for ($i = 0; $i < (count($team) / 2); $i++) {
        if (($team[$i] !== 'break') && ($team[$sec] !== 'break')) {
          $one_day_team[] = $team[$i] . ' - ' . $team[$sec];
        }
        $sec--;
      }
      $date = $this->getDate($x + 1);
      array_splice($one_day_team, 0, 0, $this->getNameTournament() . ', ' . $date);
      $team_days[$x] = $one_day_team;
      $last = array_pop($team);
      array_splice($team, 1, 0, $last);
      $one_day_team = [];
    }

    $this->printResult($team_days);
  }
```

**Work experience:**
- February - June 2021. Participated in the development of the [IT junior](https://it-junior.by/) project (Laravel).
- July 2021 - present. [YourDevTeam](https://ydt-global.com/) commercial experience. Development of CRM (Drupal).

**Education:**
- 2010 - 2015. Belarusian National Technical University (mechanical engineer).
- August 2020 - January 2021. TeachMeSkills school (php developer).

**English level:**
A2