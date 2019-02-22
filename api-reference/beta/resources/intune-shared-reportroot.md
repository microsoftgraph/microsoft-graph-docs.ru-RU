---
title: Тип ресурса reportRoot
description: Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a2e41d9b17ca7acafa98dad65db5d2ff5ce30925
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151298"
---
# <a name="reportroot-resource-type"></a>Тип ресурса reportRoot

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс, представляющий экземпляр устройства или отчет об устранении неполадок в зависимости от контекста.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта reportRoot](../api/intune-shared-reportroot-get.md)|Чтение свойств и связей объекта [reportRoot](../resources/intune-shared-reportroot.md).|
|[Обновление объекта reportRoot](../api/intune-shared-reportroot-update.md)|Обновление свойств объекта [reportRoot](../resources/intune-shared-reportroot.md).|
|**Настройка устройства**|
|[Функция deviceConfigurationUserActivity](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|Метаданные для отчета о действиях пользователей с конфигурацией устройств|
|[Функция deviceConfigurationDeviceActivity](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|Метаданные для отчета о работе устройств|
|**Устранение неполадок**|
|[Функция Манажеддевицеенроллментабандонментдетаилс](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[report](../resources/intune-shared-report.md)|Метаданные для отчета о прекращении регистрации|
|[Функция Манажеддевицеенроллментабандонментсуммари](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[report](../resources/intune-shared-report.md)|Метаданные для сводного отчета об отмене регистрации|
|[Функция Манажеддевицеенроллментфаилуредетаилс](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|Н/Д|
|[Функция Манажеддевицеенроллментфаилуретрендс](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|Метаданные отчета о тенденциях сбоев регистрации|
|[Функция Манажеддевицеенроллменттопфаилурес](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|Н/Д|

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



