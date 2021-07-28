---
title: тип ресурса cloudPcUserSetting
description: Представляем параметр пользователя облачного ПК
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 0772bfcb3ca6050ec9d920fef24613555e30f6db
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534034"
---
# <a name="cloudpcusersetting-resource-type"></a>тип ресурса cloudPcUserSetting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметр пользователя облачного ПК.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список cloudPcUserSettings](../api/virtualendpoint-list-usersettings.md)|[коллекция cloudPcUserSetting](../resources/cloudpcusersetting.md)|Получите список объектов [cloudPcUserSetting](../resources/cloudpcusersetting.md) и их свойств.|
|[Get cloudPcUserSetting](../api/cloudpcusersetting-get.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcUserSetting.](../resources/cloudpcusersetting.md)|
|[Создание cloudPcUserSetting](../api/virtualendpoint-post-usersettings.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Создание нового [объекта cloudPcUserSetting.](../resources/cloudpcusersetting.md)|
|[Обновление cloudPcUserSetting](../api/cloudpcusersetting-update.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Обновление свойств объекта [cloudPcUserSetting.](../resources/cloudpcusersetting.md)|
|[Удаление cloudPcUserSetting](../api/cloudpcusersetting-delete.md)|Нет|Удаляет объект [cloudPcUserSetting.](../resources/cloudpcusersetting.md)|
|[Assign](../api/cloudpcusersetting-assign.md)|Нет|Назначение [cloudPcUserSetting группам](../resources/cloudpcusersetting.md) пользователей.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для параметров пользователя облачного ПК. Только для чтения.|
|displayName|Строка|Имя параметра, отображаемая в пользовательском интерфейсе. |
|localAdminEnabled|Boolean|Указывает, включен ли локальный параметр администрирования. Значение по умолчанию — `false`. Чтобы включить локальный параметр администрирования, измените параметр на `true` . Если включен локальный параметр администрирования, конечный пользователь может быть администратором устройства облачного ПК. |
|selfServiceEnabled|Boolean|Указывает, включен ли параметр самообслуживки. Значение по умолчанию — `false`. Чтобы включить параметр самообслуживки, измените параметр на `true` .Если включена опция самообслуживки, конечному пользователю разрешено выполнять некоторые операции самообслуживки, например обновление облачного КОМПЬЮТЕРА через портал конечных пользователей.|
|lastModifiedDateTime|DateTimeOffset|Последняя дата и время изменения параметра. Тип Timestamp представляет сведения о дате и времени с помощью формата ISO 8601 и всегда находится во времени UTC. Например, полночь UTC 1 января 2014 г. выглядит так: '2014-01-01T00:00:00Z'. |
|createdDateTime|DateTimeOffset|Дата и время создания параметра. Тип Timestamp представляет сведения о дате и времени с помощью формата ISO 8601 и всегда находится во времени UTC. Например, полночь UTC 1 января 2014 г. выглядит так: '2014-01-01T00:00:00Z'. |

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md)|Представляет набор групп Microsoft 365 и групп безопасности в Azure AD, которые назначены cloudPCUserSetting. Возвращается только с помощью оператора `$expand`. Например, см. [статью Get cloudPcUserSettingample](../api/cloudpcusersetting-get.md).|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcUserSetting",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "id": "String (identifier)",
  "displayName": "String",
  "selfServiceEnabled": "Boolean",
  "localAdminEnabled": "Boolean",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)"
}
```
