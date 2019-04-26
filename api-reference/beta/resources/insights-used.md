---
title: используемый тип ресурса
description: Представление документов, используемых определенным пользователем. Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или к которым обращался.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 35698741cd457f4e8d202b13dd9099bb2669b6e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551293"
---
# <a name="used-resource-type"></a>используемый тип ресурса

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представление документов, используемых определенным пользователем. Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или к которым обращался. Сюда входят документы в:

- OneDrive для бизнеса
- SharePoint

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список "Использованные"](../api/insights-list-used.md) |Коллекция [инсигхтс_усед](insights-used.md)| Получение списка используемых файлов.|

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание  |
| -------------         |---------------            | -------------|
| id                    | String                    | Уникальный идентификатор связи. Только для чтения.        |
| Ластусед              | [usageDetails](insights-usagedetails.md)              | Сведения о том, когда элемент был последний раз просмотрен и изменен пользователем. Только для чтения.     |
| Ресурсе resourcevisualization | [Ресурсе resourcevisualization](insights-resourcevisualization.md)                | Свойства, которые можно использовать для отображения документа в вашем интерфейсе. Только для чтения      |
| Ресаурцереференце     | [Ресаурцереференце](insights-resourcereference.md)                      | Справочные свойства используемого документа, например URL-адрес и тип документа. Только для чтения     |

## <a name="relationships"></a>Связи

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | Объект        | Используется для перехода к использованному элементу. Для вложений в файл используется тип *fileAttachment*. Для связанных вложений используется тип *driveItem*. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
