---
title: тип ресурса deviceConfigurationConflictSummary
description: Сводка конфликтов для набора политик конфигурации устройств.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bc01628379b57b30db2bfc7f72241d7f8b39871e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086857"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a>тип ресурса deviceConfigurationConflictSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка конфликтов для набора политик конфигурации устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List deviceConfigurationConflictSummaries](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|[коллекция deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Список свойств и связей [объектов deviceConfigurationConflictSummary.](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|
|[Get deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Чтение свойств и связей [объекта deviceConfigurationConflictSummary.](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|
|[Создание deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Создание нового [объекта deviceConfigurationConflictSummary.](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|
|[Удаление устройстваConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|Нет|Удаляет [устройствоConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).|
|[Обновление устройстваConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Обновление свойств объекта [deviceConfigurationConflictSummary.](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|conflictingDeviceConfigurations|Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)|Набор политик в конфликте с заданным параметром|
|id|String|ID для этого набора конфликтующих политик. Этот id — это ids всех политик в ConflictingDeviceConfigurations в лексикографическом порядке, разделенных подчеркиваниями.|
|contributingSettings|Коллекция объектов string|Набор параметров в конфликте с заданными политиками|
|deviceCheckinsImpacted|Int32|Количество проверок, на которое влияют конфликтующие политики и параметры|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationConflictSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String",
      "sourceType": "String"
    }
  ],
  "id": "String (identifier)",
  "contributingSettings": [
    "String"
  ],
  "deviceCheckinsImpacted": 1024
}
```



