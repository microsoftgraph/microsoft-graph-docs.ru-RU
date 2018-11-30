---
title: Тип ресурса bookingPerson
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: d20f6ee9e14723a80f012cfffb1e4b8214f89739
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079770"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="363de-104">Тип ресурса bookingPerson</span><span class="sxs-lookup"><span data-stu-id="363de-104">bookingPerson resource type</span></span>

 > <span data-ttu-id="363de-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="363de-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="363de-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="363de-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="363de-107">Это базовый тип для пользователя в business резервирования Майкрософт, который может быть [bookingCustomer](bookingcustomer.md) или [bookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="363de-107">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="363de-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="363de-108">Properties</span></span>
| <span data-ttu-id="363de-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="363de-109">Property</span></span>     | <span data-ttu-id="363de-110">Тип</span><span class="sxs-lookup"><span data-stu-id="363de-110">Type</span></span>   |<span data-ttu-id="363de-111">Описание</span><span class="sxs-lookup"><span data-stu-id="363de-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="363de-112">displayName</span><span class="sxs-lookup"><span data-stu-id="363de-112">displayName</span></span>|<span data-ttu-id="363de-113">String</span><span class="sxs-lookup"><span data-stu-id="363de-113">String</span></span>|<span data-ttu-id="363de-114">Имя для производные сущности, который взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="363de-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="363de-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="363de-115">emailAddress</span></span>|<span data-ttu-id="363de-116">String</span><span class="sxs-lookup"><span data-stu-id="363de-116">String</span></span>|<span data-ttu-id="363de-117">Адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="363de-117">The email address of the person.</span></span>|
|<span data-ttu-id="363de-118">id</span><span class="sxs-lookup"><span data-stu-id="363de-118">id</span></span>|<span data-ttu-id="363de-119">String</span><span class="sxs-lookup"><span data-stu-id="363de-119">String</span></span>| <span data-ttu-id="363de-120">Идентификатор производные сущности.</span><span class="sxs-lookup"><span data-stu-id="363de-120">The ID for the derived entity.</span></span> <span data-ttu-id="363de-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="363de-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="363de-122">Связи</span><span class="sxs-lookup"><span data-stu-id="363de-122">Relationships</span></span>
<span data-ttu-id="363de-123">Нет</span><span class="sxs-lookup"><span data-stu-id="363de-123">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="363de-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="363de-124">JSON representation</span></span>

<span data-ttu-id="363de-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="363de-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingPerson"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->