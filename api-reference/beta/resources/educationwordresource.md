---
title: Тип ресурса educationWordResource
description: 'Подкласс educationResource. Это ресурс документа Word. В каталоге **fileResource** , связанный с необходимо отправить файл Word '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: d67f77774b9d3c428fcfd98006115f0459989fdc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948319"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="2d5d4-105">Тип ресурса educationWordResource</span><span class="sxs-lookup"><span data-stu-id="2d5d4-105">educationWordResource resource type</span></span>

> <span data-ttu-id="2d5d4-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2d5d4-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2d5d4-108">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="2d5d4-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="2d5d4-109">Это ресурс документа Word.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-109">This is a Word document resource.</span></span> <span data-ttu-id="2d5d4-110">В каталоге **fileResource** , связанный с назначения или отправки необходимо отправить файл Word.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-110">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="2d5d4-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d5d4-111">Properties</span></span>
| <span data-ttu-id="2d5d4-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d5d4-112">Property</span></span>     | <span data-ttu-id="2d5d4-113">Тип</span><span class="sxs-lookup"><span data-stu-id="2d5d4-113">Type</span></span>   |<span data-ttu-id="2d5d4-114">Описание</span><span class="sxs-lookup"><span data-stu-id="2d5d4-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d5d4-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="2d5d4-115">fileUrl</span></span>|<span data-ttu-id="2d5d4-116">Строка</span><span class="sxs-lookup"><span data-stu-id="2d5d4-116">String</span></span>|<span data-ttu-id="2d5d4-117">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d5d4-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d5d4-118">JSON representation</span></span>

<span data-ttu-id="2d5d4-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d5d4-119">The following is a JSON representation of the resource.</span></span>

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
