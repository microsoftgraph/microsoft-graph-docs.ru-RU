---
title: Тип ресурса ediscoveryCaseSettings
description: Содержит параметры для дела обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 9ddca3073403ea284295d89bbf4dae3fe4e380c4
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839620"
---
# <a name="ediscoverycasesettings-resource-type"></a>Тип ресурса ediscoveryCaseSettings

Пространство имен: microsoft.graph.security



Содержит параметры для дела обнаружения электронных данных. Дополнительные сведения см[. в разделе "Настройка параметров поиска и аналитики" в службе обнаружения электронных данных (цен. категория "Премиум").](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение ediscoveryCaseSettings](../api/security-ediscoverycasesettings-get.md)|[microsoft.graph.security.ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md)|Чтение свойств и связей объекта [ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md) .|
|[Обновление ediscoveryCaseSettings](../api/security-ediscoverycasesettings-update.md)|[microsoft.graph.security.ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md)|Обновление свойств объекта [ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md) .|
|[resetToDefault](../api/security-ediscoverycasesettings-resettodefault.md)|Нет|Сброс всех параметров до значений по умолчанию.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор дела обнаружения электронных данных. Наследуется от [сущности](../resources/entity.md).|
|Ocr|[microsoft.graph.security.ocrSettings](../resources/security-ocrsettings.md)|Параметры OCR (оптическое распознавание символов) для дела.|
|redundancyDetection|[microsoft.graph.security.redundancyDetectionSettings](../resources/security-redundancydetectionsettings.md)|Параметры обнаружения избыточности (почти дубликатов и потоков электронной почты) для дела.|
|topicModeling|[microsoft.graph.security.topicModelingSettings](../resources/security-topicmodelingsettings.md)|Параметры моделирования тем (тем) для дела.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryCaseSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryCaseSettings",
  "id": "String (identifier)",
  "redundancyDetection": {
    "@odata.type": "microsoft.graph.security.redundancyDetectionSettings"
  },
  "topicModeling": {
    "@odata.type": "microsoft.graph.security.topicModelingSettings"
  },
  "ocr": {
    "@odata.type": "microsoft.graph.security.ocrSettings"
  }
}
```

