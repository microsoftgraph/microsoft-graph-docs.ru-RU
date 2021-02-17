---
title: Тип ресурса temporaryAccessPassAuthenticationMethod
description: Представляет временный проход доступа, зарегистрированный для пользователя.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e7e0afc084106face2ef8726f3273638d1a8eec0
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272653"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a>Тип ресурса temporaryAccessPassAuthenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет временный доступ, зарегистрированный для пользователя. Временный пароль — это ограниченный по времени пароль, который служит в качестве надежных учетных данных и позволяет вводить учетные данные без пароля.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список](../api/temporaryaccesspassauthenticationmethod-list.md)|[коллекция temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Получить список временных **объектовAccessPassAuthenticationMethod** пользователя и их свойств. У пользователей может быть только один метод проверки подлинности с временным доступом.|
|[Создание](../api/temporaryaccesspassauthenticationmethod-post.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Создание объекта **temporaryAccessPassAuthenticationMethod** пользователя.|
|[получение](../api/temporaryaccesspassauthenticationmethod-get.md);|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Извлечение свойств временного объекта **UserAccessPassAuthenticationMethod.**||
|[удаление](../api/temporaryaccesspassauthenticationmethod-delete.md);|Нет|Удаление объекта **temporaryAccessPassAuthenticationMethod** пользователя.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор временного доступа, зарегистрированного для этого пользователя.|
|temporaryAccessPass|String|ВременныйaccessPass, используемый для проверки подлинности. Возвращается только при создании нового временногоaccessPass; возвращается как NULL с get.|
|createdDateTime|DateTimeOffset|Дата и время создания temporaryAccessPass.|
|startDateTime|DateTimeOffset|Дата и время, когда временныйaccessPass становится доступным для использования.|
|lifetimeInMinutes|Int32|Время существования temporaryAccessPass в минутах, начиная с startDateTime. Минимум 10, максимум 43200 (эквивалентно 30 дням).|
|isUsableOnce|Boolean|Определяет, ограничен ли проход одновейным использованием. Если этот проход можно использовать один раз; если этот проход можно использовать несколько раз в течение `true` `false` срока действия temporaryAccessPass.|
|isUsable|Boolean|Состояние метода проверки подлинности, который указывает, может ли пользователь в настоящее время его указать.|
|methodUsabilityReason|String|Сведения о состоянии использования (isUsable). Причины могут быть: `enabledByPolicy` , , , , `disabledByPolicy` `expired` `notYetValid` `oneTimeUsed` .|


## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "id": "String (identifier)",
  "temporaryAccessPass": "String",
  "createdDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "lifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean",
  "isUsable": "Boolean",
  "methodUsabilityReason": "String"
}
```
