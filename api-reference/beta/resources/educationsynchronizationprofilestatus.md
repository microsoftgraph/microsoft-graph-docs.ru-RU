---
title: Тип ресурса Едукатионсинчронизатионпрофилестатус
description: 'Представляет состояние синхронизации профиля School Data Synchronization. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0e792b55cddaee3069eaaf53cc9dce68aae041e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979555"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a>Тип ресурса Едукатионсинчронизатионпрофилестатус

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние синхронизации профиля School Data [Synchronization](educationsynchronizationprofile.md).

> **Примечание:** Обновление **едукатионсинчронизатионпрофилестатус** может быть отложено из-за асинхронной обработки фоновой синхронизации.

## <a name="methods"></a>Методы

| Метод                                                                      | Возвращаемый тип                               | Описание                                              |
| :-------------------------------------------------------------------------- | :---------------------------------------- | :------------------------------------------------------- |
| [Получение состояния синхронизации](../api/educationsynchronizationprofilestatus-get.md) | **едукатионсинчронизатионпрофилестатус** | Возврат состояния определенного профиля синхронизации. |

## <a name="properties"></a>Свойства

| Свойство                    | Тип                           | Описание                                                                                                              |
| :-------------------------- | :----------------------------- | :----------------------------------------------------------------------------------------------------------------------- |
| id                          | String                         | Уникальный идентификатор ресурса. (только для чтения)                                                                      |
| status                      | едукатионсинчронизатионстатус | Состояние синхронизации. Возможные значения: `paused` ,, `inProgress` , `success` , `error` `quarantined` , `validationError` . |
| ластсинчронизатиондатетиме | DateTimeOffset                 | Представляет время, в течение которого последние изменения были просмотрены в каталоге.                                        |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
  "id": "String",
  "status": { "@odata.type": "microsoft.graph.educationSynchronizationStatus" },
  "lastSynchronizationDateTime": "DateTimeOffset"
}
```


