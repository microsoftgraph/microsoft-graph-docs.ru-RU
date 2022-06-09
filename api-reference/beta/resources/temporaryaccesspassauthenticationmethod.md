---
title: Тип ресурса temporaryAccessPassAuthenticationMethod
description: Представляет временный секретный код, зарегистрированный для пользователя.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 01a393d03bd7095cce9cb8acf07335e92ce6a967
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971254"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a>Тип ресурса temporaryAccessPassAuthenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет временный секретный код, зарегистрированный для пользователя. Временный секретный код — это ограниченный по времени секретный код, который служит надежными учетными данными и позволяет подключать учетные данные без пароля.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список](../api/temporaryaccesspassauthenticationmethod-list.md)|[Коллекция temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Получение списка временных **объектовAccessPassAuthenticationMethod** пользователя и их свойств. У пользователей может быть только один метод проверки подлинности временного прохода доступа.|
|[Создание](../api/temporaryaccesspassauthenticationmethod-post.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Создайте временный **объектAccessPassAuthenticationMethod** пользователя.|
|[Get](../api/temporaryaccesspassauthenticationmethod-get.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Получение свойств объекта **temporaryAccessPassAuthenticationMethod** пользователя.|
|[Удаление](../api/temporaryaccesspassauthenticationmethod-delete.md)|Нет|Удаление объекта **temporaryAccessPassAuthenticationMethod** пользователя.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор временного прохода доступа, зарегистрированного для этого пользователя.|
|temporaryAccessPass|Строка|TemporaryAccessPass, используемый для проверки подлинности. Возвращается только при создании нового временного объектаAccessPass; возвращается как NULL с get.|
|createdDateTime|DateTimeOffset|Дата и время создания temporaryAccessPass.|
|startDateTime|DateTimeOffset|Дата и время, когда temporaryAccessPass становится доступным для использования.|
|lifetimeInMinutes|Int32|Время существования temporaryAccessPass в минутах, начиная с startDateTime. Минимум 10, максимум 43200 (эквивалентно 30 дням).|
|isUsableOnce|Boolean|Определяет, ограничен ли проход одноветным использованием. Если `true`этот проход можно использовать один раз; если `false`он может использоваться несколько раз в течение временного времени существованияAccessPass.|
|isUsable|Boolean|Состояние метода проверки подлинности, указывающее, может ли он в настоящее время быть доступен пользователю.|
|methodUsabilityReason|Строка|Сведения о состоянии удобства использования (isUsable). Возможные причины: `enabledByPolicy`, , `disabledByPolicy`, `expired`, `notYetValid``oneTimeUsed`.|


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
