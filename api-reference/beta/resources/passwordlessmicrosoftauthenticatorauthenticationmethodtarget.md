---
title: Тип ресурса Пассвордлессмикрософтаусентикатораусентикатионмесодтаржет
description: Коллекция пользователей или групп, для которых используется политика методов проверки подлинности при входе в систему без пароля.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a26a8fe76da954d3dc44a238665954539df0fa72
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418482"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type"></a>Тип ресурса Пассвордлессмикрософтаусентикатораусентикатионмесодтаржет

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Набор пользователей или групп, для которых используется политика проверки подлинности входа на телефон, не поддерживающий пароль для проверки подлинности (Майкрософт). /Ресаурцес/пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион.МД) в Azure AD.

> [!NOTE]
> Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии. Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор объекта пользователя или группы Azure AD.|
|исрегистратионрекуиред|Boolean|Определяет, применяется ли пользователь для регистрации метода проверки подлинности.|
|шовнконтекст|аусентикатораппконтексттипе|Возможные значения: `location`, `app`.|
|targetType|аусентикатионмесодтаржеттипе|Возможные значения: `user`, `group`.|
|усефорсигнин|Boolean|Определяет, можно ли использовать метод проверки подлинности для входа в Azure AD.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String"
}
```
