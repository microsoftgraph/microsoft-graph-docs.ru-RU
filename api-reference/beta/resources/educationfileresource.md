---
title: Тип ресурса Едукатионфилересаурце
description: Подкласс Едукатионресаурце, представляющий объект File, связанный с назначением или отправкой.  В этом случае файл не является одним из специальных файлов (Word, Excel и т. д.), но это файл, для которого не определена специальная обработка в системе. Файловый ресурс должен храниться в **ресаурцефолдер** , связанном с назначением или отправкой, к которому присоединен этот ресурс.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 15ca31576618f15e64b85d860077785160c25989
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542857"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="a4681-105">Тип ресурса Едукатионфилересаурце</span><span class="sxs-lookup"><span data-stu-id="a4681-105">educationFileResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4681-106">Подкласс [едукатионресаурце](educationresource.md) , представляющий объект File, связанный с назначением или отправкой.</span><span class="sxs-lookup"><span data-stu-id="a4681-106">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="a4681-107">В этом случае файл не является одним из специальных файлов (Word, Excel и т. д.), но это файл, для которого не определена специальная обработка в системе.</span><span class="sxs-lookup"><span data-stu-id="a4681-107">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="a4681-108">Файловый ресурс должен храниться в **ресаурцефолдер** , связанном с назначением или отправкой, к которому присоединен этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="a4681-108">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="a4681-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4681-109">Properties</span></span>
| <span data-ttu-id="a4681-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4681-110">Property</span></span>     | <span data-ttu-id="a4681-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a4681-111">Type</span></span>   |<span data-ttu-id="a4681-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a4681-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4681-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="a4681-113">fileUrl</span></span>|<span data-ttu-id="a4681-114">String</span><span class="sxs-lookup"><span data-stu-id="a4681-114">String</span></span>|<span data-ttu-id="a4681-115">Расположение на диске файлового ресурса.</span><span class="sxs-lookup"><span data-stu-id="a4681-115">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4681-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a4681-116">JSON representation</span></span>

<span data-ttu-id="a4681-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4681-117">The following is a JSON representation of the resource.</span></span>

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
