---
title: Тип ресурса educationWordResource
description: 'Подкласс educationResource. Это ресурс документа Word. В каталоге **fileResource** , связанный с необходимо отправить файл Word '
localization_priority: Normal
ms.openlocfilehash: 0fa366a6fb6de70d10a010cf5e0e11ffd26a3b94
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805140"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="fc05a-105">Тип ресурса educationWordResource</span><span class="sxs-lookup"><span data-stu-id="fc05a-105">educationWordResource resource type</span></span>

> <span data-ttu-id="fc05a-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc05a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc05a-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc05a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fc05a-108">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="fc05a-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="fc05a-109">Это ресурс документа Word.</span><span class="sxs-lookup"><span data-stu-id="fc05a-109">This is a Word document resource.</span></span> <span data-ttu-id="fc05a-110">В каталоге **fileResource** , связанный с назначения или отправки необходимо отправить файл Word.</span><span class="sxs-lookup"><span data-stu-id="fc05a-110">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="fc05a-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc05a-111">Properties</span></span>
| <span data-ttu-id="fc05a-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc05a-112">Property</span></span>     | <span data-ttu-id="fc05a-113">Тип</span><span class="sxs-lookup"><span data-stu-id="fc05a-113">Type</span></span>   |<span data-ttu-id="fc05a-114">Описание</span><span class="sxs-lookup"><span data-stu-id="fc05a-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc05a-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="fc05a-115">fileUrl</span></span>|<span data-ttu-id="fc05a-116">Строка</span><span class="sxs-lookup"><span data-stu-id="fc05a-116">String</span></span>|<span data-ttu-id="fc05a-117">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="fc05a-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc05a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc05a-118">JSON representation</span></span>

<span data-ttu-id="fc05a-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc05a-119">The following is a JSON representation of the resource.</span></span>

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
