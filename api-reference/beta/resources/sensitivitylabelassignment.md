---
title: Тип ресурса sensitivityLabelAssignment
description: Предоставляет сведения о метке конфиденциальности, назначенной файлу в SharePoint или OneDrive для бизнеса.
author: jaLuthra
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3f46f0c064bb03286f1d38ba9c915db243acff9f
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917924"
---
# <a name="sensitivitylabelassignment-resource-type"></a>Тип ресурса sensitivityLabelAssignment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о метке конфиденциальности, назначенной файлу [в SharePoint или](./driveitem.md) OneDrive для бизнеса.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|assignmentMethod|sensitivityLabelAssignmentMethod|Указывает, выполняется ли назначение меток автоматически, как стандартная или привилегированная операция. Допустимые значения: `standard`, `privileged`, `auto`, `unknownFutureValue`.|
|sensitivityLabelId|String|Уникальный идентификатор метки конфиденциальности, назначенной файлу.|
|tenantId|String|Уникальный идентификатор клиента, в котором размещается файл при применении этой метки.|

### <a name="sensitivitylabelassignmentmethod-values"></a>значения sensitivityLabelAssignmentMethod

| Member             | Описание                                    |
|:------------------ |:-----------------------------------------------|
| Стандартный           | Метод присваивания для метки является стандартным.|
| Привилегированных         | Метод присваивания метки является привилегированным. Указывает, что метка применяется пользователем или администратором вручную.|
| Авто               | Указывает, что метка автоматически применяется системой из-за настроенной политики, такой как метка по умолчанию или автоматическая классификация конфиденциального содержимого.|
| unknownFutureValue | Значение sentinel для развиваемого перечисления. Не следует использовать.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|Метки|[extractSensitivityLabelsResult](./extractsensitivitylabelsresult.md)|Список меток конфиденциальности, назначенных файлу.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sensitivityLabelAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sensitivityLabelAssignment",
  "assignmentMethod": "String",
  "sensitivityLabelId": "String",
  "tenantId": "String"
}
```

