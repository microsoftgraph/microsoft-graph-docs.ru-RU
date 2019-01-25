---
title: Тип ресурса educationPowerPointResource
description: 'Подкласс educationResource. Это ресурсов PowerPoint. Необходимо отправить файл PowerPoint в каталоге **fileResource** , связанный с '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: b61f210ce0efde36b83632268e12d18d3b96b661
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512201"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="d2b90-105">Тип ресурса educationPowerPointResource</span><span class="sxs-lookup"><span data-stu-id="d2b90-105">educationPowerPointResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2b90-106">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="d2b90-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="d2b90-107">Это ресурсов PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="d2b90-107">This is a PowerPoint resource.</span></span> <span data-ttu-id="d2b90-108">В каталоге **fileResource** , связанный с назначения или отправки необходимо отправить файл PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="d2b90-108">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="d2b90-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2b90-109">Properties</span></span>
| <span data-ttu-id="d2b90-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2b90-110">Property</span></span>     | <span data-ttu-id="d2b90-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d2b90-111">Type</span></span>   |<span data-ttu-id="d2b90-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d2b90-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2b90-113">FileURL</span><span class="sxs-lookup"><span data-stu-id="d2b90-113">fileUrl</span></span>|<span data-ttu-id="d2b90-114">String</span><span class="sxs-lookup"><span data-stu-id="d2b90-114">String</span></span>|<span data-ttu-id="d2b90-115">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="d2b90-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2b90-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2b90-116">JSON representation</span></span>

<span data-ttu-id="d2b90-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2b90-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
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
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerpointresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
