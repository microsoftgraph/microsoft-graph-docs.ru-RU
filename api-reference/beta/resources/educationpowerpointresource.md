---
title: Тип ресурса Едукатионповерпоинтресаурце
description: 'Подкласс объекта Едукатионресаурце. Это ресурс PowerPoint. Файл PowerPoint необходимо отправить в каталоге **филересаурце** , связанном с '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 1404d054ab26527c617ed8fce8ad03c58f520f3c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340471"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="7cd3a-105">Тип ресурса Едукатионповерпоинтресаурце</span><span class="sxs-lookup"><span data-stu-id="7cd3a-105">educationPowerPointResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cd3a-106">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="7cd3a-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="7cd3a-107">Это ресурс PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="7cd3a-107">This is a PowerPoint resource.</span></span> <span data-ttu-id="7cd3a-108">Файл PowerPoint необходимо отправить в каталоге **филересаурце** , связанном с назначением или отправкой.</span><span class="sxs-lookup"><span data-stu-id="7cd3a-108">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="7cd3a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7cd3a-109">Properties</span></span>
| <span data-ttu-id="7cd3a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7cd3a-110">Property</span></span>     | <span data-ttu-id="7cd3a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7cd3a-111">Type</span></span>   |<span data-ttu-id="7cd3a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7cd3a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cd3a-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="7cd3a-113">fileUrl</span></span>|<span data-ttu-id="7cd3a-114">String</span><span class="sxs-lookup"><span data-stu-id="7cd3a-114">String</span></span>|<span data-ttu-id="7cd3a-115">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="7cd3a-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cd3a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7cd3a-116">JSON representation</span></span>

<span data-ttu-id="7cd3a-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cd3a-117">The following is a JSON representation of the resource.</span></span>

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
