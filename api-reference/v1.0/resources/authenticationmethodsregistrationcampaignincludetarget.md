---
title: тип ресурса authenticationMethodsRegistrationCampaignIncludeTarget
description: Разрешить пользователям и группам пользователей настроить целевые методы проверки подлинности.
author: mjsantani
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 51f6e1a9842c05a8fb88a92b38cb0c54fbe0d91e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994717"
---
# <a name="authenticationmethodsregistrationcampaignincludetarget-resource-type"></a>тип ресурса authenticationMethodsRegistrationCampaignIncludeTarget

Пространство имен: microsoft.graph

Представляет пользователей и группы, которые ориентированы на кампании по регистрации метода проверки подлинности. Целевыми являются только пользователи и группы, которые могут настроить метод проверки подлинности.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор объекта пользователя Azure Active Directory группы.|
|targetedAuthenticationMethod|String|Метод проверки подлинности, который пользователю предложено зарегистрировать. Значение должно быть `microsoftAuthenticator` .|
|targetType|authenticationMethodTargetType|Тип целевой цели метода проверки подлинности. Возможные значения: `user`, `group`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "targetedAuthenticationMethod": "String"
}
```
