---
title: Тип ресурса plannerTeamsPublicationInfo
description: Содержит подробные сведения о процессе публикации, который создал plannerTask.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9db73bb5a914a848f3e19e079321681b22510e8e
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883259"
---
# <a name="plannerteamspublicationinfo-resource-type"></a>Тип ресурса plannerTeamsPublicationInfo

Пространство имен: microsoft.graph

Содержит подробные сведения о процессе публикации, который создал [plannerTask.](plannertask.md) Процесс публикации создает копии задач на основе шаблона. Эти задачи создаются в нескольких планах и имеют ограниченные разрешения для пользователей; Например, их нельзя удалить, а пользователям может быть заблокировано редактирование определенных полей. Публикация используется для распространения задач по всей организации и централизованного отслеживания их хода выполнения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения этой задачи в процессе публикации. Только для чтения. |
|publicationId|Строка| Идентификатор публикации. Только для чтения.|
|publishedToPlanId|Строка|Идентификатор **планировщика,** в который изначально была помещена эта задача. Только для чтения. |
|publishingTeamId|Строка| Идентификатор команды, [которая](team.md) инициировала процесс публикации. Только для чтения.|
|publishingTeamName|Строка|Отображаемое имя команды, которая инициировала процесс публикации. Это отображаемого имени только для ссылки и может не представлять наиболее последние имена команды. Только для чтения. |

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

