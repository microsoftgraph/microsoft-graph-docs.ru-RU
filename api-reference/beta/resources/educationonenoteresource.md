---
title: Тип ресурса Едукатиононенотересаурце
description: 'Подкласс объекта Едукатионресаурце. Представляет расположение страницы OneNote.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 60b0e4647f1a601d3cbe206e264f7d288ee2110c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507205"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="ff97b-104">Тип ресурса Едукатиононенотересаурце</span><span class="sxs-lookup"><span data-stu-id="ff97b-104">educationOneNoteResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff97b-105">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="ff97b-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="ff97b-106">Представляет расположение страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="ff97b-106">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="ff97b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff97b-107">Properties</span></span>
| <span data-ttu-id="ff97b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff97b-108">Property</span></span>     | <span data-ttu-id="ff97b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ff97b-109">Type</span></span>   |<span data-ttu-id="ff97b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ff97b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff97b-111">pageUrl</span><span class="sxs-lookup"><span data-stu-id="ff97b-111">pageUrl</span></span>|<span data-ttu-id="ff97b-112">String</span><span class="sxs-lookup"><span data-stu-id="ff97b-112">String</span></span>|<span data-ttu-id="ff97b-113">URL-адрес Microsoft Graph на страницу в OneNote.</span><span class="sxs-lookup"><span data-stu-id="ff97b-113">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="ff97b-114">sectionName</span><span class="sxs-lookup"><span data-stu-id="ff97b-114">sectionName</span></span>|<span data-ttu-id="ff97b-115">String</span><span class="sxs-lookup"><span data-stu-id="ff97b-115">String</span></span>|<span data-ttu-id="ff97b-116">Имя раздела, в который должны копироваться дистрибутивы или скопированы в.</span><span class="sxs-lookup"><span data-stu-id="ff97b-116">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff97b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff97b-117">JSON representation</span></span>

<span data-ttu-id="ff97b-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff97b-118">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonenoteresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
