---
title: Тип ресурса Аусоризатионполици
description: Представляет политику, которая может управлять параметрами авторизации Azure Active Directory.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c20f4dad0263e9d4c931e43da99870ed022f1e58
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492232"
---
# <a name="authorizationpolicy-resource-type"></a>Тип ресурса Аусоризатионполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику, которая может управлять параметрами авторизации Azure Active Directory. Это одноэлементный экземпляр, который наследуется от базового типа политики и всегда существует для клиента. 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Аусоризатионполици](../api/authorizationpolicy-get.md) | [аусоризатионполици](authorizationpolicy.md) | Чтение объекта Аусоризатионполици. |
| [Обновление Аусоризатионполици](../api/authorizationpolicy-update.md) | Нет | Обновление объекта Аусоризатионполици. |

## <a name="properties"></a>Свойства  
| Свойство | Тип | Описание | 
|-|-|-|
|id|String| Идентификатор политики авторизации. Обязательный элемент. Только для чтения.| 
|displayName|Строка| Отображаемое имя для этой политики. |  
|description|String| Описание этой политики.|  
|гуестусерролеид|Guid| Представляет templateId роли для роли, которая должна быть выделена пользователю "гость". Обратитесь к [списку унифиедроледефинитионс](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) , чтобы найти список доступных шаблонов ролей. В настоящее время поддерживаются следующие роли: пользователь (a0b1b346-4d3e-4e8b-98f8-753987be4970), гость (10dae51f-b6af-4016-8d66-8c2a99b929b3) и незащищенный гостевой пользователь (2af84b1e-32c8-42b7-82bc-daa82404023b). | 
|енабледпревиевфеатурес|Коллекция (String)| Список компонентов, включенных для закрытой предварительной версии в клиенте. | 
|блоккмсолповершелл|Логический| Чтобы отключить использование MSOL PowerShell, установите для этого свойства значение true. Если задано значение true, также будет отключен доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell. Это не повлияет на Azure AD Connect или Microsoft Graph. | 


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authorizationPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
   "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "enabledPreviewFeatures": "[String]",
  "guestUserRoleId": "Guid",
  "blockMsolPowerShell": true 
}
```
