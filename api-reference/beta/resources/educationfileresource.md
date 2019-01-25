---
title: Тип ресурса educationFileResource
description: Подкласс educationResource, которая представляет собой объект-файл, который связан с назначения или отправки.  В этом случае файл не относится к одному из специальных файлов (Word, Excel и т. д.), но представляет собой файл, для которого не специальная обработка в системе. Файл ресурсов должно храниться в **resourceFolder** , который связан с назначения или отправки, которым связан этот ресурс.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 15ca31576618f15e64b85d860077785160c25989
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520797"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="51d4e-105">Тип ресурса educationFileResource</span><span class="sxs-lookup"><span data-stu-id="51d4e-105">educationFileResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51d4e-106">Подкласс [educationResource](educationresource.md) , которая представляет собой объект-файл, который связан с назначения или отправки.</span><span class="sxs-lookup"><span data-stu-id="51d4e-106">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="51d4e-107">В этом случае файл не относится к одному из специальных файлов (Word, Excel и т. д.), но представляет собой файл, для которого не специальная обработка в системе.</span><span class="sxs-lookup"><span data-stu-id="51d4e-107">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="51d4e-108">Файл ресурсов должно храниться в **resourceFolder** , который связан с назначения или отправки, которым связан этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="51d4e-108">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="51d4e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="51d4e-109">Properties</span></span>
| <span data-ttu-id="51d4e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="51d4e-110">Property</span></span>     | <span data-ttu-id="51d4e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="51d4e-111">Type</span></span>   |<span data-ttu-id="51d4e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="51d4e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51d4e-113">FileURL</span><span class="sxs-lookup"><span data-stu-id="51d4e-113">fileUrl</span></span>|<span data-ttu-id="51d4e-114">String</span><span class="sxs-lookup"><span data-stu-id="51d4e-114">String</span></span>|<span data-ttu-id="51d4e-115">Место на диске файл ресурсов.</span><span class="sxs-lookup"><span data-stu-id="51d4e-115">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51d4e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51d4e-116">JSON representation</span></span>

<span data-ttu-id="51d4e-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51d4e-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
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
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfileresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
