---
title: Тип ресурса Едукатиононенотересаурце
description: 'Подкласс объекта Едукатионресаурце. Представляет расположение страницы OneNote.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 659ca7f55309499314f94ea62e9433c919856dc6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972651"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="078bd-104">Тип ресурса Едукатиононенотересаурце</span><span class="sxs-lookup"><span data-stu-id="078bd-104">educationOneNoteResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="078bd-105">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="078bd-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="078bd-106">Представляет расположение страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="078bd-106">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="078bd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="078bd-107">Properties</span></span>
| <span data-ttu-id="078bd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="078bd-108">Property</span></span>     | <span data-ttu-id="078bd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="078bd-109">Type</span></span>   |<span data-ttu-id="078bd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="078bd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="078bd-111">pageUrl</span><span class="sxs-lookup"><span data-stu-id="078bd-111">pageUrl</span></span>|<span data-ttu-id="078bd-112">String</span><span class="sxs-lookup"><span data-stu-id="078bd-112">String</span></span>|<span data-ttu-id="078bd-113">URL-адрес Microsoft Graph на страницу в OneNote.</span><span class="sxs-lookup"><span data-stu-id="078bd-113">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="078bd-114">sectionName</span><span class="sxs-lookup"><span data-stu-id="078bd-114">sectionName</span></span>|<span data-ttu-id="078bd-115">String</span><span class="sxs-lookup"><span data-stu-id="078bd-115">String</span></span>|<span data-ttu-id="078bd-116">Имя раздела, в который должны копироваться дистрибутивы или скопированы в.</span><span class="sxs-lookup"><span data-stu-id="078bd-116">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="078bd-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="078bd-117">JSON representation</span></span>

<span data-ttu-id="078bd-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="078bd-118">The following is a JSON representation of the resource.</span></span>

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
