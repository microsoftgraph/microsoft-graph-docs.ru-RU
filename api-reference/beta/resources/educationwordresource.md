---
title: Тип ресурса educationWordResource
description: 'Подкласс educationResource. Это ресурс документа Word. В каталоге **fileResource** , связанный с необходимо отправить файл Word '
ms.openlocfilehash: 28df3278a0d97f440014c342d592d2701b348d94
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080202"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="710dd-105">Тип ресурса educationWordResource</span><span class="sxs-lookup"><span data-stu-id="710dd-105">educationWordResource resource type</span></span>

> <span data-ttu-id="710dd-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="710dd-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="710dd-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="710dd-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="710dd-108">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="710dd-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="710dd-109">Это ресурс документа Word.</span><span class="sxs-lookup"><span data-stu-id="710dd-109">This is a Word document resource.</span></span> <span data-ttu-id="710dd-110">В каталоге **fileResource** , связанный с назначения или отправки необходимо отправить файл Word.</span><span class="sxs-lookup"><span data-stu-id="710dd-110">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="710dd-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="710dd-111">Properties</span></span>
| <span data-ttu-id="710dd-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="710dd-112">Property</span></span>     | <span data-ttu-id="710dd-113">Тип</span><span class="sxs-lookup"><span data-stu-id="710dd-113">Type</span></span>   |<span data-ttu-id="710dd-114">Description</span><span class="sxs-lookup"><span data-stu-id="710dd-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="710dd-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="710dd-115">fileUrl</span></span>|<span data-ttu-id="710dd-116">String</span><span class="sxs-lookup"><span data-stu-id="710dd-116">String</span></span>|<span data-ttu-id="710dd-117">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="710dd-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="710dd-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="710dd-118">JSON representation</span></span>

<span data-ttu-id="710dd-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="710dd-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->