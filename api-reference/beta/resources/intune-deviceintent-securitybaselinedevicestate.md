---
title: Тип ресурса Секуритибаселинедевицестате
description: Сводка по базовому состоянию соответствия требованиям безопасности для устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3a7787ae8a55192adc75ab05f6e6cd21988ab2f4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319351"
---
# <a name="securitybaselinedevicestate-resource-type"></a>Тип ресурса Секуритибаселинедевицестате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка по базовому состоянию соответствия требованиям безопасности для устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Секуритибаселинедевицестатес](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|Коллекция [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Список свойств и связей объектов [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) .|
|[Получение Секуритибаселинедевицестате](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Чтение свойств и связей объекта [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) .|
|[Создание Секуритибаселинедевицестате](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Создание нового объекта [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) .|
|[Удаление Секуритибаселинедевицестате](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|Нет|Удаляет объект [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md).|
|[Обновление Секуритибаселинедевицестате](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|Обновление свойств объекта [секуритибаселинедевицестате](../resources/intune-deviceintent-securitybaselinedevicestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта|
|манажеддевицеид|String|Идентификатор устройства Intune|
|deviceDisplayName|String|Отображаемое имя устройства|
|userPrincipalName|String|"User Principal Name" (Имя участника-пользователя);|
|состояние|[securityBaselineComplianceState](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|Состояние соответствия нормативным требованиям безопасности. Возможные значения: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|
|lastReportedDateTime|DateTimeOffset|Дата и время последнего изменения отчета о политике|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "state": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```



