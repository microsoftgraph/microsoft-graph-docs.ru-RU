---
title: Пределы API облачных коммуникаций в Microsoft Graph
description: Содержит сведения о пределах API облачных коммуникаций
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 0338c7b37a58da66aac75430234a4b1df56b07b1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871667"
---
# <a name="cloud-communication-api-limits-in-microsoft-graph"></a>Пределы API облачных коммуникаций в Microsoft Graph

В этой статье описываются ограничения API облачных коммуникаций. Эти пределы помогают обеспечить стабильность, надежность и безопасность платформы. Обратите внимание на то, что эти ограничения могут быть изменены в будущем. 

>**Примечание:** При достижении предельного значения попытка увеличить количество запросов API приведет к появлению HTTP `429 Error`-запроса.

| API      | Ограничения    |
| :------------- | :----------: |
|  Звонки | 10 000 звонков/мес и 100 одновременные вызовы   |
| Собрания   | 2000 собраний и пользователей в месяц |
| Присутствие (Предварительная версия)   | 2 запроса в секунду |

## <a name="see-also"></a>См. также

- [Работа с API Communications](/graph/api/resources/communications-api-overview?view=graph-rest-beta)
