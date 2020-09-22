---
title: " Тип ресурса Секурескореконтролстатеупдате"
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: d1678d4fe77ade738f7eb298221772ced381e2d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087553"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>Тип ресурса Секурескореконтролстатеупдате
Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).

|Свойство |Тип |Описание |
|:--|:--|:--|
|assignedTo | string | Назначение элемента управления пользователю, который будет выполнять действие |
|comment | string | Предоставляет необязательный комментарий об элементе управления |
|состояние | string | Состояние элемента управления можно изменить с помощью команды PATCH (например, игнорируется, thirdParty и т. д.) |
|упдатедби | string |Идентификатор пользователя, который обновил состояние клиента |
|упдатеддатетиме | DateTimeOffset |Время обновления состояния элемента управления |
 ## <a name="json-representation"></a>Представление в формате JSON
 Ниже указано представление ресурса в формате JSON.
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "string",
  "state": "string",
  "updatedBy": "string",
  "updatedDateTime": "DateTimeOffset"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


