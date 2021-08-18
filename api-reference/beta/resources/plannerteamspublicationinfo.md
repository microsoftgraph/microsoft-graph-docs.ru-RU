---
title: plannerTeamsPublicationInfo type
description: Содержит подробные сведения о процессе публикации, создав планировщикTask.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 7cf298b4e9933e3019a72b0750cf01a95c2bf892609f3b601c0742eaf3b9e27d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244297"
---
# <a name="plannerteamspublicationinfo-resource-type"></a>plannerTeamsPublicationInfo type

Пространство имен: microsoft.graph

Содержит подробные сведения о процессе публикации, создав [планировщикTask.](plannertask.md) Процесс публикации создает копии задач на основе шаблона. Эти задачи создаются в нескольких планах и имеют ограниченные разрешения для пользователей; например, они не могут быть удалены, а пользователям может быть заблокировано редактирование определенных полей. Публикация используется для распределения задач по организации и централизованного отслеживания их выполнения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения этой задачи в процессе публикации. Только для чтения. |
|publicationId|Строка| Идентификатор публикации. Только для чтения.|
|publishedToPlanId|Строка|Идентификатор **планировщикаPlan** этой задачи изначально был помещен. Только для чтения. |
|publishingTeamId|Строка| Идентификатор [группы, которая](team.md) инициировала процесс публикации. Только для чтения.|
|publishingTeamName|Строка|Отображает имя команды, которая инициировала процесс публикации. Это имя отображения является только для ссылки и может не представлять самое последние имя команды. Только для чтения. |

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

