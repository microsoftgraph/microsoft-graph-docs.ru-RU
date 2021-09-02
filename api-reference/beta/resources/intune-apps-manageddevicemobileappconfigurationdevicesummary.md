---
title: Тип ресурса managedDeviceMobileAppConfigurationDeviceSummary
description: Содержит свойства, унаследованные свойства и действия из сводки по состоянию конфигурации мобильных приложений MDM для устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 656110a40282d003724f391f075d40e79e2ad086
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789342"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a>Тип ресурса managedDeviceMobileAppConfigurationDeviceSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, унаследованные свойства и действия из сводки по состоянию конфигурации мобильных приложений MDM для устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта managedDeviceMobileAppConfigurationDeviceSummary](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).|
|[Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|pendingCount|Int32|Количество ожидающих устройств.|
|notApplicableCount|Int32|Количество неприменимых устройств.|
|notApplicablePlatformCount|Int32|Количество не применимых устройств из-за несоответствия платформы и политики|
|successCount|Int32|Количество успешных устройств.|
|errorCount|Int32|Количество устройств с ошибками.|
|failedCount|Int32|Число устройств со сбоями.|
|conflictCount|Int32|Количество устройств в конфликте|
|lastUpdateDateTime|DateTimeOffset|Время последнего обновления.|
|configurationVersion|Int32|Версия политики для этого обзора|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



