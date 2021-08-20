---
title: тип ресурса payloadCompatibleAssignmentFilter
description: Класс, содержащий свойства, используемые для фильтра назначения, совместимых с полезной нагрузкой.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4bedde3f48d3ae1c8a783bafb19d38ac40f14488
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58255341"
---
# <a name="payloadcompatibleassignmentfilter-resource-type"></a>тип ресурса payloadCompatibleAssignmentFilter

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для фильтра назначения, совместимых с полезной нагрузкой.


Наследует от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список полезной нагрузкиCompatibleAssignmentFilters](../api/intune-policyset-payloadcompatibleassignmentfilter-list.md)|[коллекция payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|Список свойств и связей объектов [payloadCompatibleAssignmentFilter.](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|
|[Get payloadCompatibleAssignmentFilter](../api/intune-policyset-payloadcompatibleassignmentfilter-get.md)|[payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|Чтение свойств и связей объекта [payloadCompatibleAssignmentFilter.](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|
|[Создание полезной нагрузкиCompatibleAssignmentFilter](../api/intune-policyset-payloadcompatibleassignmentfilter-create.md)|[payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|Создайте новый [объект payloadCompatibleAssignmentFilter.](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|
|[Удаление полезной нагрузкиCompatibleAssignmentFilter](../api/intune-policyset-payloadcompatibleassignmentfilter-delete.md)|Нет|Удаляет [полезноеloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md).|
|[Обновление полезной нагрузкиCompatibleAssignmentFilter](../api/intune-policyset-payloadcompatibleassignmentfilter-update.md)|[payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|Обновление свойств объекта [payloadCompatibleAssignmentFilter.](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|createdDateTime|DateTimeOffset|Время создания фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|displayName|Строка|DisplayName фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|description|String|Описание фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|платформа|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|Тип платформы устройств, на которых будет применяться фильтр назначения. Наследуется [от deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md). Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|правило|String|Определение правила фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|roleScopeTags|Коллекция String|RoleScopeTags фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|payloadType|[assignmentFilterPayloadType](../resources/intune-policyset-assignmentfilterpayloadtype.md)|PayloadType фильтра назначения. Возможные значения: `notSet`, `enrollmentRestrictions`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.payloadCompatibleAssignmentFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.payloadCompatibleAssignmentFilter",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "platform": "String",
  "rule": "String",
  "roleScopeTags": [
    "String"
  ],
  "payloadType": "String"
}
```




