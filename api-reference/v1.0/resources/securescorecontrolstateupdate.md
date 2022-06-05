---
title: Тип ресурса secureScoreControlStateUpdate
description: Этот ресурс содержит журнал состояний элементов управления, обновленных пользователем (состояния элементов управления включают Default, Ignored, ThirdParty, Reviewed).
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5c91abead33b725862242e2f8864371729668583
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898898"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a>Тип ресурса secureScoreControlStateUpdate

Пространство имен: microsoft.graph

Содержит журнал состояний элементов управления, обновленных пользователем (состояния элементов управления включают Default, Ignored, ThirdParty, Reviewed).

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|assignedTo|String|Назначает элемент управления пользователю, который будет выполнять действие. |
|comment|String|Предоставляет необязательный комментарий к элементу управления. |
|state|String|Состояние элемента управления, которое можно изменить с помощью команды PATCH (например, игнорируется, thirdParty). |
|updatedBy|Строка|Идентификатор пользователя, который обновил состояние клиента. |
|updatedDateTime|DateTimeOffset|Время обновления состояния элемента управления. |

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

