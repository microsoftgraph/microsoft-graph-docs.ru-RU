---
title: Тип ресурса temporaryAccessPassAuthenticationMethod
description: Представляет временный секретный код, зарегистрированный для пользователя.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 136df8006925470d139c7c94f3d7a2c3e0ff35be
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094073"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a>Тип ресурса temporaryAccessPassAuthenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет временный секретный код, зарегистрированный для пользователя. Временный секретный код — это ограниченный по времени секретный код, который служит надежными учетными данными и позволяет подключать учетные данные без пароля. Доступность и параметры, которые можно настроить для **temporaryAccessPassAuthenticationMethod** , зависят от политики временных методов [access Pass](temporaryaccesspassauthenticationmethodconfiguration.md).

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
|temporaryAccessPass|String|Временный секретный код, используемый для проверки подлинности. Возвращается только при создании нового объекта **temporaryAccessPassAuthenticationMethod** ; Скрыто в последующих операциях чтения и возвращается, как `null` в get.|


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
