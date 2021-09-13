---
title: тип ресурса deviceManagementReports
description: Объект Singleton, который выступает в качестве контейнера для всех функциональных возможностей отчетов.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cbcffd77d9002477c2f20fc54f8909e60cc2c70b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086136"
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
|id|String|Уникальный идентификатор для этого объекта|

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



