# PotionStacker
• PotionStacker - плагин для позволяющий стакать зелья 


============================================
Дополнительная информация: (RU)
============================================
optimization:
   use-caching: Включить/отключить кэширование хешей зелий
   РЕКОМЕНДУЕТСЯ: true
   ОПИСАНИЕ: Кэширование резко улучшает производительность при большом
   количестве операций стакания. Плагин сохранит уникальный "отпечаток"
   каждого зелья в памяти, чтобы быстро определять, идентичны ли два зелья.
   Вместо проверки всех параметров зелья, плагин просто сравнит два "отпечатка".
  use-caching: true

   hopper-check-delay: Задержка проверки хопера в тиках (1 тик = 0.05 сек)
   РЕКОМЕНДУЕТСЯ: 10
   ОПИСАНИЕ: Определяет, как часто плагин проверяет хопер на наличие зелий
   для стакания. Чем больше число, тем реже проверка (меньше нагрузка,
   но медленнее стакание). 10 тиков = один раз в 0.5 секунды.
   ПРИМЕРЫ:
     5  = Частая проверка (нагруженно, но быстрее)
     10 = Рекомендуемое значение
     20 = Редкая проверка (мало нагрузки, но медленнее)
  hopper-check-delay: 10

   max-operations-per-tick: Максимум операций стакания за один тик
   РЕКОМЕНДУЕТСЯ: 50
   ОПИСАНИЕ: Ограничивает количество операций, которые плагин выполнит
   за один игровой тик. Это предотвращает лаги на сервере. Если установить
   слишком б  льшое число, сервер может начать лагать когда много зелий
   стакается одновременно.
   ПРИМЕРЫ:
     25 = Консервативная нагрузка (меньше лагов, медленнее)
     50 = Стандартная нагрузка
     100+ = Агрессивная нагрузка (может вызвать лаги)
  max-operations-per-tick: 50

   cache-clear-interval: Интервал очистки кэша в тиках
   РЕКОМЕНДУЕТСЯ: 1200
   ОПИСАНИЕ: Каждые N тиков плагин очищает кэш. Это освобождает память.
   Установите 0 для отключения очистки (не рекомендуется для больших серверов).
   1200 тиков = 60 секунд
   ПРИМЕРЫ:
     0 = Кэш никогда не очищается (много памяти)
     600 = Очистка каждые 30 секунд
     1200 = Очистка каждые 60 секунд
     2400 = Очистка каждые 120 секунд
  cache-clear-interval: 1200



============================================
Additional information: (EN)
============================================
optimization:
   use-caching: Enable/disable caching of potion hash values
   RECOMMENDED: true
   DESCRIPTION: Caching significantly improves performance when handling a large
   number of stacking operations. The plugin stores a unique "fingerprint"
   of each potion in memory to quickly determine whether two potions are identical.
   Instead of checking all potion parameters, the plugin simply compares two "fingerprints".
  use-caching: true

   hopper-check-delay: Hopper check delay in ticks (1 tick = 0.05 seconds)
   RECOMMENDED: 10
   DESCRIPTION: Determines how often the plugin checks the hopper for potions
   to be stacked. A higher number means less frequent checks (lower load,
   but slower stacking). 10 ticks = once every 0.5 seconds.
   EXAMPLES:
     5  = Frequent checks (higher load, faster stacking)
     10 = Recommended value
     20 = Infrequent checks (lower load, slower stacking)
  hopper-check-delay: 10

   max-operations-per-tick: Maximum stacking operations per tick
   RECOMMENDED: 50
   DESCRIPTION: Limits the number of operations the plugin will perform
   in a single game tick. This prevents server lags. Setting this value
   too high may cause the server to lag when many potions are being stacked simultaneously.
   EXAMPLES:
     25 = Conservative load (fewer lags, slower stacking)
     50 = Standard load
     100+ = Aggressive load (may cause lags)
  max-operations-per-tick: 50

   cache-clear-interval: Cache clearing interval in ticks
   RECOMMENDED: 1200
   DESCRIPTION: Every N ticks, the plugin clears the cache. This frees up memory.
   Set to 0 to disable cache clearing (not recommended for large servers).
   1200 ticks = 60 seconds
   EXAMPLES:
     0  = Cache is never cleared (high memory usage)
     600 = Clear cache every 30 seconds
     1200 = Clear cache every 60 seconds
     2400 = Clear cache every 120 seconds
  cache-clear-interval: 1200




