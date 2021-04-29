---
title: тип ресурса параметров (eDiscovery)
description: Параметры для дела об обнаружении электронной почты
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 9f0248fa0c6080a143272d997b9d6125e0ccb5a2
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080881"
---
# <a name="settings-resource-type-ediscovery"></a>тип ресурса параметров (eDiscovery)

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры для дела об обнаружении электронной почты. Подробные сведения [см. в материале Настройка параметров](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)поиска и аналитики в Advanced eDiscovery.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение параметров](../api/ediscovery-settings-get.md)|[microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md)|Ознакомьтесь с свойствами и отношениями объекта [microsoft.graph.ediscovery.settings.](../resources/ediscovery-settings.md)|
|[Обновление параметров](../api/ediscovery-settings-update.md)|[microsoft.graph.ediscovery.settings](../resources/ediscovery-settings.md)|Обновление свойств объекта [microsoft.graph.ediscovery.settings.](../resources/ediscovery-settings.md)|
|[resetToDefault](../api/ediscovery-settings-resettodefault.md)|Нет|Сброс всех параметров в значения по умолчанию.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|Id|String|ID дела об обнаружении электронной почты. Наследуется от [сущности](../resources/entity.md).|
|ocr|[microsoft.graph.ediscovery.ocrSettings](../resources/ediscovery-ocrsettings.md)|Параметры OCR (Optical Character Recognition) для дела.|
|redundancyDetection|[microsoft.graph.ediscovery.redundancyDetectionSettings](../resources/ediscovery-redundancydetectionsettings.md)|Параметры обнаружения избыточности (рядом с дубликатом и потоком электронной почты) для дела.|
|topicModeling|[microsoft.graph.ediscovery.topicModelingSettings](../resources/ediscovery-topicmodelingsettings.md)|Параметры моделирования тем (Темы) для дела.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.settings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.settings",
  "id": "String (identifier)",
  "redundancyDetection": {
    "@odata.type": "microsoft.graph.ediscovery.redundancyDetectionSettings"
  },
  "topicModeling": {
    "@odata.type": "microsoft.graph.ediscovery.topicModelingSettings"
  },
  "ocr": {
    "@odata.type": "microsoft.graph.ediscovery.ocrSettings"
  }
}
```
