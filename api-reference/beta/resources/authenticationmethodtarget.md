---
title: Тип ресурса authenticationMethodTarget
description: Коллекция пользователей или групп, которые могут использовать метод проверки подлинности в рамках политики методов проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 19f8fb774ad0a60fa74d2c27655ee1174e0989af
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135452"
---
# <a name="authenticationmethodtarget-resource-type"></a>Тип ресурса authenticationMethodTarget

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция пользователей или групп, которые могут использовать метод проверки подлинности в рамках политики методов проверки подлинности в Azure AD.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ИД объекта пользователя или группы Azure AD.|
|isRegistrationRequired|Boolean|Определяет, принудительно ли зарегистрирует метод проверки подлинности для пользователя.|
|targetType|authenticationMethodTargetType|Возможные значения: `user`, `group`.|
|useForSignIn|Boolean|Определяет, можно ли использовать метод проверки подлинности для входов в Azure AD.|

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
