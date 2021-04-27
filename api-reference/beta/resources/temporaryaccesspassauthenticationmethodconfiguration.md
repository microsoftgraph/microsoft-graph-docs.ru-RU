---
title: temporaryAccessPassAuthenticationMethodConfiguration resource type
description: Представляет политику методов проверки подлинности с временным пропуском доступа.
author: inbarckms
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 5cac99576931ff15636df6f69b548ecfb53c01f3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052546"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>temporaryAccessPassAuthenticationMethodConfiguration resource type
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику методов проверки подлинности с временным пропуском доступа. Политика методов проверки подлинности определяет параметры конфигурации и пользователей или групп, которым включен метод проверки подлинности.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[получение](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md);|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Ознакомьтесь с свойствами и отношениями объекта **temporaryaccesspassauthenticationmethodconfiguration.**|
|[Обновление](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Обновление свойств объекта **temporaryaccesspassauthenticationmethodconfiguration.**|
|[удаление](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md);|Нет|Возвращает объект **temporaryaccesspassauthenticationmethodconfiguration** к конфигурации по умолчанию.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности.|
|minimumLifetimeInMinutes|Целое|Минимальный срок службы в минутах для любого временногоAccessPass, созданного в клиенте. Значение может быть от 10 до 43200 минут (эквивалентно 30 дням).|
|maximumLifetimeInMinutes|Целое|Максимальный срок службы в минутах для любого временногоAccessPass, созданного в клиенте. Значение может быть от 10 до 43200 минут (эквивалентно 30 дням).|
|defaultLifetimeInMinutes|int|Срок службы по умолчанию в минутах для временногоAccessPass. Значение может быть между минимумомLifetimeInMinutes и maximumLifetimeInMinutes.|
|defaultLength|int|Длина по умолчанию в символах временногоAccessPass составляет от 8 до 48 символов.|
|isUsableOnce|Логический   |Если все пропуска в клиенте будут ограничены `true` одновековой помощью. Если в клиенте может быть создано однократное использование или `false` многократное использование времени.|
|state|authenticationMethodState|Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|includeTargets|[коллекция authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.|

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.

``` json
{
  "@odata.type": "#microsoft.authMethodPolicy.temporaryAccessPassAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "defaultLifetimeInMinutes": "Integer",
  "defaultLength": "Integer",
  "minimumLifetimeInMinutes": "Integer",
  "maximumLifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean"
},
"includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
