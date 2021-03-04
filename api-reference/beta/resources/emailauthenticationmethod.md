---
title: тип ресурса emailAuthenticationMethod
description: Представление адреса электронной почты, зарегистрированного пользователем. Электронная почта — это метод проверки подлинности, доступный только для сброса пароля самообслуживления (SSPR)
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a24a67fdb4bcc054036de26ba235bf4bac0f2da2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440369"
---
# <a name="emailauthenticationmethod-resource-type"></a>тип ресурса emailAuthenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление адреса электронной почты, зарегистрированного пользователем. Электронная почта — это метод проверки подлинности, доступный только для сброса пароля самообслуживления (SSPR). У пользователей может быть только один метод проверки подлинности электронной почты.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список](../api/emailauthenticationmethod-list.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md) collection|Извлечение списка электронной почты пользователяAuthenticationMethods. У пользователей может быть только один метод проверки подлинности электронной почты.|
|[Создание](../api/emailauthenticationmethod-post.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Создайте объект электронной почты пользователяMethods.|
|[получение](../api/emailauthenticationmethod-get.md);|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Извлечение свойств объекта электронной почты пользователяAuthenticationMethod.|
|[Обновление](../api/emailauthenticationmethod-update.md)|[emailAuthenticationMethod](../resources/emailauthenticationmethod.md)|Обновление свойств объекта электронной почты пользователяMethods.|
|[удаление](../api/emailauthenticationmethod-delete.md);|Нет|Удаление объекта электронной почты пользователяAuthenticationMethod.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор адреса электронной почты, зарегистрированного для этого пользователя.|
|emailAddress|String|Адрес электронной почты, зарегистрированный для этого пользователя.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethod",
  "id": "String (identifier)",
  "emailAddress": "String"
}
```

