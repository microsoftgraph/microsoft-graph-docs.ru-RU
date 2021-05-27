---
title: тип ресурса authenticationMethodsRegistrationCampaignIncludeTarget
description: Разрешить пользователям и группам пользователей настроить целевые методы проверки подлинности.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 04dc753dd1a574bbf0b30d29b4b80375e7ab9a2c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682930"
---
# <a name="authenticationmethodsregistrationcampaignincludetarget-resource-type"></a>тип ресурса authenticationMethodsRegistrationCampaignIncludeTarget

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользователей и группы, которые ориентированы на кампании по регистрации метода проверки подлинности. Целевыми являются только пользователи и группы, которые могут настроить метод проверки подлинности.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор объекта пользователя или группы Azure AD.|
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
