---
title: Тип ресурса educationOneNoteResource
description: 'Подкласс educationResource. Представляет расположение страницы OneNote.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b10bef551cdc2dd29a8a20c69d2c4657ee66af4e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927921"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="9fb39-104">Тип ресурса educationOneNoteResource</span><span class="sxs-lookup"><span data-stu-id="9fb39-104">educationOneNoteResource resource type</span></span>

> <span data-ttu-id="9fb39-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9fb39-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fb39-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fb39-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9fb39-107">Подкласс [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="9fb39-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="9fb39-108">Представляет расположение страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="9fb39-108">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="9fb39-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fb39-109">Properties</span></span>
| <span data-ttu-id="9fb39-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fb39-110">Property</span></span>     | <span data-ttu-id="9fb39-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9fb39-111">Type</span></span>   |<span data-ttu-id="9fb39-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9fb39-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fb39-113">pageUrl</span><span class="sxs-lookup"><span data-stu-id="9fb39-113">pageUrl</span></span>|<span data-ttu-id="9fb39-114">Строка</span><span class="sxs-lookup"><span data-stu-id="9fb39-114">String</span></span>|<span data-ttu-id="9fb39-115">URL-адрес графическое представление Microsoft на страницу OneNote.</span><span class="sxs-lookup"><span data-stu-id="9fb39-115">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="9fb39-116">sectionName</span><span class="sxs-lookup"><span data-stu-id="9fb39-116">sectionName</span></span>|<span data-ttu-id="9fb39-117">Строка</span><span class="sxs-lookup"><span data-stu-id="9fb39-117">String</span></span>|<span data-ttu-id="9fb39-118">Имя раздела, который следует скопировать в или были скопированы в распределения.</span><span class="sxs-lookup"><span data-stu-id="9fb39-118">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fb39-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fb39-119">JSON representation</span></span>

<span data-ttu-id="9fb39-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fb39-120">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
