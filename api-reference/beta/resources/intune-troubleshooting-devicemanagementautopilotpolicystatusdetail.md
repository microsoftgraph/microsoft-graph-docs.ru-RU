---
title: Тип ресурса Девицеманажементаутопилотполицистатусдетаил
description: Элемент сведений о состоянии политики, содержащийся в событии автопилота.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d45ee08be1f7ea04e27f3fa002b58f4ebf7e6434
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087665"
---
# <a name="devicemanagementautopilotpolicystatusdetail-resource-type"></a>Тип ресурса Девицеманажементаутопилотполицистатусдетаил

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Элемент сведений о состоянии политики, содержащийся в событии автопилота.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементаутопилотполицистатусдетаилс](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-list.md)|Коллекция [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Список свойств и связей объектов [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .|
|[Получение Девицеманажементаутопилотполицистатусдетаил](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-get.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Чтение свойств и связей объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .|
|[Создание Девицеманажементаутопилотполицистатусдетаил](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-create.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Создание нового объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .|
|[Удаление Девицеманажементаутопилотполицистатусдетаил](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-delete.md)|Нет|Удаляет объект [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).|
|[Обновление Девицеманажементаутопилотполицистатусдетаил](../api/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail-update.md)|[deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)|Обновление свойств объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|UUID объекта.|
|displayName|Строка|Понятное имя политики.|
|полицитипе|[deviceManagementAutopilotPolicyType](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|Тип политики. Возможные значения: `unknown`, `application`, `appModel`, `configurationPolicy`.|
|комплианцестатус|[deviceManagementAutopilotPolicyComplianceStatus](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|Состояние соответствия политике. Возможные значения: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.|
|траккедоненроллментстатус|Boolean|Указывает, была ли эта пролици зарегистрирована в рамках сеанса синхронизации автоматической загрузки для автоматической пилотной установки|
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






