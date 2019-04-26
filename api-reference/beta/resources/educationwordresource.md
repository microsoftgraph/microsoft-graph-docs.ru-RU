---
title: Тип ресурса Едукатионвордресаурце
description: 'Подкласс объекта Едукатионресаурце. Это ресурс документа Word. Файл Word необходимо отправить в каталоге **филересаурце** , связанном с '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9bd9af22c141991efd85fc240a002b5c7a0eac3b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340208"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="66e25-105">Тип ресурса Едукатионвордресаурце</span><span class="sxs-lookup"><span data-stu-id="66e25-105">educationWordResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66e25-106">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="66e25-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="66e25-107">Это ресурс документа Word.</span><span class="sxs-lookup"><span data-stu-id="66e25-107">This is a Word document resource.</span></span> <span data-ttu-id="66e25-108">Файл Word необходимо отправить в каталоге **филересаурце** , связанном с назначением или отправкой.</span><span class="sxs-lookup"><span data-stu-id="66e25-108">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="66e25-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="66e25-109">Properties</span></span>
| <span data-ttu-id="66e25-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="66e25-110">Property</span></span>     | <span data-ttu-id="66e25-111">Тип</span><span class="sxs-lookup"><span data-stu-id="66e25-111">Type</span></span>   |<span data-ttu-id="66e25-112">Описание</span><span class="sxs-lookup"><span data-stu-id="66e25-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66e25-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="66e25-113">fileUrl</span></span>|<span data-ttu-id="66e25-114">String</span><span class="sxs-lookup"><span data-stu-id="66e25-114">String</span></span>|<span data-ttu-id="66e25-115">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="66e25-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66e25-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66e25-116">JSON representation</span></span>

<span data-ttu-id="66e25-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66e25-117">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
