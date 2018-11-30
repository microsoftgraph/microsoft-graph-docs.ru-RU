---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: contentTypeOrder
ms.openlocfilehash: a6b83627d86bbb35357f03dbee3605c6fb1df7a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081784"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="74a29-102">Тип ресурса contentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="74a29-102">ContentTypeOrder resource type</span></span>

> <span data-ttu-id="74a29-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74a29-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74a29-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74a29-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74a29-105">Ресурс **contentTypeOrder** указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="74a29-105">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74a29-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="74a29-106">JSON representation</span></span>

<span data-ttu-id="74a29-107">Ниже показано представление ресурса **contentTypeOrder** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74a29-107">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="74a29-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="74a29-108">Properties</span></span>

| <span data-ttu-id="74a29-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="74a29-109">Property name</span></span> | <span data-ttu-id="74a29-110">Тип</span><span class="sxs-lookup"><span data-stu-id="74a29-110">Type</span></span>    | <span data-ttu-id="74a29-111">Описание</span><span class="sxs-lookup"><span data-stu-id="74a29-111">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="74a29-112">**default**</span><span class="sxs-lookup"><span data-stu-id="74a29-112">**default**</span></span>   | <span data-ttu-id="74a29-113">логический</span><span class="sxs-lookup"><span data-stu-id="74a29-113">boolean</span></span> | <span data-ttu-id="74a29-114">Указывает, используется ли этот тип контента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="74a29-114">Whether this is the default Content Type</span></span>
| <span data-ttu-id="74a29-115">**position**</span><span class="sxs-lookup"><span data-stu-id="74a29-115">**position**</span></span>  | <span data-ttu-id="74a29-116">Int32</span><span class="sxs-lookup"><span data-stu-id="74a29-116">Int32</span></span>   | <span data-ttu-id="74a29-117">Указывает позицию, в которой тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="74a29-117">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
