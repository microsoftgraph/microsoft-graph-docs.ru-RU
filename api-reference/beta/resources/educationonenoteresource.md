---
title: Тип ресурса Едукатиононенотересаурце
description: 'Подкласс объекта Едукатионресаурце. Представляет расположение страницы OneNote.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 890adf73330fd6ac9b5642c94b2995eda8d625bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055650"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="fe090-104">Тип ресурса Едукатиононенотересаурце</span><span class="sxs-lookup"><span data-stu-id="fe090-104">educationOneNoteResource resource type</span></span>

<span data-ttu-id="fe090-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe090-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe090-106">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="fe090-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="fe090-107">Представляет расположение страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="fe090-107">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="fe090-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe090-108">Properties</span></span>
| <span data-ttu-id="fe090-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe090-109">Property</span></span>     | <span data-ttu-id="fe090-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fe090-110">Type</span></span>   |<span data-ttu-id="fe090-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fe090-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe090-112">pageUrl</span><span class="sxs-lookup"><span data-stu-id="fe090-112">pageUrl</span></span>|<span data-ttu-id="fe090-113">String</span><span class="sxs-lookup"><span data-stu-id="fe090-113">String</span></span>|<span data-ttu-id="fe090-114">URL-адрес Microsoft Graph на страницу в OneNote.</span><span class="sxs-lookup"><span data-stu-id="fe090-114">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="fe090-115">sectionName</span><span class="sxs-lookup"><span data-stu-id="fe090-115">sectionName</span></span>|<span data-ttu-id="fe090-116">String</span><span class="sxs-lookup"><span data-stu-id="fe090-116">String</span></span>|<span data-ttu-id="fe090-117">Имя раздела, в который должны копироваться дистрибутивы или скопированы в.</span><span class="sxs-lookup"><span data-stu-id="fe090-117">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe090-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fe090-118">JSON representation</span></span>

<span data-ttu-id="fe090-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe090-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


