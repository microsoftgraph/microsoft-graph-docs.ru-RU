---
title: Тип ресурса educationPowerPointResource
description: 'Подкласс educationResource. Это ресурсов PowerPoint. Необходимо отправить файл PowerPoint в каталоге **fileResource** , связанный с '
ms.openlocfilehash: a83a78449ecb7c64f62557ddfa642ab02b55c206
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080209"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="32685-105">Тип ресурса educationPowerPointResource</span><span class="sxs-lookup"><span data-stu-id="32685-105">educationPowerPointResource resource type</span></span>

> <span data-ttu-id="32685-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="32685-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32685-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32685-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32685-108">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="32685-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="32685-109">Это ресурсов PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="32685-109">This is a PowerPoint resource.</span></span> <span data-ttu-id="32685-110">В каталоге **fileResource** , связанный с назначения или отправки необходимо отправить файл PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="32685-110">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="32685-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="32685-111">Properties</span></span>
| <span data-ttu-id="32685-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="32685-112">Property</span></span>     | <span data-ttu-id="32685-113">Тип</span><span class="sxs-lookup"><span data-stu-id="32685-113">Type</span></span>   |<span data-ttu-id="32685-114">Description</span><span class="sxs-lookup"><span data-stu-id="32685-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32685-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="32685-115">fileUrl</span></span>|<span data-ttu-id="32685-116">String</span><span class="sxs-lookup"><span data-stu-id="32685-116">String</span></span>|<span data-ttu-id="32685-117">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="32685-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32685-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32685-118">JSON representation</span></span>

<span data-ttu-id="32685-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32685-119">The following is a JSON representation of the resource.</span></span>

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