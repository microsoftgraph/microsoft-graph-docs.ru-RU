---
title: Тип ресурса reportRoot
description: Ресурс, который представляет экземпляр объекта устройства или устранения неполадок отчет, в зависимости от контекста.
localization_priority: Normal
ms.openlocfilehash: 8a2c1cbc666698eea7f466c32bae6c404264f545
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809648"
---
# <a name="reportroot-resource-type"></a>Тип ресурса reportRoot

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс, который представляет экземпляр объекта устройства или устранения неполадок отчет, в зависимости от контекста.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта reportRoot](../api/intune-shared-reportroot-get.md)|Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).|
|[Обновление объекта reportRoot](../api/intune-shared-reportroot-update.md)|Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).|
|**Конфигурация устройств**|
|[Функция deviceConfigurationUserActivity](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|Метаданные для отчета о действиях пользователей с конфигурацией устройств|
|[Функция deviceConfigurationDeviceActivity](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|Метаданные для отчета о работе устройств|
|**Устранение неполадок**|
|[функция managedDeviceEnrollmentAbandonmentDetails](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[report](../resources/intune-shared-report.md)|Метаданные для отчета о регистрации abandonment|
|[функция managedDeviceEnrollmentAbandonmentSummary](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[report](../resources/intune-shared-report.md)|Метаданные для регистрации abandonment сводного отчета|
|[функция managedDeviceEnrollmentFailureDetails](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|Н/Д|
|[функция managedDeviceEnrollmentFailureTrends](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|Метаданные для отчета тенденций сбой подачи заявок|
|[функция managedDeviceEnrollmentTopFailures](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



