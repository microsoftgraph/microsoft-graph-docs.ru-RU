---
title: Тип ресурса Едукатиононенотересаурце
description: 'Подкласс объекта Едукатионресаурце. Представляет расположение страницы OneNote.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: cec9c2f2a092175c7ccecaa09c7b8b510000205c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501551"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="418ac-104">Тип ресурса Едукатиононенотересаурце</span><span class="sxs-lookup"><span data-stu-id="418ac-104">educationOneNoteResource resource type</span></span>

<span data-ttu-id="418ac-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="418ac-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="418ac-106">Подкласс объекта [едукатионресаурце](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="418ac-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="418ac-107">Представляет расположение страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="418ac-107">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="418ac-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="418ac-108">Properties</span></span>
| <span data-ttu-id="418ac-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="418ac-109">Property</span></span>     | <span data-ttu-id="418ac-110">Тип</span><span class="sxs-lookup"><span data-stu-id="418ac-110">Type</span></span>   |<span data-ttu-id="418ac-111">Описание</span><span class="sxs-lookup"><span data-stu-id="418ac-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="418ac-112">pageUrl</span><span class="sxs-lookup"><span data-stu-id="418ac-112">pageUrl</span></span>|<span data-ttu-id="418ac-113">String</span><span class="sxs-lookup"><span data-stu-id="418ac-113">String</span></span>|<span data-ttu-id="418ac-114">URL-адрес Microsoft Graph на страницу в OneNote.</span><span class="sxs-lookup"><span data-stu-id="418ac-114">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="418ac-115">sectionName</span><span class="sxs-lookup"><span data-stu-id="418ac-115">sectionName</span></span>|<span data-ttu-id="418ac-116">String</span><span class="sxs-lookup"><span data-stu-id="418ac-116">String</span></span>|<span data-ttu-id="418ac-117">Имя раздела, в который должны копироваться дистрибутивы или скопированы в.</span><span class="sxs-lookup"><span data-stu-id="418ac-117">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="418ac-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="418ac-118">JSON representation</span></span>

<span data-ttu-id="418ac-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="418ac-119">The following is a JSON representation of the resource.</span></span>

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
