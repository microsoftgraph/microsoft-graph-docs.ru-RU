---
title: " Тип ресурса Секурескореконтролстатеупдате"
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f3b69838a6de68938efac12acdfbcd4fd977c684
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810407"
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
