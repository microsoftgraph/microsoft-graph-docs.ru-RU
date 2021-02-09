---
title: Тип ресурса deviceManagementReports
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8ca39e6f1c8c2425123c04b71ca5146fc5585419
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160640"
---
# <a name="devicemanagementreports-resource-type"></a>Тип ресурса deviceManagementReports

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементный объект, служащий контейнером для всех функций управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get deviceManagementReports](../api/intune-rapolicy-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-rapolicy-devicemanagementreports.md)|Чтение свойств и связей объекта [deviceManagementReports.](../resources/intune-rapolicy-devicemanagementreports.md)|
|[Обновление deviceManagementReports](../api/intune-rapolicy-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-rapolicy-devicemanagementreports.md)|Обновление свойств объекта [deviceManagementReports.](../resources/intune-rapolicy-devicemanagementreports.md)|
|[Действие getCertificatesReport](../api/intune-rapolicy-devicemanagementreports-getcertificatesreport.md)|Stream|Н/Д|

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




