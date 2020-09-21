---
title: Тип ресурса educationRoot
description: 'Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a6f72f16d3a1e121883c4aa297aa0a4c93fe79d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989670"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="741ea-103">Тип ресурса educationRoot</span><span class="sxs-lookup"><span data-stu-id="741ea-103">educationRoot resource type</span></span>

<span data-ttu-id="741ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="741ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="741ea-105">Пространство имен `/education` обеспечивает функциональность, предназначенную для сектора образования.</span><span class="sxs-lookup"><span data-stu-id="741ea-105">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="741ea-106">Некоторые объекты пространства имен `/education` можно найти в других частях Microsoft Graph (например, [users](user.md)).</span><span class="sxs-lookup"><span data-stu-id="741ea-106">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="741ea-107">Пространство имен для образовательной сферы позволяет использовать специальные свойства и функции для этих объектов.</span><span class="sxs-lookup"><span data-stu-id="741ea-107">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="741ea-108">Методы</span><span class="sxs-lookup"><span data-stu-id="741ea-108">Methods</span></span>

| <span data-ttu-id="741ea-109">Метод</span><span class="sxs-lookup"><span data-stu-id="741ea-109">Method</span></span>           | <span data-ttu-id="741ea-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="741ea-110">Return Type</span></span>    |<span data-ttu-id="741ea-111">Описание</span><span class="sxs-lookup"><span data-stu-id="741ea-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="741ea-112">Создание educationClass</span><span class="sxs-lookup"><span data-stu-id="741ea-112">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="741ea-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="741ea-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="741ea-114">Создание объекта **educationClass** путем публикации в коллекции курсов.</span><span class="sxs-lookup"><span data-stu-id="741ea-114">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="741ea-115">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="741ea-115">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="741ea-116">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="741ea-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="741ea-117">Получение коллекции объектов **educationClass**.</span><span class="sxs-lookup"><span data-stu-id="741ea-117">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="741ea-118">Создание educationSchool</span><span class="sxs-lookup"><span data-stu-id="741ea-118">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="741ea-119">educationSchool</span><span class="sxs-lookup"><span data-stu-id="741ea-119">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="741ea-120">Создание объекта **educationSchool** путем публикации в коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="741ea-120">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="741ea-121">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="741ea-121">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="741ea-122">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="741ea-122">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="741ea-123">Получение коллекции объектов **educationSchool**.</span><span class="sxs-lookup"><span data-stu-id="741ea-123">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="741ea-124">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="741ea-124">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="741ea-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="741ea-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="741ea-126">Создание **educationUser** путем публикации в коллекции пользователей.</span><span class="sxs-lookup"><span data-stu-id="741ea-126">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="741ea-127">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="741ea-127">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="741ea-128">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="741ea-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="741ea-129">Получение коллекции объектов **educationUser**.</span><span class="sxs-lookup"><span data-stu-id="741ea-129">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="741ea-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="741ea-130">Properties</span></span>
<span data-ttu-id="741ea-131">Нет</span><span class="sxs-lookup"><span data-stu-id="741ea-131">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="741ea-132">Связи</span><span class="sxs-lookup"><span data-stu-id="741ea-132">Relationships</span></span>
| <span data-ttu-id="741ea-133">Связь</span><span class="sxs-lookup"><span data-stu-id="741ea-133">Relationship</span></span> | <span data-ttu-id="741ea-134">Тип</span><span class="sxs-lookup"><span data-stu-id="741ea-134">Type</span></span>   |<span data-ttu-id="741ea-135">Описание</span><span class="sxs-lookup"><span data-stu-id="741ea-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="741ea-136">classes</span><span class="sxs-lookup"><span data-stu-id="741ea-136">classes</span></span>|<span data-ttu-id="741ea-137">Коллекция [educationClass](educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="741ea-137">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="741ea-p102">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="741ea-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="741ea-140">me</span><span class="sxs-lookup"><span data-stu-id="741ea-140">me</span></span>|[<span data-ttu-id="741ea-141">educationUser</span><span class="sxs-lookup"><span data-stu-id="741ea-141">educationUser</span></span>](educationuser.md)| <span data-ttu-id="741ea-p103">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="741ea-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="741ea-144">schools</span><span class="sxs-lookup"><span data-stu-id="741ea-144">schools</span></span>|<span data-ttu-id="741ea-145">Коллекция [educationSchool](educationschool.md)</span><span class="sxs-lookup"><span data-stu-id="741ea-145">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="741ea-p104">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="741ea-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="741ea-148">users</span><span class="sxs-lookup"><span data-stu-id="741ea-148">users</span></span>|<span data-ttu-id="741ea-149">Коллекция [educationUser](educationuser.md)</span><span class="sxs-lookup"><span data-stu-id="741ea-149">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="741ea-p105">Только для чтения. Допускается значение NULL.</span><span class="sxs-lookup"><span data-stu-id="741ea-p105">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


