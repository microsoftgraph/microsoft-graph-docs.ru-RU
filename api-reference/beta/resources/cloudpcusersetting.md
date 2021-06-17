---
title: тип ресурса cloudPcUserSetting
description: Представляем параметр пользователя облачного компьютера
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 324d2ba65c82b44595fff366c5d6eb25005c20ef
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993744"
---
# <a name="cloudpcusersetting-resource-type"></a>тип ресурса cloudPcUserSetting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметр пользователя облачного КОМПЬЮТЕРА.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список cloudPcUserSettings](../api/virtualendpoint-list-usersettings.md)|[коллекция cloudPcUserSetting](../resources/cloudpcusersetting.md)|Получите список объектов [cloudPcUserSetting](../resources/cloudpcusersetting.md) и их свойств.|
|[Get cloudPcUserSetting](../api/cloudpcusersetting-get.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcUserSetting.](../resources/cloudpcusersetting.md)|
|[Создание cloudPcUserSetting](../api/virtualendpoint-post-usersettings.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Создание нового [объекта cloudPcUserSetting.](../resources/cloudpcusersetting.md)|
|[Обновление cloudPcUserSetting](../api/cloudpcusersetting-update.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|Обновление свойств объекта [cloudPcUserSetting.](../resources/cloudpcusersetting.md)|
|[Удаление cloudPcUserSetting](../api/cloudpcusersetting-delete.md)|Нет|Удаляет объект [cloudPcUserSetting.](../resources/cloudpcusersetting.md)|
|[назначение](../api/cloudpcusersetting-assign.md)|Нет|Назначение [cloudPcUserSetting группам](../resources/cloudpcusersetting.md) пользователей.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для параметров пользователя облачного КОМПЬЮТЕРА. Только для чтения.|
|displayName|String|Имя параметра, отображаемая в пользовательском интерфейсе. |
|localAdminEnabled|Логический|Указывает, включен ли локальный параметр администрирования. Значение по умолчанию — `false`. Чтобы включить локальный параметр администрирования, измените параметр на `true` . |
|selfServiceEnabled|Логический|Указывает, включен ли параметр самообслуживки. Значение по умолчанию — `false`. Чтобы включить параметр самообслуживки, измените параметр на `true` . |
|lastModifiedDateTime|DateTimeOffset|Последняя дата и время изменения параметра. Тип Timestamp представляет сведения о дате и времени с помощью формата ISO 8601 и всегда находится во времени UTC. Например, полночь UTC 1 января 2014 г. выглядит так: '2014-01-01T00:00:00Z'. |
|createdDateTime|DateTimeOffset|Дата и время создания параметра. Тип Timestamp представляет сведения о дате и времени с помощью формата ISO 8601 и всегда находится во времени UTC. Например, полночь UTC 1 января 2014 г. выглядит так: '2014-01-01T00:00:00Z'. |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md)|Office 365 группы безопасности в Azure AD могут иметь набор параметров пользователя.|

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
