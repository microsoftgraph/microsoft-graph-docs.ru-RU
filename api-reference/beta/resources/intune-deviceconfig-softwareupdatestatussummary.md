---
title: Тип ресурса softwareUpdateStatusSummary
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67b22bd543b286cbcd714127483550a606fadf7c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793584"
---
# <a name="softwareupdatestatussummary-resource-type"></a>Тип ресурса softwareUpdateStatusSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта softwareUpdateStatusSummary](../api/intune-deviceconfig-softwareupdatestatussummary-get.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Чтение свойств и связей объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).|
|[Обновление объекта softwareUpdateStatusSummary](../api/intune-deviceconfig-softwareupdatestatussummary-update.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|displayName|Строка|Имя политики.|
|compliantDeviceCount|Int32|Количество устройств, соответствующих требованиям.|
|nonCompliantDeviceCount|Int32|Количество устройств, не соответствующих требованиям.|
|remediatedDeviceCount|Int32|Количество исправленных устройств.|
|errorDeviceCount|Int32|Количество устройств с ошибками.|
|unknownDeviceCount|Int32|Количество неизвестных устройств|
|conflictDeviceCount|Int32|Количество конфликтующих устройств.|
|notApplicableDeviceCount|Int32|Количество неприменимых устройств.|
|compliantUserCount|Int32|Количество пользователей, соответствующих требованиям.|
|nonCompliantUserCount|Int32|Количество пользователей, не соответствующих требованиям.|
|remediatedUserCount|Int32|Количество исправленных пользователей.|
|errorUserCount|Int32|Количество пользователей с ошибками.|
|unknownUserCount|Int32|Количество неизвестных пользователей.|
|conflictUserCount|Int32|Количество конфликтующих пользователей.|
|notApplicableUserCount|Int32|Количество неприменимых пользователей.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```



