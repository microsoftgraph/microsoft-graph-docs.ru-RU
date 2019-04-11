---
title: Тип ресурса deviceConfigurationUserStatus
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c7d975d3c59976a2880f7299917d8a1158ddc4d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773212"
---
# <a name="deviceconfigurationuserstatus-resource-type"></a>Тип ресурса deviceConfigurationUserStatus

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceConfigurationUserStatus](../api/intune-deviceconfig-deviceconfigurationuserstatus-list.md)|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Список свойств и связей объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).|
|[Get deviceConfigurationUserStatus](../api/intune-deviceconfig-deviceconfigurationuserstatus-get.md)|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Чтение свойств и связей объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).|
|[Создание объекта deviceConfigurationUserStatus](../api/intune-deviceconfig-deviceconfigurationuserstatus-create.md)|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Создание объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).|
|[Delete deviceConfigurationUserStatus](../api/intune-deviceconfig-deviceconfigurationuserstatus-delete.md)|Нет|Удаляет объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).|
|[Обновление объекта deviceConfigurationUserStatus](../api/intune-deviceconfig-deviceconfigurationuserstatus-update.md)|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Обновление свойств объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|userDisplayName|String|Имя пользователя в объекте DevicePolicyStatus.|
|devicesCount|Int32|Количество устройств для этого пользователя.|
|status|[Комплианцестатус](../resources/intune-shared-compliancestatus.md)|Состояние соответствия требованиям для отчета о политике. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Дата и время последнего изменения отчета о политике.|
|userPrincipalName|String|Имя участника-пользователя.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```





