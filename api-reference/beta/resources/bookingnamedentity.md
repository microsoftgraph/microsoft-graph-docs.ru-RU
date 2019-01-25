---
title: Тип ресурса bookingNamedEntity
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1cee769181fdf8dce694050cdbc2658fdf29ece4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515323"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="54c1a-104">Тип ресурса bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="54c1a-104">bookingNamedEntity resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="54c1a-105">Это базовый тип для резервирования Microsoft сущностей, которые обеспечивают отображаемое имя, например, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="54c1a-105">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="54c1a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="54c1a-106">Properties</span></span>
| <span data-ttu-id="54c1a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="54c1a-107">Property</span></span>     | <span data-ttu-id="54c1a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="54c1a-108">Type</span></span>   |<span data-ttu-id="54c1a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="54c1a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54c1a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="54c1a-110">displayName</span></span>|<span data-ttu-id="54c1a-111">String</span><span class="sxs-lookup"><span data-stu-id="54c1a-111">String</span></span>|<span data-ttu-id="54c1a-112">Имя для производные сущности, который взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="54c1a-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="54c1a-113">id</span><span class="sxs-lookup"><span data-stu-id="54c1a-113">id</span></span>|<span data-ttu-id="54c1a-114">String</span><span class="sxs-lookup"><span data-stu-id="54c1a-114">String</span></span>| <span data-ttu-id="54c1a-115">Идентификатор производные сущности.</span><span class="sxs-lookup"><span data-stu-id="54c1a-115">The ID for the derived entity.</span></span> <span data-ttu-id="54c1a-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="54c1a-116">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54c1a-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="54c1a-117">Relationships</span></span>
<span data-ttu-id="54c1a-118">Нет</span><span class="sxs-lookup"><span data-stu-id="54c1a-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="54c1a-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54c1a-119">JSON representation</span></span>

<span data-ttu-id="54c1a-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54c1a-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingNamedEntity"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingnamedentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
