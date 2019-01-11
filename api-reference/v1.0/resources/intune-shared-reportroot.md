---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр отчетов журнала.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53fedc78575e48d77419a598b73e1760c8c6457c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850290"
---
# <a name="reportroot-resource-type"></a>Тип ресурса reportRoot

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс, представляющий экземпляр отчетов журнала.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта reportRoot](../api/intune-shared-reportroot-get.md)|[reportRoot](../resources/intune-shared-reportroot.md)|Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).|
|[Обновление объекта reportRoot](../api/intune-shared-reportroot-update.md)|[reportRoot](../resources/intune-shared-reportroot.md)|Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).|
|**Конфигурация устройств**|
|[Функция deviceConfigurationDeviceActivity](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|[report](../resources/intune-shared-report.md)|Метаданные для отчета о действиях устройств с конфигурацией устройств|
|[Функция deviceConfigurationUserActivity](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|[report](../resources/intune-shared-report.md)|Метаданные для отчета о действиях пользователей с конфигурацией устройств|
|**Устранение неполадок**|
|[функция managedDeviceEnrollmentFailureDetails](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|[report](../resources/intune-shared-report.md)|Еще не документированы.|
|[функция managedDeviceEnrollmentTopFailures](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|[report](../resources/intune-shared-report.md)|Еще не документированы.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a>Пример

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
