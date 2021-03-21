---
title: тип ресурса windowsHelloForBusinessAuthenticationMethod
description: Представление экземпляра Windows Hello для бизнеса, зарегистрированного для пользователя. Windows Hello для бизнеса — это метод проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ad3fd83605d49351e2c57b469339fcfe222f05cb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964857"
---
# <a name="windowshelloforbusinessauthenticationmethod-resource-type"></a>тип ресурса windowsHelloForBusinessAuthenticationMethod

Пространство имен: microsoft.graph

Представление метода проверки подлинности Windows Hello для бизнеса, зарегистрированного для пользователя. Windows Hello для бизнеса — это метод проверки подлинности для устройств Windows.

Наследует от [проверки подлинностиMethod](../resources/authenticationmethod.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список windowsHelloForBusinessAuthenticationMethods](../api/windowshelloforbusinessauthenticationmethod-list.md)|[коллекция windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|Получите список объектов [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) и их свойств.|
|[Get windowsHelloForBusinessAuthenticationMethod](../api/windowshelloforbusinessauthenticationmethod-get.md)|[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)|Ознакомьтесь с свойствами и отношениями [объекта windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)|
|[Удаление windowsHelloForBusinessAuthenticationMethod](../api/windowshelloforbusinessauthenticationmethod-delete.md)|Нет|Удаляет [объект windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время регистрации этого ключа Windows Hello для бизнеса.|
|displayName|String|Имя устройства, на котором зарегистрирована Windows Hello для бизнеса|
|id|String|Уникальный идентификатор для этого метода проверки подлинности. Унаследованный от [проверки подлинностиMethod](../resources/authenticationmethod.md)|
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
