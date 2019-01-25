---
title: Тип ресурса educationExcelResource
description: 'Подкласс educationResource. Этот тип ресурсов представляет документа в формате Excel.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 14d7823f166ca12d202a6561bc9fe7b158ab7476
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522422"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="ab56b-104">Тип ресурса educationExcelResource</span><span class="sxs-lookup"><span data-stu-id="ab56b-104">educationExcelResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab56b-105">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="ab56b-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="ab56b-106">Этот тип ресурсов представляет документа в формате Excel.</span><span class="sxs-lookup"><span data-stu-id="ab56b-106">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="ab56b-107">**Примечание:** Файл Excel должен находиться в папку ресурсов, связанного с объектом назначения или отправки, к которой принадлежит ресурс.</span><span class="sxs-lookup"><span data-stu-id="ab56b-107">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="ab56b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab56b-108">Properties</span></span>
| <span data-ttu-id="ab56b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab56b-109">Property</span></span>     | <span data-ttu-id="ab56b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ab56b-110">Type</span></span>   |<span data-ttu-id="ab56b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ab56b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab56b-112">FileURL</span><span class="sxs-lookup"><span data-stu-id="ab56b-112">fileUrl</span></span>|<span data-ttu-id="ab56b-113">String</span><span class="sxs-lookup"><span data-stu-id="ab56b-113">String</span></span>|<span data-ttu-id="ab56b-114">Указатель на объект файла Excel.</span><span class="sxs-lookup"><span data-stu-id="ab56b-114">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab56b-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab56b-115">JSON representation</span></span>

<span data-ttu-id="ab56b-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab56b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationexcelresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
