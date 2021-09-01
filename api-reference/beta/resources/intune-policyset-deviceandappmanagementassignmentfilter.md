---
title: тип ресурса deviceAndAppManagementAssignmentFilter
description: Класс, содержащий свойства, используемые для фильтра назначения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a21edb65043744659b6797470fd19bf475625076
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796841"
---
# <a name="deviceandappmanagementassignmentfilter-resource-type"></a>тип ресурса deviceAndAppManagementAssignmentFilter

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для фильтра назначения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List deviceAndAppManagementAssignmentFilters](../api/intune-policyset-deviceandappmanagementassignmentfilter-list.md)|[коллекция deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Список свойств и связей [объектов deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[Get deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-get.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Чтение свойств и связей [объекта deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[Создание устройстваAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-create.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Создайте новое [устройствоAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[Удаление устройстваAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-delete.md)|Нет|Удаляет [устройствоAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).|
|[Обновление устройстваAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-update.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Обновление свойств объекта [deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[проверка действияFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-validatefilter.md)|[assignmentFilterValidationResult](../resources/intune-policyset-assignmentfiltervalidationresult.md)|Пока не задокументировано.|
|[включить действие](../api/intune-policyset-deviceandappmanagementassignmentfilter-enable.md)|Нет|Н/Д|
|[функция getState](../api/intune-policyset-deviceandappmanagementassignmentfilter-getstate.md)|[assignmentFilterState](../resources/intune-policyset-assignmentfilterstate.md)|Пока не задокументировано.|
|[функция getPlatformSupportedProperties](../api/intune-policyset-deviceandappmanagementassignmentfilter-getplatformsupportedproperties.md)|[assignmentFilterSupportedProperty](../resources/intune-policyset-assignmentfiltersupportedproperty.md) collection|Пока не задокументировано.|
|[функция getSupportedProperties](../api/intune-policyset-deviceandappmanagementassignmentfilter-getsupportedproperties.md)|[assignmentFilterSupportedProperty](../resources/intune-policyset-assignmentfiltersupportedproperty.md) collection|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ фильтра назначения.|
|createdDateTime|DateTimeOffset|Время создания фильтра назначения.|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время фильтра назначения.|
|displayName|Строка|DisplayName фильтра назначения.|
|description|Строка|Описание фильтра назначения.|
|платформа|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|Тип платформы устройств, на которых будет применяться фильтр назначения. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|правило|Строка|Определение правила фильтра назначения.|
|roleScopeTags|Коллекция String|RoleScopeTags фильтра назначения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "platform": "String",
  "rule": "String",
  "roleScopeTags": [
    "String"
  ]
}
```



