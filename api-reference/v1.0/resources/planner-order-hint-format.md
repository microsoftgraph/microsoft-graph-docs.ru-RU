---
title: Использование подсказок порядка в Планировщике
description: '`)'
author: TarkanSevilmis
ms.localizationpriority: medium
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: ff33069f1427700d0c60bf7300052eb127c37e34
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044435"
---
# <a name="using-order-hints-in-planner"></a>Использование подсказок порядка в Планировщике

Пространство имен: microsoft.graph

Порядок сортировки объектов в Планировщике определяется подсказками порядка. Значения подсказок порядка — строки. Чтобы определить порядок следования элементов, клиенты могут сортировать эти строки по порядковому значению символов в них. Сравниваются символы с начала строки и до тех пор, пока не будет обнаружена разница в порядковом значении символов, либо пока одна из строк не закончится — в таком случае короткая строка будет расположена выше длинной. Значения могут содержать любой символ с порядковым номером от 32 (пробел) до 126 (`~`).

Например, элемент с подсказкой порядка `a` (порядковый номер 97) будет размещен выше элемента с подсказкой порядка `z` (порядковый номер 122). Элемент с подсказкой порядка `abc` (порядковые номера 97, 98, 99) будет размещен выше элемента с подсказкой порядка `abd` (порядковые номера 97, 98, 100). Элемент с подсказкой порядка `a` будет размещен выше элемента с подсказкой порядка `ab`, так как все существующие знаки совпадают, а `a` короче.

Значения для всех подсказок порядка вычисляет служба. Клиент может изменить расположение элементов, указав для определенного элемента подсказку порядка, которая переместит его между двумя указанными элементами. Для этого необходимо задать такое значение подсказки порядка: `<previous order hint> <next order hint>!` (где `<previous order hint>` — значение, которое будет заменено подсказкой порядка элемента, расположенного перед целевым местом, а `<next order hint>` — значение, которое будет заменено подсказкой порядка элемента, расположенного после целевого места). Между этими значениями ставится пробел, а в конце значения указывается суффикс `!`. Если предыдущий или предшествующий элемент не существует, вместо него следует указать пустую строку. Значение также можно составить на основе проведенных ранее расчетов. Кроме того, клиент может использовать это значение для сортировки элементов в порядке возвращения подсказок порядка. После того как клиент отправит эти значения в обновлении, служба вычислит короткое значение, которое поможет выполнить сортировку.

**Обратите внимание**: в следующих примерах значения подсказки порядка приведены в одинарных кавычках (`'`) для наглядности, однако кавычки не являются частью данных и не должны отправляться в службу.
 
Рассмотрим следующий список подсказок порядка сортировки.

1. Элемент 1 (подсказка порядка: `'5637'`).
2. Элемент 2 (подсказка порядка: `'adhg'`).

Расположите элемент 3 перед элементом 1, а затем поместите элемент 4 между элементами 1 и 2. Затем поместите элемент 5 после элемента 2. В клиенте будут созданы следующие подсказки порядка. 

1. Элемент 3 (подсказка порядка: `' 5637!'`).
2. Элемент 1 (подсказка порядка: `'5637'`).
3. Элемент 4 (подсказка порядка: `'5637 adhg!'`).
4. Элемент 2 (подсказка порядка: `'adhg'`).
5. Элемент 5 (подсказка порядка: `'adhg !'`).

Затем переместите элемент 1 в конец списка. Будут созданы следующие подсказки.

1. Элемент 3 (подсказка порядка: `' 5637!'`).
2. Элемент 4 (подсказка порядка: `'5637 adhg!'`).
3. Элемент 2 (подсказка порядка: `'adhg'`).
4. Элемент 5 (подсказка порядка: `'adhg !'`).
5. Элемент 1 (подсказка порядка: `'adhg ! !'`).

Поместите элемент 5 между элементами 3 и 4. Будут созданы следующие подсказки.

1. Элемент 3 (подсказка порядка: `' 5637!'`).
2. Элемент 5 (подсказка порядка: `' 5637! 5637 adhg!!'`).
3. Элемент 4 (подсказка порядка: `'5637 adhg!'`).
4. Элемент 2 (подсказка порядка: `'adhg'`).
5. Элемент 1 (подсказка порядка: `'adhg ! !'`).

После того как эти изменения значений подсказок порядка будут отправлены в службу с помощью запросов Patch, служба рассчитает правильные значения, соответствующие порядку следования, предусмотренному клиентом. Клиент может получить эти значения немедленно, если в запросах `PATCH` указана настройка `return=representation`. Значения для указанного выше случая могут выглядеть следующим образом (фактические значения могут отличаться). 

1. Элемент 3 (подсказка порядка: `'432b'`).
2. Элемент 5 (подсказка порядка: `'6F"#'`).
3. Элемент 4 (подсказка порядка: `'7A$6'`).
4. Элемент 2 (подсказка порядка: `'adhg'`).
5. Элемент 1 (подсказка порядка: `'de5%'`).

Для создания первого элемента в списке можно использовать значение подсказки порядка `!`, так как ни предыдущий, ни следующий элемент в таком случае не существуют. Но это не обязательно, так как служба автоматически создаст значения для всех подсказок порядка, если они не указаны во время создания элемента. В следующем примере показаны подсказки порядка, которые следует использовать для добавления элементов в пустой список.
Добавьте первый элемент:

1. Элемент 1 (подсказка порядка: `' !'`).

Добавьте второй элемент вверху:

1. Элемент 2 (подсказка порядка: `'  !!'`).
2. Элемент 1 (подсказка порядка: `' !'`).

Добавьте третий элемент внизу.

1. Элемент 2 (подсказка порядка: `'  !!'`).
2. Элемент 1 (подсказка порядка: `' !'`).
3. Элемент 3 (подсказка порядка: `' ! !'`).








