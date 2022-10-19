<div align="center">

## Paczka Only DD2 - Wersja Mini.

<img src="https://i.imgur.com/LPsTt48.png"></img>

</div>

<p align="center">
  <a href="#requirements">Wymagania ℹ</a> ×
  <a href="#description">Opis 📄</a> ×
  <a href="#vip">Opis VIP'a 📝</a> ×
  <a href="#configure">Konfiguracja 🛠</a> ×
  <a href="#screenshots">Screenshot 📷</a>
</p>

---


### Description 
- Narzędzia, które ułatwiają prace administracji serwera:
  - **Admin ESP** - plugin, który pozwala adminom widzieć innych graczy przez ściany,
  - **Admin Freelook** - plugin, pozwala adminom sprawdzać każdy team, nie muszą wchodzić na SPECT'a,
  - **Admin IP** - plugin pozwala wydrukować listę graczy wraz z ich adresami IP,
  - **Admin Listen** - plugin dzięki, któremu admin widzi wszystkie wiadomości na say oraz słyszy wszystkie rozmowy graczy,
  - **Admin Voice** - plugin, który dodaje voice chat dla adminów w celu lepszej komunikacji,
  - **Admin Chat** - plugin został odświeżony, zostały dodane do niego nowe kolory, wiadomości na say również zostały odświeżone.

- Pluginy, które urozmaicają rozgrywke:
  - **ABD** - zaawansowany system pokazywania obrażeń,
  - **Assist** - system asyst, tak żeby każdy gracz był zadowolony i nie mówił, że nic nie ma z zabójstwa,
  - **Bomb Timer** - licznik do wybuchu bomby, prosty, informacyjny,
  - **Limit Ping** - wyrzucanie Graczy za zbyt duży ping,
  - **Medals** - system medali, medale zdobywane są za zostanie najlepszym graczem mapy,
  - **Menu** - menu serwera, mały pomocnik dla nowych graczy,
  - **MVP** - system najlepszego gracza rundy, najlepszy gracz rundy otrzymuje również dodatkowe punkty do rang,
  - **No Team Flash** - jak sama nazwa wskazuje, anty flash dla teamu,
  - **Parachute** - zoptymalizowany spadochron,
  - **Ranks** - rozbudowany system rang,
  - **Reset Score** - gracz otrzymuje możliwość zrestartowania statystyk,
  - **Round Sound** - muzyka na sam koniec rundy, z zapisem opcji włącz/wyłącz,
  - **Server Hud** - informacyjny HUD w lewym górnym rogu,
  - **VIP** - system VIP.


### VIP
- VIP posiada:
  - Menu broni dostępne od X rundy,
  - Status **VIP** w Tabeli [TAB],
  - Prefix **VIP** na czacie,
  - Dodatkowe HP za fraga X HP | X HP za HS,
  - Dodatkowe dolary za fraga X$ | X$ HS,
  - Granaty dostępne od X rundy,
  - Deagle dostępny od X rundy.
  
*X - ustawienie cvarów*

### Configure
- Każdy plugin posiada własne cvary, dzięki którym możemy sami ustawić sobie dosłownie wszystko.

<details>
  <summary><b>Admin ESP</b></summary>

```cfg
  - amxx4u_esp "1"
    - Czy Admin ESP ma być włączony?
  - amxx4u_esp_timer "0.3"
    - Czas odświeżania "pasków", które widzi admin
  - amxx4u_esp_allow_all "0"
    - Admin ESP ma być dla każdego?
  - amxx4u_esp_disable_keys "0"
    - Jeżeli nie chcesz ustawiać ESP za pomocą klawiszy reload/backward/forward, ustaw cvar na 1
```
</details>

<details>
  <summary><b>ABD</b></summary>

```cfg
  - dmg_self_self "1"
    - Pokazywać obrażenia od upadku?
  - dmg_self_spec "1"
    - Czy spect ma widzieć obrażenia od spadku obserwowanego gracza?
  - dmg_td_self "1"
    - Pokazywać otrzymane obrażenia?
  - dmg_td_spec "0"
    - Czy spect ma widzieć otrzymane obrażenia obserwowanego gracza?
  - dmg_ta_self "1"
    - Pokazywać zadawane obrażenia?
  - dmg_ta_spec "1"
    - Czy spect ma widzieć zadawane obrażenia obserwowanego gracza?
  - dmg_taken_self "2"
    - Pokazywać obrażenia otrzymane przez ściany?
      - 0 - nie pokazuj | 1 - zawsze pokazuj | 2 - nie pokazuj obrażeń przez ściany
  - dmg_taken_spec "1"
    - Czy spect ma widzieć otrzymane obrażenia przez ściany obserwowanego gracza?
  - dmg_made_self "1"
    - Pokazywać obrażenia zadawane przez ściany?
  - dmg_made_spec "1"
    - Czy spect ma widzieć zadawane obrażenia przez ściany obserwowanego gracza?
  - dmg_hs_taken_self "1"
    - Pokazywać obrażenia otrzymane w głowe?
  - dmg_hs_taken_spec "1"
    - Czy spect ma widzieć otrzymane obrażenia w głowe obserwowanego gracza?
  - dmg_hs_made_self "1"
    - Pokazywać obrażenia zadawane w głowe?
  - dmg_hs_made_spec "1"
    - Czy spect ma widzieć zadawane obrażenia w głowe obserwowanego gracza?
```
</details>

<details>
  <summary><b>Limit Ping</b></summary>

```cfg
  - amxx4u_check_ping "5.0"
    - Co ile ma być sprawdzany ping gracza?
  - amxx4u_check_admin "1"
    - Czy ping admina ma być sprawdzany?
  - amxx4u_ban_kick "0"
    - Co ma być robione z graczem jeżeli przekroczy limit?
      - 0 - Kick | 1 - Ban | 2 - nic nie rób
  - amxx4u_ban_time "5"
    - Czas bana za przekroczony limit pingu
  - amxx4u_limit_check "5"
    - Ile razy gracz ma zostać sprawdzony przed interwencją?
  - amxx4u_limit_ping "105"
    - Jaki maksymalny ping może mieć gracz?
```
</details>

<details>
  <summary><b>Medals</b></summary>

```cfg
  - amxx4u_medals_host "localhost"
  - amxx4u_medals_user "root"
  - amxx4u_medals_pass "pass"
  - amxx4u_medals_data "database"
  - amxx4u_medals_players "4"
    - Od ilu graczy mają być rozdawane medale?
  - amxx4u_medals_map "10.0"
    - Ile czasu przed zmianą mapy mają być rozdawane medale?
```
</details>


<details>
  <summary><b>MVP</b></summary>

```cfg
  - mvp_kill_points "1"
    - Ile punktów za zabójstwo gracza
  - mvp_killhs_points "2"
    - Ile punktów za zabójstwo gracza w glowe
  - mvp_planted_points "2"
    - Ile punktów za podłożenie bomby
  - mvp_explode_points "3"
    - Ile punktów za wybuch bomby dla plantującego
  - mvp_defused_points "2"
    - Ile punktów za rozbrojenie bomby
  - mvp_ctwin_points "1"
    - Ile punktów za wygranie rundy przez CT
  - mvp_ttwin_points "1"
    - Ile punktów za wygranie rundy przez TT
  - mvp_reward_points "1"
    - Ile punktów doliczyć do rangi za zostanie MVP
```
</details>

<details>
  <summary><b>Parachute</b></summary>

```cfg
  - amxx4u_parachute_speed "-150.0"
    - Jaka ma być prędkość spadania?
```
</details>

<details>
  <summary><b>Ranks</b></summary>

```cfg
  - amxx4u_rank_host "localhost"
  - amxx4u_rank_user "root"
  - amxx4u_rank_pass "pass"
  - amxx4u_rank_data "database"
  - amxx4u_rank_players "4"
    - Od ilu graczy ma dodawać punkty do rangi?
  - amxx4u_rank_pkt_kill "1"
    - Ile punktów ma otrzymywać gracz za zabójstwo?
  - amxx4u_rank_pkt_hs "1"
    - Ile punktów ma otrzymywać gracz za zabójstwo w głowe?
  - amxx4u_rank_pkt_plant "1"
    - Ile punktów ma otrzymać gracz za zaplantowanie C4?
  - amxx4u_rank_pkt_defuse "1"
    - Ile punktów ma otrzymać gracz, który rozbroił C4?
  - amxx4u_rank_pkt_round "1"
    - Ile punktów ma otrzymać drużyna, która wygrała runde?
```
</details>

<details>
  <summary><b>HUD</b></summary>

```cfg
  - amxx4u_hud_enabled "1"
    - HUD ma być włączony?
  - amxx4u_hud_chat "1"
    - Wyświetlać informacje co X graczowi, że jego HUD jest wyłączony?
  - amxx4u_hud_time "360.0"
    - Co ile (sekund) wyświetlać graczowi informacje?
  - amxx4u_hud_board "AMXX4u.pl"
    - Nazwa forum wyświetlana w HUD
  - amxx4u_hud_account "1"
    - Wyświetlać status konta gracza?
  - amxx4u_hud_kd "1"
    - Wyświetlać K/D gracza?
  - amxx4u_hud_rank "1"
    - Wyświetlać range gracza?
```
</details>

<details>
  <summary><b>VIP</b></summary>

```cfg
  - vip_player_flag "t"
    - Jaką flagę musi posiadać gracz, aby otrzymać VIP'a?
  - vip_gunmenu_round "3"
    - Od której rundy ma byc wyświetlane menu broni?
  - vip_kill_money "100"
    - Ile dolarów VIP otrzymuje za zabicie gracza?
  - vip_hs_money "200"
    - Ile dolarów VIP otrzymuje za zabicie gracza w głowe?
  - vip_kill_hp "5"
    - Ile HP VIP otrzymuje za zabicie gracza?
  - vip_hs_hp "10"
    - Ile HP VIP otrzymuje za zabicie gracza w głowe?
  - vip_grenade_round "3"
    - Od której rundy VIP ma dostawać granaty?
  - vip_deagle_round "3"
    - Od której rundy VIP ma dostawać deagle?
  - vip_free_enable "1"
    - Darmowy VIP ma być włączony?
  - vip_draw_round "2"
    - W której rundzie ma być losowany VIP?
  - vip_hour_start "21"
    - Od której godziny VIP jest darmowy?
  - vip_hour_end "09"
    - Do której godziny VIP jest darmowy?
  - vip_draw_players "3"
    - Od ilu graczy ma być losowanie VIP'a?
```
</details>

### Screenshots

<details>
  <summary><b>Admin Chat</b></summary>
  
- Nowe kolory

  <img align="left" width="311" height="111" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/admin_lime_say.png"></img>
  <img align="center" width="311" height="111" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/admin_pink_say.png"></img>
  <img align="right" width="311" height="111" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/admin_violet_say.png"></img>

- Odświeżone informacje na czacie

  <img align="left" width="401" height="46" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/admin_chat_mplayer.png"></img>
  <img align="center" width="401" height="46" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/admin_chat_madmin.png"></img>

</details>

<details>
  <summary><b>Admin IP</b></summary>
  
- Menu

  <img width="579" height="327" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/admin_ip_menu.png"></img>

- Konsola

  <img width="990" height="262" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/admin_ip_console.png"></img>

</details>

<details>
  <summary><b>Chat</b></summary>
  
- Wygląd wiadomości na czacie 

  <img width="427" height="42" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/chat_message.png"></img>
</details>


<details>
  <summary><b>VIP</b></summary>
  
- Menu zawierające opis VIP'a

  <img width="566" height="463" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/VIP.png"></img>
</details>


<details>
  <summary><b>HUD</b></summary>
  
- Główny HUD

  <img width="437" height="225" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/hud.png"></img>

- Włącz/Wyłącz HUD Informacja na czacie

  <img width="247" height="39" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/hud_info.png"></img>
  
- Informacja o wyłaczonym HUD'zie

  <img width="437" height="21" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/hud_off_info.png"></img>
</details>


<details>
  <summary><b>Menu</b></summary>
  
- Wygląd menu

  <img width="465" height="314" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/menu.png"></img>
</details>

<details>
  <summary><b>RoundSound</b></summary>
  
- Główne menu roundsound

  <img width="508" height="363" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/res1.png"></img>
  
- Lista utworów

  <img width="504" height="388" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/res2.png"></img>
</details>

<details>
  <summary><b>TOP'ki</b></summary>
  
- TOP Medale

  <img width="951" height="473" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/top_medale.png"></img>
  
- TOP Rangi

  <img width="951" height="473" src="https://github.com/AMXX4u/DD2-1/blob/main/assets/top_rangi.png"></img>
</details>

### Requirements 
- AMXModX 1.9 / AMXModX 1.10
- ReHLDS 3.12.0.780
- ReAPI 5.22.0.254
- ReGameDLL 5.21.0.556
