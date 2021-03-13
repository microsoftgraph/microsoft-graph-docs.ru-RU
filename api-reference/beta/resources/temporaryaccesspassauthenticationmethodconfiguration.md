---
title: temporaryAccessPassAuthenticationMethodConfiguration resource type
description: Представляет политику методов проверки подлинности с временным пропуском доступа.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: ccdb139beff0019e9cad3f6c4e223369f9c6e66e
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760969"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>temporaryAccessPassAuthenticationMethodConfiguration resource type
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику методов проверки подлинности с временным пропуском доступа. Политика методов проверки подлинности определяет параметры конфигурации и пользователей или групп, которым включен метод проверки подлинности.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[получение](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md);|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Ознакомьтесь с свойствами и отношениями объекта **temporaryaccesspassauthenticationmethodconfiguration.**|
|[Update](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Обновление свойств объекта **temporaryaccesspassauthenticationmethodconfiguration.**|
|[Удаление](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|Нет|Возвращает объект **temporaryaccesspassauthenticationmethodconfiguration** к конфигурации по умолчанию.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности.|
|minimumLifetimeInMinutes|Целое|Минимальный срок службы в минутах для любого временногоAccessPass, созданного в клиенте. Значение может быть от 10 до 43200 минут (эквивалентно 30 дням).|
|maximumLifetimeInMinutes|Целое|Максимальный срок службы в минутах для любого временногоAccessPass, созданного в клиенте. Значение может быть от 10 до 43200 минут (эквивалентно 30 дням).|
|defaultLifetimeInMinutes|int|Срок службы по умолчанию в минутах для временногоAccessPass. Значение может быть между минимумомLifetimeInMinutes и maximumLifetimeInMinutes.|
|defaultLength|int|Длина по умолчанию в символах временногоAccessPass составляет от 8 до 48 символов.|
|isUsableOnce|Boolean   |Если все пропуска в клиенте будут ограничены `true` одновековой помощью. Если в клиенте может быть создано однократное использование или `false` многократное использование времени.|
|state|authenticationMethodState|Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|includeTargets|[коллекция authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
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
