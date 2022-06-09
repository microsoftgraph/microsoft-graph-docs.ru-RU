---
title: Тип ресурса temporaryAccessPassAuthenticationMethod
description: Представляет временный секретный код, зарегистрированный для пользователя.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 67f364c387554e972b7fa68d50ac6ee77be26ca9
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971704"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a>Тип ресурса temporaryAccessPassAuthenticationMethod

Пространство имен: microsoft.graph

Представляет временный секретный код, зарегистрированный для пользователя. Временный секретный код — это ограниченный по времени секретный код, который служит надежными учетными данными и позволяет подключать учетные данные без пароля.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список](../api/authentication-list-temporaryaccesspassmethods.md)|[Коллекция temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Получение списка временных **объектовAccessPassAuthenticationMethod** пользователя и их свойств. У пользователей может быть только один метод проверки подлинности временного прохода доступа.|
|[Создание](../api/authentication-post-temporaryaccesspassmethods.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Создайте временный **объектAccessPassAuthenticationMethod** пользователя.|
|[Get](../api/temporaryaccesspassauthenticationmethod-get.md)|[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)|Получение свойств объекта **temporaryAccessPassAuthenticationMethod** пользователя.|
|[Удаление](../api/temporaryaccesspassauthenticationmethod-delete.md)|Нет|Удаление объекта **temporaryAccessPassAuthenticationMethod** пользователя.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания временного прохода доступа.|
|id|Строка|Идентификатор временного прохода доступа, зарегистрированного для этого пользователя. Наследуется от [сущности](../resources/entity.md).|
|isUsableOnce|Boolean|Определяет, ограничен ли проход однофакторным использованием. Если `true`этот проход можно использовать один раз; если `false`этот проход можно использовать несколько раз в течение времени существования временного прохода доступа.|
|isUsable|Boolean|Состояние метода проверки подлинности, указывающее, может ли он в настоящее время быть доступен пользователю.|
|lifetimeInMinutes|Int32|Время существования временного прохода доступа в минутах, начиная с **startDateTime**. Должно быть от 10 до 43200 включительно (эквивалентно 30 дням).|
|methodUsabilityReason|Строка|Сведения о состоянии удобства использования (**isUsable**). Возможные причины: `EnabledByPolicy`, , `DisabledByPolicy`, `Expired`, `NotYetValid``OneTimeUsed`.|
|startDateTime|DateTimeOffset|Дата и время, когда временный секретный код становится доступным для использования и когда **применяется режим isUsable**`true`.|
|temporaryAccessPass|Строка|Временный секретный код, используемый для проверки подлинности. Возвращается только при создании нового временного объектаAccessPass; Скрыто в последующих операциях чтения и возвращается, как `null` в get.|

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
