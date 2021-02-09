---
title: Тип ресурса deviceAndAppManagementAssignmentFilter
description: Класс, содержащий свойства, используемые для фильтра назначений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 842a724a70f27edfbcd75a423ecaa8aab547e873
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157535"
---
# <a name="deviceandappmanagementassignmentfilter-resource-type"></a>Тип ресурса deviceAndAppManagementAssignmentFilter

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для фильтра назначений.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceAndAppManagementAssignmentFilters](../api/intune-policyset-deviceandappmanagementassignmentfilter-list.md)|[Коллекция deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Список свойств и связей объектов [deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[Get deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-get.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Чтение свойств и связей объекта [deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[Создание deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-create.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Создание объекта [deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[Удаление deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-delete.md)|Нет|Удаляет [deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[Обновление deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-update.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Обновление свойств объекта [deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[Действие validateFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-validatefilter.md)|[assignmentFilterValidationResult](../resources/intune-policyset-assignmentfiltervalidationresult.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ фильтра назначений.|
|createdDateTime|DateTimeOffset|Время создания фильтра назначений.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения фильтра назначений.|
|displayName|String|DisplayName фильтра назначений.|
|description|String|Описание фильтра назначений.|
|платформа|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|Тип платформы устройств, на которых будет применяться фильтр назначений. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|rule|String|Определение правила фильтра назначений.|
|roleScopeTags|Коллекция String|RoleScopeTags фильтра назначений.|

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




