---
title: Тип ресурса Едукатионповерпоинтресаурце
description: 'Подкласс объекта Едукатионресаурце. Это ресурс PowerPoint. Файл PowerPoint необходимо отправить в каталоге **филересаурце** , связанном с '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 72ab3435ed30602bbd9b2fadf9a6f4d0879e9198
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972607"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="4c776-105">Тип ресурса Едукатионповерпоинтресаурце</span><span class="sxs-lookup"><span data-stu-id="4c776-105">educationPowerPointResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c776-106">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="4c776-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="4c776-107">Это ресурс PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="4c776-107">This is a PowerPoint resource.</span></span> <span data-ttu-id="4c776-108">Файл PowerPoint необходимо отправить в каталоге **филересаурце** , связанном с назначением или отправкой.</span><span class="sxs-lookup"><span data-stu-id="4c776-108">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="4c776-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c776-109">Properties</span></span>
| <span data-ttu-id="4c776-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c776-110">Property</span></span>     | <span data-ttu-id="4c776-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4c776-111">Type</span></span>   |<span data-ttu-id="4c776-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4c776-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c776-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="4c776-113">fileUrl</span></span>|<span data-ttu-id="4c776-114">String</span><span class="sxs-lookup"><span data-stu-id="4c776-114">String</span></span>|<span data-ttu-id="4c776-115">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="4c776-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c776-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c776-116">JSON representation</span></span>

<span data-ttu-id="4c776-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c776-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
