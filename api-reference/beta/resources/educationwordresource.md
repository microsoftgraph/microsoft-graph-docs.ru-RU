---
title: Тип ресурса Едукатионвордресаурце
description: 'Подкласс объекта Едукатионресаурце. Это ресурс документа Word. Файл Word необходимо отправить в каталоге **филересаурце** , связанном с '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 69339b3192a37c286f430a4b65c1aee64a9cbab5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055570"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="29a37-105">Тип ресурса Едукатионвордресаурце</span><span class="sxs-lookup"><span data-stu-id="29a37-105">educationWordResource resource type</span></span>

<span data-ttu-id="29a37-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29a37-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29a37-107">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="29a37-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="29a37-108">Это ресурс документа Word.</span><span class="sxs-lookup"><span data-stu-id="29a37-108">This is a Word document resource.</span></span> <span data-ttu-id="29a37-109">Файл Word необходимо отправить в каталоге **филересаурце** , связанном с назначением или отправкой.</span><span class="sxs-lookup"><span data-stu-id="29a37-109">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="29a37-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="29a37-110">Properties</span></span>
| <span data-ttu-id="29a37-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="29a37-111">Property</span></span>     | <span data-ttu-id="29a37-112">Тип</span><span class="sxs-lookup"><span data-stu-id="29a37-112">Type</span></span>   |<span data-ttu-id="29a37-113">Описание</span><span class="sxs-lookup"><span data-stu-id="29a37-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29a37-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="29a37-114">fileUrl</span></span>|<span data-ttu-id="29a37-115">String</span><span class="sxs-lookup"><span data-stu-id="29a37-115">String</span></span>|<span data-ttu-id="29a37-116">Расположение файла на диске.</span><span class="sxs-lookup"><span data-stu-id="29a37-116">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29a37-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="29a37-117">JSON representation</span></span>

<span data-ttu-id="29a37-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29a37-118">The following is a JSON representation of the resource.</span></span>

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


