---
title: plannerTeamsPublicationInfo type
description: Содержит подробные сведения о процессе публикации, создав планировщикTask.
author: TarkanSevilmis
ms.localizationpriority: medium
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 77441184468a87e6d12d32adedc98a26c228db68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115046"
---
# <a name="plannerteamspublicationinfo-resource-type"></a>plannerTeamsPublicationInfo type

Пространство имен: microsoft.graph

Содержит подробные сведения о процессе публикации, создав [планировщикTask.](plannertask.md) Процесс публикации создает копии задач на основе шаблона. Эти задачи создаются в нескольких планах и имеют ограниченные разрешения для пользователей; например, они не могут быть удалены, а пользователям может быть заблокировано редактирование определенных полей. Публикация используется для распределения задач по организации и централизованного отслеживания их выполнения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения этой задачи в процессе публикации. Только для чтения. |
|publicationId|String| Идентификатор публикации. Только для чтения.|
|publishedToPlanId|String|Идентификатор **планировщикаPlan** этой задачи изначально был помещен. Только для чтения. |
|publishingTeamId|String| Идентификатор [группы, которая](team.md) инициировала процесс публикации. Только для чтения.|
|publishingTeamName|String|Отображает имя команды, которая инициировала процесс публикации. Это имя отображения является только для ссылки и может не представлять самое последние имя команды. Только для чтения. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerTeamsPublicationInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTeamsPublicationInfo",
  "publicationId": "String",
  "publishingTeamId": "String",
  "publishingTeamName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "publishedToPlanId": "String"
}
```

