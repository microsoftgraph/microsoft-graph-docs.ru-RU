---
title: тип ресурса authenticationMethodTarget
description: Коллекция пользователей или групп, включенная для использования метода проверки подлинности в рамках политики метода проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4c9265fa359e5b60da6f8e36c13d1a4340ba6d1a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964983"
---
# <a name="authenticationmethodtarget-resource-type"></a>тип ресурса authenticationMethodTarget

Пространство имен: microsoft.graph

Коллекция пользователей или групп, включенная для использования метода проверки подлинности в рамках политики метода проверки подлинности в Azure AD.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Объект Id пользователя или группы Azure AD.|
|isRegistrationRequired|Boolean|Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности.|
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
