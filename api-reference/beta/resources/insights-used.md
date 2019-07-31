---
title: Тип ресурса Усединсигхт
description: Представление документов, используемых определенным пользователем. Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или к которым обращался.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2b6e7a7c4df94e9ffbcb34ef200457b4a903eb24
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005690"
---
# <a name="usedinsight-resource-type"></a>Тип ресурса Усединсигхт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление документов, используемых определенным пользователем. Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или к которым обращался. Сюда входят документы в:

- OneDrive для бизнеса
- SharePoint

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список "Использованные"](../api/insights-list-used.md) |Коллекция [usedInsight](insights-used.md)| Получение списка используемых файлов.|

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание  |
| -------------         |---------------            | -------------|
| id                    | String                    | Уникальный идентификатор связи. Только для чтения.        |
| Ластусед              | [usageDetails](insights-usagedetails.md)              | Сведения о том, когда элемент был последний раз просмотрен и изменен пользователем. Только для чтения.     |
| Ресурсе resourcevisualization | [Ресурсе resourcevisualization](insights-resourcevisualization.md)                | Свойства, которые можно использовать для отображения документа в вашем интерфейсе. Только для чтения      |
| Ресаурцереференце     | [Ресаурцереференце](insights-resourcereference.md)                      | Справочные свойства используемого документа, например URL-адрес и тип документа. Только для чтения     |

## <a name="relationships"></a>Отношения

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | Коллекция [объектов](entity.md)    | Используется для перехода к использованному элементу. Для вложений в файл используется тип *fileAttachment*. Для связанных вложений используется тип *driveItem*. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": { "@odata.type": "microsoft.graph.resourceVisualization" },
  "resourceReference": { "@odata.type": "microsoft.graph.resourceReference" }
}
```
