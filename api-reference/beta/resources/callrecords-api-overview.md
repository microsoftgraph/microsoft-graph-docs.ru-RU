---
title: Работа с API записей звонков в Microsoft Graph
description: API записей звонков Microsoft Graph позволяет извлекать данные об использовании и диагностике для звонков и собраний по сети в вашей организации.
author: williamlooney
doc_type: conceptualPageType
ms.prod: cloud-communications
ms.localizationpriority: high
ms.openlocfilehash: dafb08c19ad84a23b5954687c4f18ff091cfc3ab
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695464"
---
# <a name="working-with-the-call-records-api-in-microsoft-graph"></a>Работа с API записей звонков в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Записи звонков содержат сведения об использовании и диагностике, касающиеся звонков и собраний по сети в вашей организации при применении Microsoft Teams или Skype для бизнеса. Вы можете использовать API записей звонков, чтобы подписаться на записи звонков и искать их по идентификаторам.

API записи звонков задается в подпространстве имен OData, `microsoft.graph.callRecords`.

## <a name="key-resource-types"></a>Ключевые типы ресурсов

| Ресурс | Методы |
| :-- | :-- |
| [callRecord](callrecords-callrecord.md) | [Получение callRecord](../api/callrecords-callrecord-get.md) |
| [session](callrecords-session.md) | [Получение callRecord](../api/callrecords-callrecord-get.md)<br />[Перечисление сеансов](../api/callrecords-session-list.md) |
| [segment](callrecords-segment.md) | [Получение callRecord](../api/callrecords-callrecord-get.md)<br />[Перечисление сеансов](../api/callrecords-session-list.md) |
| [pstnCallLogRow](callrecords-pstncalllogrow.md)|[Получение pstnCallLogRow](../api/callrecords-callrecord-getpstncalls.md) |
| [directRoutingLogRow](callrecords-directroutinglogrow.md) | [Получение directRoutingLogRow](../api/callrecords-callrecord-getdirectroutingcalls.md)|

## <a name="call-record-structure"></a>Структура записи звонка

Объект [callRecord](callrecords-callrecord.md) представляет один одноранговый звонок или групповой звонок между несколькими участниками, иногда называемый собранием по сети.

Одноранговый звонок содержит один объект [session](callrecords-session.md)между двумя участниками звонка. Групповые звонки содержат один или несколько объектов **session**. В групповом звонке каждый объект **session** находится между участником и конечной точкой службы.

Каждый объект **session** содержит один или несколько объектов [segment](callrecords-segment.md). Объект **segment** представляет ссылку на носитель между двумя [конечными точками](callrecords-endpoint.md). В большинстве звонков для каждого объекта **session** будет существовать только один объект **segment**, но иногда может иметься одна или несколько промежуточных **конечных точек**.

![Изображение структуры данных, представляющей полную запись звонка](/graph/images/callrecords-structure.png)

На схеме выше числа обозначают допустимое количество дочерних элементов каждого типа. Например, связь 1..N между **callRecord** и **session** означает, что один экземпляр **callRecord** может содержать один или несколько экземпляров **session**. Таким же образом, связь 1..N между **segment** и **media** означает, что один экземпляр **segment** может содержать один или несколько потоков [media](callrecords-media.md).

## <a name="see-also"></a>См. также

- [Подписки веб-перехватчиков](/graph/api/resources/webhooks?view=graph-rest-beta)


