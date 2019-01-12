---
title: Тип ресурса educationFileResource
description: Подкласс educationResource, которая представляет собой объект-файл, который связан с назначения или отправки.  В этом случае файл не относится к одному из специальных файлов (Word, Excel и т. д.), но представляет собой файл, для которого не специальная обработка в системе. Файл ресурсов должно храниться в **resourceFolder** , который связан с назначения или отправки, которым связан этот ресурс.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 96c03dc1571e0f8686116f169706aa35003f92a3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953660"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="1e705-105">Тип ресурса educationFileResource</span><span class="sxs-lookup"><span data-stu-id="1e705-105">educationFileResource resource type</span></span>

> <span data-ttu-id="1e705-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1e705-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e705-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e705-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e705-108">Подкласс [educationResource](educationresource.md) , которая представляет собой объект-файл, который связан с назначения или отправки.</span><span class="sxs-lookup"><span data-stu-id="1e705-108">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="1e705-109">В этом случае файл не относится к одному из специальных файлов (Word, Excel и т. д.), но представляет собой файл, для которого не специальная обработка в системе.</span><span class="sxs-lookup"><span data-stu-id="1e705-109">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="1e705-110">Файл ресурсов должно храниться в **resourceFolder** , который связан с назначения или отправки, которым связан этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="1e705-110">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="1e705-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e705-111">Properties</span></span>
| <span data-ttu-id="1e705-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e705-112">Property</span></span>     | <span data-ttu-id="1e705-113">Тип</span><span class="sxs-lookup"><span data-stu-id="1e705-113">Type</span></span>   |<span data-ttu-id="1e705-114">Описание</span><span class="sxs-lookup"><span data-stu-id="1e705-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e705-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="1e705-115">fileUrl</span></span>|<span data-ttu-id="1e705-116">Строка</span><span class="sxs-lookup"><span data-stu-id="1e705-116">String</span></span>|<span data-ttu-id="1e705-117">Место на диске файл ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1e705-117">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e705-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e705-118">JSON representation</span></span>

<span data-ttu-id="1e705-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e705-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
