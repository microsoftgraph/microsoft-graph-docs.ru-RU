---
title: Тип ресурса windowsInformationProtectionNetworkLearningSummary
description: Объект сводки по обучению Windows Information Protection для сетей
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ad392b2685d4322c5afc90f82c381a790ef8a46
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250490"
---
# <a name="windowsinformationprotectionnetworklearningsummary-resource-type"></a>Тип ресурса windowsInformationProtectionNetworkLearningSummary

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект сводки по обучению Windows Information Protection для сетей

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-list.md)|Коллекция [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Список свойств и связей объектов [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|
|[Получение объекта windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-get.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|Чтение свойств и связей объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|
|[Создание объекта windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-create.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|Создание объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|
|[Удаление объекта windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-delete.md)|Нет|Удаляет объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|
|[Обновление объекта windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-update.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.|
|url|String|URL-адрес веб-сайта|
|deviceCount|Int32|Количество устройств|

## <a name="relationships"></a>Связи
None

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionNetworkLearningSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "String (identifier)",
  "url": "String",
  "deviceCount": 1024
}
```



