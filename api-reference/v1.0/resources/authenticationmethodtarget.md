---
title: тип ресурса authenticationMethodTarget
description: Коллекция пользователей или групп, включенная для использования метода проверки подлинности в рамках политики метода проверки подлинности.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: efb7371c68a7e9deee9e176ebf2a69e70930e4e9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126956"
---
# <a name="authenticationmethodtarget-resource-type"></a>тип ресурса authenticationMethodTarget

Пространство имен: microsoft.graph

Коллекция пользователей или групп, включенная для использования метода проверки подлинности в рамках политики метода проверки подлинности в Azure AD.


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Объект Id пользователя или группы Azure AD.|
|isRegistrationRequired|Логический|Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности.|
|targetType|authenticationMethodTargetType|Возможные значения: `user`, `group`.|
|useForSignIn|Логический|Определяет, можно ли использовать метод проверки подлинности для входов в Azure AD.|

## <a name="relationships"></a>Отношения
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
