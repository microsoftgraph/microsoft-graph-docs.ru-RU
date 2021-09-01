---
title: тип ресурса deviceManagementReports
description: Класс DeviceManagementReports для отчетности V2
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3a726d3fb1cd0222e3a9939467e0d94ebb27df9c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820339"
---
# <a name="devicemanagementreports-resource-type"></a>тип ресурса deviceManagementReports

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс DeviceManagementReports для отчетности V2

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get deviceManagementReports](../api/intune-remoteassistance-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-remoteassistance-devicemanagementreports.md)|Чтение свойств и связей [объекта deviceManagementReports.](../resources/intune-remoteassistance-devicemanagementreports.md)|
|[Обновление deviceManagementReports](../api/intune-remoteassistance-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-remoteassistance-devicemanagementreports.md)|Обновление свойств объекта [deviceManagementReports.](../resources/intune-remoteassistance-devicemanagementreports.md)|
|[getRemoteAssistanceSessionsReport action](../api/intune-remoteassistance-devicemanagementreports-getremoteassistancesessionsreport.md)|Stream|Н/Д|
|[getRemoteAssistanceMonitorActiveSessionsReport](../api/intune-remoteassistance-devicemanagementreports-getremoteassistancemonitoractivesessionsreport.md)|Stream|Н/Д|
|[getRemoteAssistanceMonitorTotalSessionsReport](../api/intune-remoteassistance-devicemanagementreports-getremoteassistancemonitortotalsessionsreport.md)|Stream|Н/Д|
|[getRemoteAssistanceMonitorAvgSessionTimeReport action](../api/intune-remoteassistance-devicemanagementreports-getremoteassistancemonitoravgsessiontimereport.md)|Stream|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReports"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "String (identifier)"
}
```



