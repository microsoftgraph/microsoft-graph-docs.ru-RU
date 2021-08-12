---
title: secureScoreControlStateUpdate type
description: Этот ресурс содержит историю состояния управления, обновляемого пользователем (состояния управления включают Default, Ignored, ThirdParty, Reviewed).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3268b5f537b8538173031b3367ff0e13d2873a906dfe01a5b6d6562070812d56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146365"
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
|updatedBy|String|ID пользователя, обновившего состояние клиента. |
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

