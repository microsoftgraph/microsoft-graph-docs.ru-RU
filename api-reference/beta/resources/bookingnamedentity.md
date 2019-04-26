---
title: Тип ресурса Букингнамедентити
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: c9dc533360d28fc470a3a00528a20cea1b7ea551
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328194"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="19cfd-104">Тип ресурса Букингнамедентити</span><span class="sxs-lookup"><span data-stu-id="19cfd-104">bookingNamedEntity resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="19cfd-105">Это базовый тип для сущностей Microsoft Books, предоставляющих отображаемое имя, например, [букингбусинесс](bookingbusiness.md), [букингперсон](bookingperson.md), [букингсервице](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="19cfd-105">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="19cfd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="19cfd-106">Properties</span></span>
| <span data-ttu-id="19cfd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="19cfd-107">Property</span></span>     | <span data-ttu-id="19cfd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="19cfd-108">Type</span></span>   |<span data-ttu-id="19cfd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="19cfd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19cfd-110">displayName</span><span class="sxs-lookup"><span data-stu-id="19cfd-110">displayName</span></span>|<span data-ttu-id="19cfd-111">String</span><span class="sxs-lookup"><span data-stu-id="19cfd-111">String</span></span>|<span data-ttu-id="19cfd-112">Имя производной сущности, которая взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="19cfd-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="19cfd-113">id</span><span class="sxs-lookup"><span data-stu-id="19cfd-113">id</span></span>|<span data-ttu-id="19cfd-114">String</span><span class="sxs-lookup"><span data-stu-id="19cfd-114">String</span></span>| <span data-ttu-id="19cfd-115">Идентификатор производной сущности.</span><span class="sxs-lookup"><span data-stu-id="19cfd-115">The ID for the derived entity.</span></span> <span data-ttu-id="19cfd-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19cfd-116">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19cfd-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="19cfd-117">Relationships</span></span>
<span data-ttu-id="19cfd-118">Нет</span><span class="sxs-lookup"><span data-stu-id="19cfd-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="19cfd-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19cfd-119">JSON representation</span></span>

<span data-ttu-id="19cfd-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19cfd-120">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
