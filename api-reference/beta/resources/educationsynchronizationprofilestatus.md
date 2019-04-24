---
title: Тип ресурса Едукатионсинчронизатионпрофилестатус
description: 'Представляет состояние синхронизации профиля School Data Synchronization. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 12908f6454cb27c673935f1e4c64c921b7ff0dcd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507095"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>Тип ресурса Едукатионсинчронизатионпрофилестатус

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние синхронизации профиля School Data [Synchronization](educationsynchronizationprofile.md). 

> **Примечание:** Обновление **едукатионсинчронизатионпрофилестатус** может быть отложено из-за асинхронной обработки фоновой синхронизации.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:-|:-|:-|
| [Получение состояния синхронизации](../api/educationsynchronizationprofilestatus-get.md) | **Едукатионсинчронизатионпрофилестатус** | Возврат состояния определенного профиля синхронизации. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-|:-|:-|
| **status** | Едукатионсинчронизатионстатус | Состояние синхронизации. Возможные `paused`значения:, `inProgress`, `success`, `error`, `quarantined`,. `validationError` |
| **Ластсинчронизатиондатетиме** | DateTimeOffset | Представляет время, в течение которого последние изменения были просмотрены в каталоге.  |

## <a name="json-representation"></a>Представление JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationprofilestatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
