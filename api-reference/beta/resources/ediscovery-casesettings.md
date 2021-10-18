---
title: тип ресурса caseSettings
description: Содержит ettings для дела об обнаружении электронной почты.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 97b79952653c33d614276ca57c4b726a97cd9be4
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60446460"
---
# <a name="casesettings-resource-type"></a>тип ресурса caseSettings

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит параметры для дела об обнаружении электронной почты. Подробные сведения [см. в материале Настройка параметров](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)поиска и аналитики в Advanced eDiscovery.

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get caseSettings](../api/ediscovery-casesettings-get.md)|[microsoft.graph.ediscovery.caseSettings](../resources/ediscovery-casesettings.md)|Ознакомьтесь с свойствами и отношениями объекта [microsoft.graph.ediscovery.caseSettings.](../resources/ediscovery-casesettings.md)|
|[Обновление caseSettings](../api/ediscovery-casesettings-update.md)|[microsoft.graph.ediscovery.caseSettings](../resources/ediscovery-casesettings.md)|Обновление свойств объекта [microsoft.graph.ediscovery.caseSettings.](../resources/ediscovery-casesettings.md)|
|[resetToDefault](../api/ediscovery-casesettings-resettodefault.md)|Отсутствует|Сброс всех параметров в значения по умолчанию.|

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
  "@odata.type": "microsoft.graph.ediscovery.caseSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseSettings",
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
