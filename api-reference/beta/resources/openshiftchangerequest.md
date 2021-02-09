---
title: Тип ресурса openShiftChangeRequest
description: Представляет тип запроса на смену для утверждения открытой смены в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e141dcb6657c9efc7d751b1713aa8b53d79c9264
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161431"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="d28df-103">Тип ресурса openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="d28df-103">openShiftChangeRequest resource type</span></span>

<span data-ttu-id="d28df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d28df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d28df-105">Представляет тип запроса на смену для утверждения [openshift](../resources/openshift.md) в [расписании.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="d28df-105">Represents a type of shift request to claim an [openshift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d28df-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d28df-106">Methods</span></span>

| <span data-ttu-id="d28df-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d28df-107">Method</span></span>       | <span data-ttu-id="d28df-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d28df-108">Return Type</span></span> | <span data-ttu-id="d28df-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d28df-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d28df-110">Создание</span><span class="sxs-lookup"><span data-stu-id="d28df-110">Create</span></span>](../api/openshiftchangerequest-post.md) | [<span data-ttu-id="d28df-111">openshiftchangerequest</span><span class="sxs-lookup"><span data-stu-id="d28df-111">openshiftchangerequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="d28df-112">Создание экземпляра объекта openshiftchangerequest.</span><span class="sxs-lookup"><span data-stu-id="d28df-112">Create an instance of an openshiftchangerequest object.</span></span> |
| [<span data-ttu-id="d28df-113">Список</span><span class="sxs-lookup"><span data-stu-id="d28df-113">List</span></span>](../api/openshiftchangerequest-list.md) | <span data-ttu-id="d28df-114">Коллекция [openshiftchangerequest](openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="d28df-114">Collection of [openshiftchangerequest](openshiftchangerequest.md)</span></span> | <span data-ttu-id="d28df-115">Список свойств и связей объектов **openShiftChangeRequest** в команде.</span><span class="sxs-lookup"><span data-stu-id="d28df-115">List the properties and relationships of **openShiftChangeRequest** objects in a team.</span></span> |
| [<span data-ttu-id="d28df-116">Получение</span><span class="sxs-lookup"><span data-stu-id="d28df-116">Get</span></span>](../api/openshiftchangerequest-get.md) | [<span data-ttu-id="d28df-117">openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="d28df-117">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="d28df-118">Чтение свойств и связей объекта **openShiftChangeRequest.**</span><span class="sxs-lookup"><span data-stu-id="d28df-118">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="d28df-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="d28df-119">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="d28df-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d28df-120">None</span></span>|<span data-ttu-id="d28df-121">Утверждение запроса на изменение открытой смены.</span><span class="sxs-lookup"><span data-stu-id="d28df-121">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="d28df-122">Отклонение</span><span class="sxs-lookup"><span data-stu-id="d28df-122">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="d28df-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d28df-123">None</span></span>| <span data-ttu-id="d28df-124">Отклонение запроса на изменение открытой смены.</span><span class="sxs-lookup"><span data-stu-id="d28df-124">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="d28df-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="d28df-125">Properties</span></span>

| <span data-ttu-id="d28df-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="d28df-126">Property</span></span>     | <span data-ttu-id="d28df-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d28df-127">Type</span></span>        | <span data-ttu-id="d28df-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d28df-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d28df-129">openShiftId</span><span class="sxs-lookup"><span data-stu-id="d28df-129">openShiftId</span></span>|<span data-ttu-id="d28df-130">String</span><span class="sxs-lookup"><span data-stu-id="d28df-130">String</span></span>| <span data-ttu-id="d28df-131">ИД для открытой смены.</span><span class="sxs-lookup"><span data-stu-id="d28df-131">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d28df-132">Связи</span><span class="sxs-lookup"><span data-stu-id="d28df-132">Relationships</span></span>

<span data-ttu-id="d28df-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d28df-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d28df-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d28df-134">JSON representation</span></span>

<span data-ttu-id="d28df-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d28df-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
}-->

```json
{
  "openShiftId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


