---
title: Тип ресурса windowsInformationProtectionNetworkLearningSummary
description: Объект сводки по обучению Windows Information Protection для сетей
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3c37fa23add89b0366d2f200baea58581d5f231e
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60446184"
---
# <a name="windowsinformationprotectionnetworklearningsummary-resource-type"></a>Тип ресурса windowsInformationProtectionNetworkLearningSummary

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект сводки по обучению Windows Information Protection для сетей

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-list.md)|Коллекция [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Список свойств и связей объектов [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|
|[Получение объекта windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-get.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Чтение свойств и связей объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|
|[Создание объекта windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-create.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Создание объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|
|[Удаление объекта windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-delete.md)|Нет|Удаляет объект [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|
|[Обновление объекта windowsInformationProtectionNetworkLearningSummary](../api/intune-wip-windowsinformationprotectionnetworklearningsummary-update.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md)|Обновление свойств объекта [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта WindowsInformationProtectionNetworkLearningSummary.|
|url|String|URL-адрес веб-сайта|
|deviceCount|Int32|Количество устройств|

## <a name="relationships"></a>Связи
Нет

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



