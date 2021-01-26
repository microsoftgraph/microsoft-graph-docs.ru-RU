---
title: Тип ресурса windowsHelloForBusinessAuthenticationMethod
description: Представление экземпляра Windows Hello для бизнеса, зарегистрированного для пользователя. Windows Hello для бизнеса — это метод проверки подлинности при входе.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dcbbebf03a91563e5504eb3032f57f973a4c3ede
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982483"
---
# <a name="windowshelloforbusinessauthenticationmethod-resource-type"></a>Тип ресурса windowsHelloForBusinessAuthenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление метода проверки подлинности Windows Hello для бизнеса, зарегистрированного для пользователя. Windows Hello для бизнеса — это способ проверки подлинности при входе на устройства с Windows.

Наследуется от [authenticationMethod.](../resources/authenticationmethod.md)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список windowsHelloForBusinessAuthenticationMethods](../api/windowshelloforbusinessauthenticationmethod-list.md)|[Коллекция windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|Получите список объектов [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) и их свойств.|
|[Get windowsHelloForBusinessAuthenticationMethod](../api/windowshelloforbusinessauthenticationmethod-get.md)|[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|Чтение свойств и связей объекта [windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)|
|[Удаление windowsHelloForBusinessAuthenticationMethod](../api/windowshelloforbusinessauthenticationmethod-delete.md)|Нет|Удаляет объект [windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время регистрации этого ключа Windows Hello для бизнеса.|
|displayName|String|Имя устройства, на котором зарегистрирована windows Hello для бизнеса|
|id|String|Уникальный идентификатор для этого метода проверки подлинности. Наследуется [от authenticationMethod](../resources/authenticationmethod.md)|
|keyStrength|authenticationMethodKeyStrength|Ключевая сила этого ключа Windows Hello для бизнеса. Возможные значения: `normal`, `weak`, `unknown`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|device;|[device](../resources/device.md)|Зарегистрированное устройство, на котором находится этот ключ Windows Hello для бизнеса.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "createdDateTime": "String",
  "keyStrength": {"@odata.type": "microsoft.graph.authenticationMethodKeyStrength"}
}
```
