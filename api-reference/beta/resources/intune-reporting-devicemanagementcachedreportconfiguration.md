---
title: тип ресурса deviceManagementCachedReportConfiguration
description: Объект, представляющий конфигурацию кэшного отчета
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1eab917cfba35a38ce5e19b99c6b56505a1f053f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039443"
---
# <a name="devicemanagementcachedreportconfiguration-resource-type"></a>тип ресурса deviceManagementCachedReportConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий конфигурацию кэшного отчета

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementCachedReportConfigurations](../api/intune-reporting-devicemanagementcachedreportconfiguration-list.md)|[коллекция deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|Список свойств и связей [объектов deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|
|[Get deviceManagementCachedReportConfiguration](../api/intune-reporting-devicemanagementcachedreportconfiguration-get.md)|[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|Чтение свойств и связей [объекта deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|
|[Создание deviceManagementCachedReportConfiguration](../api/intune-reporting-devicemanagementcachedreportconfiguration-create.md)|[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|Создание нового [объекта deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|
|[Удаление deviceManagementCachedReportConfiguration](../api/intune-reporting-devicemanagementcachedreportconfiguration-delete.md)|Нет|Удаляет [устройствоManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).|
|[Обновление deviceManagementCachedReportConfiguration](../api/intune-reporting-devicemanagementcachedreportconfiguration-update.md)|[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|Обновление свойств объекта [deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта|
|reportName|String|Имя отчета|
|filter|String|Фильтры, применяемые при создании отчета.|
|select|Коллекция объектов string|Столбцы, выбранные из отчета|
|orderBy|Коллекция объектов string|Порядок столбцов в отчете|
|метаданные|String|Метаданные, управляемые вызывателями, связанные с отчетом|
|status|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|Состояние кэшного отчета. Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|lastRefreshDateTime|DateTimeOffset|Время последнего обновления кэшного отчета|
|expirationDateTime|DateTimeOffset|Время истечения срока действия кэш-отчета|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCachedReportConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "id": "String (identifier)",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "metadata": "String",
  "status": "String",
  "lastRefreshDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```



