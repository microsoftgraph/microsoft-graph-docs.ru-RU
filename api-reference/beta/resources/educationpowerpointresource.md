---
title: Тип ресурса educationPowerPointResource
description: 'Подкласс educationResource. Это ресурсов PowerPoint. Необходимо отправить файл PowerPoint в каталоге **fileResource** , связанный с '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f92d74d8e3dfb7cebcecd607bbd4bd8e2f3b43da
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940668"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="3f08b-105">Тип ресурса educationPowerPointResource</span><span class="sxs-lookup"><span data-stu-id="3f08b-105">educationPowerPointResource resource type</span></span>

> <span data-ttu-id="3f08b-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3f08b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f08b-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f08b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3f08b-108">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="3f08b-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="3f08b-109">Это ресурсов PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="3f08b-109">This is a PowerPoint resource.</span></span> <span data-ttu-id="3f08b-110">В каталоге **fileResource** , связанный с назначения или отправки необходимо отправить файл PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="3f08b-110">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="3f08b-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f08b-111">Properties</span></span>
| <span data-ttu-id="3f08b-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f08b-112">Property</span></span>     | <span data-ttu-id="3f08b-113">Тип</span><span class="sxs-lookup"><span data-stu-id="3f08b-113">Type</span></span>   |<span data-ttu-id="3f08b-114">Описание</span><span class="sxs-lookup"><span data-stu-id="3f08b-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f08b-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="3f08b-115">fileUrl</span></span>|<span data-ttu-id="3f08b-116">Строка</span><span class="sxs-lookup"><span data-stu-id="3f08b-116">String</span></span>|<span data-ttu-id="3f08b-117">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="3f08b-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f08b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f08b-118">JSON representation</span></span>

<span data-ttu-id="3f08b-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f08b-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
