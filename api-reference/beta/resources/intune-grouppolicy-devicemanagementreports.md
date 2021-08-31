---
title: тип ресурса deviceManagementReports
description: Объект Singleton, который выступает в качестве контейнера для всех функциональных возможностей отчетов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 243fd6d317f5fe081feb8193cdfec7df9f2ec720
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58795846"
---
# <a name="devicemanagementreports-resource-type"></a>тип ресурса deviceManagementReports

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект Singleton, который выступает в качестве контейнера для всех функциональных возможностей отчетов.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get deviceManagementReports](../api/intune-grouppolicy-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-grouppolicy-devicemanagementreports.md)|Чтение свойств и связей [объекта deviceManagementReports.](../resources/intune-grouppolicy-devicemanagementreports.md)|
|[Обновление deviceManagementReports](../api/intune-grouppolicy-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-grouppolicy-devicemanagementreports.md)|Обновление свойств объекта [deviceManagementReports.](../resources/intune-grouppolicy-devicemanagementreports.md)|
|[getGroupPolicySettingsDeviceSettingsReport action](../api/intune-grouppolicy-devicemanagementreports-getgrouppolicysettingsdevicesettingsreport.md)|Stream|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для этого объекта|

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



