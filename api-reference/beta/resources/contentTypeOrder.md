---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: contentTypeOrder
localization_priority: Normal
ms.openlocfilehash: ad25ececa9a32a1aaab7f25bf909f7e1ef640dec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825755"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="2384b-102">Тип ресурса contentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="2384b-102">ContentTypeOrder resource type</span></span>

> <span data-ttu-id="2384b-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2384b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2384b-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2384b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2384b-105">Ресурс **contentTypeOrder** указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="2384b-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2384b-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2384b-106">JSON representation</span></span>

<span data-ttu-id="2384b-107">Ниже показано представление ресурса **contentTypeOrder** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2384b-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="2384b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2384b-108">Properties</span></span>

| <span data-ttu-id="2384b-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2384b-109">Property name</span></span> | <span data-ttu-id="2384b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2384b-110">Type</span></span>    | <span data-ttu-id="2384b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2384b-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="2384b-112">**default**</span><span class="sxs-lookup"><span data-stu-id="2384b-112">**default**</span></span>   | <span data-ttu-id="2384b-113">логический</span><span class="sxs-lookup"><span data-stu-id="2384b-113">boolean</span></span> | <span data-ttu-id="2384b-114">Указывает, используется ли этот тип контента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2384b-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="2384b-115">**position**</span><span class="sxs-lookup"><span data-stu-id="2384b-115">**position**</span></span>  | <span data-ttu-id="2384b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="2384b-116">Int32</span></span>   | <span data-ttu-id="2384b-117">Указывает позицию, в которой тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="2384b-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
