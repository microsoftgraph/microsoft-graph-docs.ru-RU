---
title: Тип ресурса Девицеманажементаутопилотполицистатусдетаил
description: Элемент сведений о состоянии политики, содержащийся в событии автопилота.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 59e2ec1273d9bc2cdb938021e8eba45debedf7b9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42765736"
---
# <a name="devicemanagementautopilotpolicystatusdetail-resource-type"></a>Тип ресурса Девицеманажементаутопилотполицистатусдетаил

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Элемент сведений о состоянии политики, содержащийся в событии автопилота.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементаутопилотполицистатусдетаилс](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-list.md)|Коллекция [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Список свойств и связей объектов [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .|
|[Получение Девицеманажементаутопилотполицистатусдетаил](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-get.md)|[девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Чтение свойств и связей объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .|
|[Создание Девицеманажементаутопилотполицистатусдетаил](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-create.md)|[девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Создание нового объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .|
|[Удаление Девицеманажементаутопилотполицистатусдетаил](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-delete.md)|Нет|Удаляет объект [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).|
|[Обновление Девицеманажементаутопилотполицистатусдетаил](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-update.md)|[девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Обновление свойств объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта.|
|displayName|Строка|Понятное имя политики.|
|полицитипе|[девицеманажементаутопилотполицитипе](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|Тип политики. Возможные значения: `unknown`, `application`, `appModel`, `configurationPolicy`.|
|комплианцестатус|[девицеманажементаутопилотполицикомплианцестатус](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|Состояние соответствия политике. Возможные значения: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.|
|траккедоненроллментстатус|Логический|Указывает, была ли эта пролици зарегистрирована в рамках сеанса синхронизации автоматической загрузки для автоматической пилотной установки|
|lastReportedDateTime|DateTimeOffset|Метка времени для отчета о состоянии политики|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAutopilotPolicyStatusDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "String (identifier)",
  "displayName": "String",
  "policyType": "String",
  "complianceStatus": "String",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "String (timestamp)"
}
```



