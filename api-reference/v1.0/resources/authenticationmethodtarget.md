---
title: тип ресурса authenticationMethodTarget
description: Коллекция пользователей или групп, включенная для использования метода проверки подлинности в рамках политики метода проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ff64481140678055f8bab28f2ff4aa443689b11eec8a14d17648cf800a179996
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124565"
---
# <a name="authenticationmethodtarget-resource-type"></a>тип ресурса authenticationMethodTarget

Пространство имен: microsoft.graph

Коллекция пользователей или групп, включенная для использования метода проверки подлинности в рамках политики метода проверки подлинности в Azure AD.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Объект Id пользователя или группы Azure AD.|
|isRegistrationRequired|Логическое|Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности.|
|targetType|authenticationMethodTargetType|Возможные значения: `user`, `group`.|
|useForSignIn|Логическое|Определяет, можно ли использовать метод проверки подлинности для входов в Azure AD.|

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
