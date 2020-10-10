---
title: Тип ресурса Аусентикатионмесодтаржет
description: Коллекция пользователей или групп, которые включены для использования метода проверки подлинности в рамках политики метода проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7112249f618bbda31eddeb07967d201c8b641075
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418478"
---
# <a name="authenticationmethodtarget-resource-type"></a>Тип ресурса Аусентикатионмесодтаржет

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция пользователей или групп, которые включены для использования метода проверки подлинности в рамках политики метода проверки подлинности в Azure AD.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор объекта пользователя или группы Azure AD.|
|исрегистратионрекуиред|Boolean|Определяет, применяется ли пользователь для регистрации метода проверки подлинности.|
|targetType|аусентикатионмесодтаржеттипе|Возможные значения: `user`, `group`.|
|усефорсигнин|Boolean|Определяет, можно ли использовать метод проверки подлинности для входа в Azure AD.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodTarget",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean"
}
```
