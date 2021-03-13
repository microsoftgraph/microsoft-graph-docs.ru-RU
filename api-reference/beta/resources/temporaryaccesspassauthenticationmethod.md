---
title: temporaryAccessPassAuthenticationMethod type
description: Представляет временный пропуск доступа, зарегистрированный пользователю.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8c118978f9e7c8a7c3aa127ba12aba48f2cfe362
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760962"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a>temporaryAccessPassAuthenticationMethod type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет временный пропуск доступа, зарегистрированный пользователю. Временный пропуск доступа — это ограниченный по времени пароль, который служит прочным учетным данным и позволяет использовать учетные данные без паролей.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление](../api/temporaryaccesspassauthenticationmethod-list.md)|[коллекция temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Извлечение списка временных **объектовAccessPassAuthenticationMethod** и их свойств. У пользователей может быть только один метод проверки подлинности временных пропусков доступа.|
|[Создание](../api/temporaryaccesspassauthenticationmethod-post.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Создайте временный **объектAccessPassAuthenticationMethod.**|
|[Получение](../api/temporaryaccesspassauthenticationmethod-get.md);|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Извлечение свойств объекта **temporaryAccessPassAuthenticationMethod** пользователя.||
|[Удаление](../api/temporaryaccesspassauthenticationmethod-delete.md)|Нет|Удаление объекта **temporaryAccessPassAuthenticationMethod** пользователя.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор временного пропуска доступа, зарегистрированного для этого пользователя.|
|temporaryAccessPass|String|Для проверки подлинности используется temporaryAccessPass. Возвращается только при создании нового временногоAccessPass; возвращается как NULL с GET.|
|createdDateTime|DateTimeOffset|Дата и время создания временногоAccessPass.|
|startDateTime|DateTimeOffset|Дата и время, когда становится доступным для использования temporaryAccessPass.|
|lifetimeInMinutes|Int32|Срок службы temporaryAccessPass в минутах, начиная с startDateTime. Минимум 10, максимум 43200 (эквивалент 30 дней).|
|isUsableOnce|Boolean|Определяет, ограничен ли пропуск одно время использования. Если пропуск можно использовать один раз; если пропуск можно использовать несколько раз в течение `true` `false` срока службы temporaryAccessPass.|
|isUsable|Boolean|Состояние метода проверки подлинности, которое указывает, является ли он в настоящее время удобным для пользователя.|
|methodUsabilityReason|String|Сведения о состоянии использования (isUsable). Причины могут включать: `enabledByPolicy` `disabledByPolicy` , , , `expired` `notYetValid` `oneTimeUsed` .|


## <a name="relationships"></a>Отношения
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
