---
title: Тип ресурса temporaryAccessPassAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности для временного прохода доступа.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9edb4038180a96d6878fcaf6770728a1befbca19
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272650"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>Тип ресурса temporaryAccessPassAuthenticationMethodConfiguration
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику методов проверки подлинности для временного прохода доступа. Политика методов проверки подлинности определяет параметры конфигурации и пользователей или группы, которым включено использование метода проверки подлинности.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[получение](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md);|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Чтение свойств и связей объекта **temporaryaccesspassauthenticationmethodconfiguration.**|
|[обновление](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md).|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Обновление свойств объекта **temporaryaccesspassauthenticationmethodconfiguration.**|
|[удаление](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md);|Нет|Возвращает объект **temporaryaccesspassauthenticationmethodconfiguration** в конфигурацию по умолчанию.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики метода проверки подлинности.|
|minimumLifetimeInMinutes|Целое|Минимальный срок жизни (в минутах) для всех временныхaccessPass, созданных в клиенте. Значение может быть от 10 до 43200 минут (эквивалентно 30 дням).|
|maximumLifetimeInMinutes|Целое|Максимальный срок действия в минутах для всех временныхaccessPass, созданных в клиенте. Значение может быть от 10 до 43200 минут (эквивалентно 30 дням).|
|defaultLifetimeInMinutes|int|Время жизни по умолчанию (в минутах) для temporaryAccessPass. Значение может быть между minimumLifetimeInMinutes и maximumLifetimeInMinutes.|
|defaultLength|int|Длина по умолчанию (в символах) временногоaccessPass от 8 до 48 символов.|
|isUsableOnce|Boolean   |Если `true` все проходы в клиенте будут ограничены одновейным использованием. Если , передается клиент может быть создан для `false` однократного или многократного использования.|
|state|authenticationMethodState|Возможные значения: `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|includeTargets|[Коллекция authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Коллекция пользователей или групп, которым включен метод проверки подлинности.|

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
