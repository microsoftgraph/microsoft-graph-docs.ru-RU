---
title: Тип ресурса Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион
description: Представляет политику методов проверки подлинности входа с помощью пароля Майкрософт для проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ddf6a66abbf745a769a44cf323ebb245c31ecf60
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418483"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type"></a>Тип ресурса Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику методов проверки подлинности входа с помощью пароля Майкрософт для проверки подлинности. Методы проверки подлинности определяют параметры конфигурации, а также пользователей или группы, для которых разрешено использование метода проверки подлинности.

> [!NOTE]
> Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии. Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md)|[пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|Чтение свойств и связей объекта Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион.|
|[Обновление](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md)|[пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|Обновление свойств объекта Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион.|
|[Удаление](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md)|Нет|Возвращает объект Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион в конфигурацию по умолчанию.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности.|
|state|аусентикатионмесодстате|Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|инклудетаржетс|Коллекция [пассвордлессмикрософтаусентикатораусентикатионмесодтаржет](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md)|Коллекция пользователей или групп, которым разрешено использовать метод проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
