---
title: Тип ресурса получателей
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: c0afde5b7bd427389b5b81be055781dfaff194e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829587"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="bb8cf-103">Тип ресурса получателей</span><span class="sxs-lookup"><span data-stu-id="bb8cf-103">recipients resource type</span></span>

> <span data-ttu-id="bb8cf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bb8cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb8cf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb8cf-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb8cf-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb8cf-106">JSON representation</span></span>

<span data-ttu-id="bb8cf-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="bb8cf-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipients"
}-->

```json
{
  "alias": "string",
  "email": "string",
  "objectId": "string",
  "permissionIdentityType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="bb8cf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb8cf-108">Properties</span></span>
| <span data-ttu-id="bb8cf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb8cf-109">Property</span></span>     | <span data-ttu-id="bb8cf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bb8cf-110">Type</span></span>   |<span data-ttu-id="bb8cf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bb8cf-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb8cf-112">alias</span><span class="sxs-lookup"><span data-stu-id="bb8cf-112">alias</span></span>|<span data-ttu-id="bb8cf-113">String</span><span class="sxs-lookup"><span data-stu-id="bb8cf-113">String</span></span>||
|<span data-ttu-id="bb8cf-114">email</span><span class="sxs-lookup"><span data-stu-id="bb8cf-114">email</span></span>|<span data-ttu-id="bb8cf-115">String</span><span class="sxs-lookup"><span data-stu-id="bb8cf-115">String</span></span>||
|<span data-ttu-id="bb8cf-116">objectId</span><span class="sxs-lookup"><span data-stu-id="bb8cf-116">objectId</span></span>|<span data-ttu-id="bb8cf-117">String</span><span class="sxs-lookup"><span data-stu-id="bb8cf-117">String</span></span>||
|<span data-ttu-id="bb8cf-118">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="bb8cf-118">permissionIdentityType</span></span>|<span data-ttu-id="bb8cf-119">String</span><span class="sxs-lookup"><span data-stu-id="bb8cf-119">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipients resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
