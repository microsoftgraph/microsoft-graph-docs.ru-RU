---
title: Тип ресурса Секурескореконтролстатеупдате
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0fe88741da75718b1509fd4f8015a37fcf7828bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446963"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a>Тип ресурса Секурескореконтролстатеупдате

Пространство имен: microsoft.graph

Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|assignedTo|String|Назначает элемент управления пользователю, который будет выполнять действие. |
|comment|String|Предоставляет необязательный комментарий об элементе управления. |
|state|String|Состояние элемента управления, которое можно изменить с помощью команды PATCH (например, игнорируется, thirdParty). |
|упдатедби|String|Идентификатор пользователя, который обновил состояние клиента. |
|упдатеддатетиме|DateTimeOffset|Время обновления состояния элемента управления. |

## <a name="json-representation"></a>Представление JSON
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
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "String (timestamp)"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
