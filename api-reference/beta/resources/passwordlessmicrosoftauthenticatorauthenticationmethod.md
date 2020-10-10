---
title: Тип ресурса Пассвордлессмикрософтаусентикатораусентикатионмесод
description: Представление метода входа с помощью пароля Майкрософт для проверки подлинности, зарегистрированного для пользователя.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b34b807106591390198c58d26d7804dc6ada5460
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418486"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethod-resource-type"></a>Тип ресурса Пассвордлессмикрософтаусентикатораусентикатионмесод

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление метода входа с помощью пароля Майкрософт для проверки подлинности, зарегистрированного для пользователя.

> [!NOTE]
> Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии. Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.


## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md)|Коллекция [пассвордлессмикрософтаусентикатораусентикатионмесод](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|Получение списка объектов Пассвордлессмикрософтаусентикатораусентикатионмесод пользователя и их свойств.|
|[Получение](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md)|[пассвордлессмикрософтаусентикатораусентикатионмесод](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|Чтение свойств и связей объекта Пассвордлессмикрософтаусентикатораусентикатионмесод пользователя.|
|[Удаление](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md)|Нет|Удаляет объект Пассвордлессмикрософтаусентикатораусентикатионмесод пользователя.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор метода проверки подлинности.|
|displayName|String|Отображаемое имя мобильного устройства, заданное пользователем.|
|креатиондатетиме|DateTimeOffset|Временная метка, когда этот метод был зарегистрирован для пользователя.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)"
}
```

