---
title: Тип ресурса Букингнамедентити
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: aa200d2d7aee435f6bb156cc857d471c222e740d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453666"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="e6480-104">Тип ресурса Букингнамедентити</span><span class="sxs-lookup"><span data-stu-id="e6480-104">bookingNamedEntity resource type</span></span>

<span data-ttu-id="e6480-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6480-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="e6480-106">Это базовый тип для сущностей Microsoft Books, предоставляющих отображаемое имя, например, [букингбусинесс](bookingbusiness.md), [букингперсон](bookingperson.md), [букингсервице](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="e6480-106">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e6480-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6480-107">Properties</span></span>
| <span data-ttu-id="e6480-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6480-108">Property</span></span>     | <span data-ttu-id="e6480-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e6480-109">Type</span></span>   |<span data-ttu-id="e6480-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e6480-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6480-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e6480-111">displayName</span></span>|<span data-ttu-id="e6480-112">Строка</span><span class="sxs-lookup"><span data-stu-id="e6480-112">String</span></span>|<span data-ttu-id="e6480-113">Имя производной сущности, которая взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="e6480-113">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="e6480-114">id</span><span class="sxs-lookup"><span data-stu-id="e6480-114">id</span></span>|<span data-ttu-id="e6480-115">String</span><span class="sxs-lookup"><span data-stu-id="e6480-115">String</span></span>| <span data-ttu-id="e6480-116">Идентификатор производной сущности.</span><span class="sxs-lookup"><span data-stu-id="e6480-116">The ID for the derived entity.</span></span> <span data-ttu-id="e6480-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6480-117">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6480-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="e6480-118">Relationships</span></span>
<span data-ttu-id="e6480-119">Нет</span><span class="sxs-lookup"><span data-stu-id="e6480-119">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6480-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6480-120">JSON representation</span></span>

<span data-ttu-id="e6480-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6480-121">The following is a JSON representation of the resource.</span></span>

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
