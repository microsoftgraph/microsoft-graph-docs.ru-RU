---
title: Тип ресурса ediscoveryCaseSettings
description: Содержит параметры для дела обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 76ec63befe49601e404c3d2dc21e8832cd82ed8c
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946123"
---
# <a name="ediscoverycasesettings-resource-type"></a>Тип ресурса ediscoveryCaseSettings

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит параметры для дела обнаружения электронных данных. Дополнительные сведения см [. в разделе "Настройка параметров поиска и аналитики" в advanced eDiscovery](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).

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

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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

