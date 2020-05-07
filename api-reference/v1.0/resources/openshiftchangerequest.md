---
title: Тип ресурса Опеншифтчанжерекуест
description: Представляет запрос на утверждение открытых смен в расписании.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 47a2aa9eddc4e45d88c3768ded2b44e9d5952178
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154986"
---
# <a name="openshiftchangerequest-resource-type"></a><span data-ttu-id="406a9-103">Тип ресурса Опеншифтчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="406a9-103">openShiftChangeRequest resource type</span></span>

<span data-ttu-id="406a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="406a9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="406a9-105">Представляет запрос на утверждение [опеншифт](../resources/openshift.md) по [расписанию](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="406a9-105">Represents request to claim an [openShift](../resources/openshift.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="406a9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="406a9-106">Methods</span></span>

| <span data-ttu-id="406a9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="406a9-107">Method</span></span>       | <span data-ttu-id="406a9-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="406a9-108">Return Type</span></span> | <span data-ttu-id="406a9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="406a9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="406a9-110">List</span><span class="sxs-lookup"><span data-stu-id="406a9-110">List</span></span>](../api/openshiftchangerequest-list.md) | <span data-ttu-id="406a9-111">Коллекция [опеншифтчанжерекуест](openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="406a9-111">Collection of [openShiftChangeRequest](openshiftchangerequest.md)</span></span> | <span data-ttu-id="406a9-112">Перечисление свойств и связей объектов **опеншифтчанжерекуест** в команде.</span><span class="sxs-lookup"><span data-stu-id="406a9-112">List the properties and relationships of **openShiftChangeRequest** objects in a team.</span></span> |
| <span data-ttu-id="406a9-113">[создание](../api/openshiftchangerequest-post.md);</span><span class="sxs-lookup"><span data-stu-id="406a9-113">[Create](../api/openshiftchangerequest-post.md)</span></span> | [<span data-ttu-id="406a9-114">опеншифтчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="406a9-114">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="406a9-115">Создайте экземпляр объекта **опеншифтчанжерекуест** .</span><span class="sxs-lookup"><span data-stu-id="406a9-115">Create an instance of an **openShiftChangeRequest** object.</span></span> |
| <span data-ttu-id="406a9-116">[получение](../api/openshiftchangerequest-get.md);</span><span class="sxs-lookup"><span data-stu-id="406a9-116">[Get](../api/openshiftchangerequest-get.md)</span></span> | [<span data-ttu-id="406a9-117">опеншифтчанжерекуест</span><span class="sxs-lookup"><span data-stu-id="406a9-117">openShiftChangeRequest</span></span>](openshiftchangerequest.md) | <span data-ttu-id="406a9-118">Чтение свойств и связей объекта **опеншифтчанжерекуест** .</span><span class="sxs-lookup"><span data-stu-id="406a9-118">Read the properties and relationships of an **openShiftChangeRequest** object.</span></span> |
|[<span data-ttu-id="406a9-119">Утвердить</span><span class="sxs-lookup"><span data-stu-id="406a9-119">Approve</span></span>](../api/openshiftchangerequest-approve.md)|<span data-ttu-id="406a9-120">Нет</span><span class="sxs-lookup"><span data-stu-id="406a9-120">None</span></span>|<span data-ttu-id="406a9-121">Утверждение запроса на изменение открытого сочетания клавиш.</span><span class="sxs-lookup"><span data-stu-id="406a9-121">Approve an open shift change request.</span></span>|
|[<span data-ttu-id="406a9-122">Отклоня</span><span class="sxs-lookup"><span data-stu-id="406a9-122">Decline</span></span>](../api/openshiftchangerequest-decline.md)|<span data-ttu-id="406a9-123">Нет</span><span class="sxs-lookup"><span data-stu-id="406a9-123">None</span></span>| <span data-ttu-id="406a9-124">Отклонить запрос на изменение открытого Shift.</span><span class="sxs-lookup"><span data-stu-id="406a9-124">Decline an open shift change request.</span></span>|

## <a name="properties"></a><span data-ttu-id="406a9-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="406a9-125">Properties</span></span>

| <span data-ttu-id="406a9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="406a9-126">Property</span></span>     | <span data-ttu-id="406a9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="406a9-127">Type</span></span>        | <span data-ttu-id="406a9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="406a9-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="406a9-129">опеншифтид</span><span class="sxs-lookup"><span data-stu-id="406a9-129">openShiftId</span></span>|<span data-ttu-id="406a9-130">Строка</span><span class="sxs-lookup"><span data-stu-id="406a9-130">String</span></span>| <span data-ttu-id="406a9-131">Идентификатор для открытой смены.</span><span class="sxs-lookup"><span data-stu-id="406a9-131">ID for the open shift.</span></span>|

## <a name="relationships"></a><span data-ttu-id="406a9-132">Связи</span><span class="sxs-lookup"><span data-stu-id="406a9-132">Relationships</span></span>

<span data-ttu-id="406a9-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="406a9-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="406a9-134">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="406a9-134">JSON representation</span></span>

<span data-ttu-id="406a9-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="406a9-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openShiftChangeRequest",
  "baseType": ""
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
