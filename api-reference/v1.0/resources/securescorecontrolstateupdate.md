---
title: secureScoreControlStateUpdate type
description: Этот ресурс содержит историю состояния управления, обновляемого пользователем (состояния управления включают Default, Ignored, ThirdParty, Reviewed).
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1e896d1b63a9b6024b62e5d7ada95049e2f717f1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084092"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate type

Пространство имен: microsoft.graph

Содержит историю состояния управления, обновляемого пользователем (состояния управления включают Default, Ignored, ThirdParty, Reviewed).

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|assignedTo|String|Назначает управление пользователю, который будет принимать действие. |
|comment|String|Предоставляет необязательный комментарий по поводу управления. |
|state|String|Состояние управления, которое можно изменить с помощью команды PATCH (например, игнорируется, thirdParty). |
|updatedBy|Строка|ID пользователя, обновившего состояние клиента. |
|updatedDateTime|DateTimeOffset|Время обновления состояния управления. |

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

