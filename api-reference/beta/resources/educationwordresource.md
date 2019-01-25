---
title: Тип ресурса educationWordResource
description: 'Подкласс educationResource. Это ресурс документа Word. В каталоге **fileResource** , связанный с необходимо отправить файл Word '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9d92b993ab920a894590346bf5fde0ff86c73e8d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529672"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="ab0d6-105">Тип ресурса educationWordResource</span><span class="sxs-lookup"><span data-stu-id="ab0d6-105">educationWordResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab0d6-106">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="ab0d6-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="ab0d6-107">Это ресурс документа Word.</span><span class="sxs-lookup"><span data-stu-id="ab0d6-107">This is a Word document resource.</span></span> <span data-ttu-id="ab0d6-108">В каталоге **fileResource** , связанный с назначения или отправки необходимо отправить файл Word.</span><span class="sxs-lookup"><span data-stu-id="ab0d6-108">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="ab0d6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab0d6-109">Properties</span></span>
| <span data-ttu-id="ab0d6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab0d6-110">Property</span></span>     | <span data-ttu-id="ab0d6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ab0d6-111">Type</span></span>   |<span data-ttu-id="ab0d6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ab0d6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab0d6-113">FileURL</span><span class="sxs-lookup"><span data-stu-id="ab0d6-113">fileUrl</span></span>|<span data-ttu-id="ab0d6-114">String</span><span class="sxs-lookup"><span data-stu-id="ab0d6-114">String</span></span>|<span data-ttu-id="ab0d6-115">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="ab0d6-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab0d6-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab0d6-116">JSON representation</span></span>

<span data-ttu-id="ab0d6-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab0d6-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
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
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationwordresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
