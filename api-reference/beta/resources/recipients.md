---
title: Тип ресурса получателей
description: Ниже представлено описание ресурса в формате JSON.
ms.openlocfilehash: aa620fa920b4f91b2b2214f02c2e75d7a8cbcc4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081536"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="7f195-103">Тип ресурса получателей</span><span class="sxs-lookup"><span data-stu-id="7f195-103">recipients resource type</span></span>

> <span data-ttu-id="7f195-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f195-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f195-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f195-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f195-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f195-106">JSON representation</span></span>

<span data-ttu-id="7f195-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="7f195-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="7f195-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f195-108">Properties</span></span>
| <span data-ttu-id="7f195-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f195-109">Property</span></span>     | <span data-ttu-id="7f195-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7f195-110">Type</span></span>   |<span data-ttu-id="7f195-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7f195-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f195-112">alias</span><span class="sxs-lookup"><span data-stu-id="7f195-112">alias</span></span>|<span data-ttu-id="7f195-113">String</span><span class="sxs-lookup"><span data-stu-id="7f195-113">String</span></span>||
|<span data-ttu-id="7f195-114">email</span><span class="sxs-lookup"><span data-stu-id="7f195-114">email</span></span>|<span data-ttu-id="7f195-115">String</span><span class="sxs-lookup"><span data-stu-id="7f195-115">String</span></span>||
|<span data-ttu-id="7f195-116">objectId</span><span class="sxs-lookup"><span data-stu-id="7f195-116">objectId</span></span>|<span data-ttu-id="7f195-117">String</span><span class="sxs-lookup"><span data-stu-id="7f195-117">String</span></span>||
|<span data-ttu-id="7f195-118">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="7f195-118">permissionIdentityType</span></span>|<span data-ttu-id="7f195-119">String</span><span class="sxs-lookup"><span data-stu-id="7f195-119">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipients resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->