---
title: temporaryAccessPassAuthenticationMethod type
description: Представляет временный пропуск доступа, зарегистрированный пользователю.
author: inbarckms
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1d4b084bdb66215bb60990c62dbfa6682bafe0b1
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546947"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a>temporaryAccessPassAuthenticationMethod type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет временный пропуск доступа, зарегистрированный пользователю. Временный пропуск доступа — это ограниченный по времени пароль, который служит прочным учетным данным и позволяет использовать учетные данные без паролей.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список](../api/temporaryaccesspassauthenticationmethod-list.md)|[коллекция temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Извлечение списка временных **объектовAccessPassAuthenticationMethod** и их свойств. У пользователей может быть только один метод проверки подлинности временных пропусков доступа.|
|[Создание](../api/temporaryaccesspassauthenticationmethod-post.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Создайте временный **объектAccessPassAuthenticationMethod.**|
|[получение](../api/temporaryaccesspassauthenticationmethod-get.md);|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Извлечение свойств объекта **temporaryAccessPassAuthenticationMethod** пользователя.|
|[удаление](../api/temporaryaccesspassauthenticationmethod-delete.md);|Нет|Удаление объекта **temporaryAccessPassAuthenticationMethod** пользователя.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор временного пропуска доступа, зарегистрированного для этого пользователя.|
|temporaryAccessPass|String|Для проверки подлинности используется temporaryAccessPass. Возвращается только при создании нового временногоAccessPass; возвращается как NULL с GET.|
|createdDateTime|DateTimeOffset|Дата и время создания временногоAccessPass.|
|startDateTime|DateTimeOffset|Дата и время, когда становится доступным для использования temporaryAccessPass.|
|lifetimeInMinutes|Int32|Срок службы temporaryAccessPass в минутах, начиная с startDateTime. Минимум 10, максимум 43200 (эквивалент 30 дней).|
|isUsableOnce|Логический|Определяет, ограничен ли пропуск одно время использования. Если пропуск можно использовать один раз; если пропуск можно использовать несколько раз в течение `true` `false` срока службы temporaryAccessPass.|
|isUsable|Логический|Состояние метода проверки подлинности, которое указывает, является ли он в настоящее время удобным для пользователя.|
|methodUsabilityReason|String|Сведения о состоянии использования (isUsable). Причины могут включать: `enabledByPolicy` `disabledByPolicy` , , , `expired` `notYetValid` `oneTimeUsed` .|


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
