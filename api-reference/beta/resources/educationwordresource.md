---
title: Тип ресурса Едукатионвордресаурце
description: 'Подкласс объекта Едукатионресаурце. Это ресурс документа Word. Файл Word необходимо отправить в каталоге **филересаурце** , связанном с '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0bd326ea45130da7e7eadb7eb1d21ae3a6c31cce
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972287"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="08f28-105">Тип ресурса Едукатионвордресаурце</span><span class="sxs-lookup"><span data-stu-id="08f28-105">educationWordResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08f28-106">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="08f28-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="08f28-107">Это ресурс документа Word.</span><span class="sxs-lookup"><span data-stu-id="08f28-107">This is a Word document resource.</span></span> <span data-ttu-id="08f28-108">Файл Word необходимо отправить в каталоге **филересаурце** , связанном с назначением или отправкой.</span><span class="sxs-lookup"><span data-stu-id="08f28-108">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="08f28-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="08f28-109">Properties</span></span>
| <span data-ttu-id="08f28-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="08f28-110">Property</span></span>     | <span data-ttu-id="08f28-111">Тип</span><span class="sxs-lookup"><span data-stu-id="08f28-111">Type</span></span>   |<span data-ttu-id="08f28-112">Описание</span><span class="sxs-lookup"><span data-stu-id="08f28-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08f28-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="08f28-113">fileUrl</span></span>|<span data-ttu-id="08f28-114">String</span><span class="sxs-lookup"><span data-stu-id="08f28-114">String</span></span>|<span data-ttu-id="08f28-115">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="08f28-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08f28-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08f28-116">JSON representation</span></span>

<span data-ttu-id="08f28-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08f28-117">The following is a JSON representation of the resource.</span></span>

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
