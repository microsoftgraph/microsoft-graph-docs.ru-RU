---
title: Тип ресурса deviceComplianceDeviceStatus
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68a2993b3705a391738c7d8f0cf2c35d4e63fb05
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979524"
---
# <a name="devicecompliancedevicestatus-resource-type"></a>Тип ресурса deviceComplianceDeviceStatus

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceComplianceDeviceStatus](../api/intune-deviceconfig-devicecompliancedevicestatus-list.md)|Коллекция [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|Список свойств и связей объектов [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).|
|[Получение объекта deviceComplianceDeviceStatus](../api/intune-deviceconfig-devicecompliancedevicestatus-get.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md);|Чтение свойств и связей объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).|
|[Создание объекта deviceComplianceDeviceStatus](../api/intune-deviceconfig-devicecompliancedevicestatus-create.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md);|Создание объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).|
|[Удаление объекта deviceComplianceDeviceStatus](../api/intune-deviceconfig-devicecompliancedevicestatus-delete.md)|Нет|Удаляет объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).|
|[Обновление объекта deviceComplianceDeviceStatus](../api/intune-deviceconfig-devicecompliancedevicestatus-update.md)|[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)|Обновление свойств объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|deviceDisplayName|String|Имя устройства в объекте DevicePolicyStatus.|
|userName|String|Имя пользователя в отчете|
|deviceModel|String|Модель устройства в отчете|
|platform|Int32|Платформа для устройства, о котором сообщается|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время, когда истекает период отсрочки применения политик на устройстве.|
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
  "@odata.type": "microsoft.graph.deviceComplianceDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "platform": 1024,
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```





