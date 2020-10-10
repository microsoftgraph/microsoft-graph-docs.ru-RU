---
title: Тип ресурса Емаилаусентикатионмесод
description: Представление адреса электронной почты, зарегистрированного для пользователя. Электронная почта — способ проверки подлинности, доступный только для самостоятельного сброса пароля (SSPR)
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6dde3c9a859f2527241b66c0172d6b5dd877aac4
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418475"
---
# <a name="emailauthenticationmethod-resource-type"></a>Тип ресурса Емаилаусентикатионмесод

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление адреса электронной почты, зарегистрированного для пользователя. Электронная почта — это способ проверки подлинности, доступный только для самостоятельного сброса пароля (SSPR). У пользователей может быть только один способ проверки подлинности электронной почты.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление](../api/emailauthenticationmethod-list.md)|Коллекция [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md)|Получение списка Емаилаусентикатионмесодс пользователя. У пользователей может быть только один способ проверки подлинности электронной почты.|
|[Создание](../api/emailauthenticationmethod-post.md)|[емаилаусентикатионмесод](../resources/emailauthenticationmethod.md)|Создание объекта Емаилмесодс пользователя.|
|[Получение](../api/emailauthenticationmethod-get.md)|[емаилаусентикатионмесод](../resources/emailauthenticationmethod.md)|Получение свойств объекта Емаилаусентикатионмесод пользователя.|
|[Обновление](../api/emailauthenticationmethod-update.md)|[емаилаусентикатионмесод](../resources/emailauthenticationmethod.md)|Обновление свойств объекта Емаилмесодс пользователя.|
|[Удаление](../api/emailauthenticationmethod-delete.md)|Нет|Удаление объекта Емаилаусентикатионмесод пользователя.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор адреса электронной почты, зарегистрированный для этого пользователя.|
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

