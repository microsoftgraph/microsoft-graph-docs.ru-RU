---
title: Тип ресурса Букингнамедентити
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3302f364b3f16dc6327b9a1e9ab74161e122ebfb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071782"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="f6a32-104">Тип ресурса Букингнамедентити</span><span class="sxs-lookup"><span data-stu-id="f6a32-104">bookingNamedEntity resource type</span></span>

<span data-ttu-id="f6a32-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6a32-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="f6a32-106">Это базовый тип для сущностей Microsoft Books, предоставляющих отображаемое имя, например, [букингбусинесс](bookingbusiness.md), [букингперсон](bookingperson.md), [букингсервице](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="f6a32-106">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f6a32-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6a32-107">Properties</span></span>
| <span data-ttu-id="f6a32-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6a32-108">Property</span></span>     | <span data-ttu-id="f6a32-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f6a32-109">Type</span></span>   |<span data-ttu-id="f6a32-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f6a32-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6a32-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f6a32-111">displayName</span></span>|<span data-ttu-id="f6a32-112">String</span><span class="sxs-lookup"><span data-stu-id="f6a32-112">String</span></span>|<span data-ttu-id="f6a32-113">Имя производной сущности, которая взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="f6a32-113">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="f6a32-114">id</span><span class="sxs-lookup"><span data-stu-id="f6a32-114">id</span></span>|<span data-ttu-id="f6a32-115">String</span><span class="sxs-lookup"><span data-stu-id="f6a32-115">String</span></span>| <span data-ttu-id="f6a32-116">Идентификатор производной сущности.</span><span class="sxs-lookup"><span data-stu-id="f6a32-116">The ID for the derived entity.</span></span> <span data-ttu-id="f6a32-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6a32-117">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6a32-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="f6a32-118">Relationships</span></span>
<span data-ttu-id="f6a32-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f6a32-119">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f6a32-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6a32-120">JSON representation</span></span>

<span data-ttu-id="f6a32-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6a32-121">The following is a JSON representation of the resource.</span></span>

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


