---
title: Тип ресурса userSource
description: Контейнер для почтового ящика хранителя и сайта OneDrive для бизнеса.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f0d98ac894d3d60bed2bb249ef9daec707f6f7ba
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447538"
---
# <a name="usersource-resource-type"></a><span data-ttu-id="a01a1-103">Тип ресурса userSource</span><span class="sxs-lookup"><span data-stu-id="a01a1-103">userSource resource type</span></span>

<span data-ttu-id="a01a1-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a01a1-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a01a1-105">Контейнер для [почтового ящика хранителя](ediscovery-custodian.md) и сайта OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a01a1-105">The container for a [custodian's](ediscovery-custodian.md) mailbox and OneDrive for Business site.</span></span>

## <a name="methods"></a><span data-ttu-id="a01a1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a01a1-106">Methods</span></span>

|<span data-ttu-id="a01a1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a01a1-107">Method</span></span>|<span data-ttu-id="a01a1-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="a01a1-108">Return type</span></span>|<span data-ttu-id="a01a1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a01a1-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a01a1-110">Список userSources</span><span class="sxs-lookup"><span data-stu-id="a01a1-110">List userSources</span></span>](../api/ediscovery-custodian-list-usersources.md)|<span data-ttu-id="a01a1-111">[коллекция microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="a01a1-111">[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) collection</span></span>|<span data-ttu-id="a01a1-112">Получите список объектов **userSource** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="a01a1-112">Get a list of the **userSource** objects and their properties.</span></span>|
|[<span data-ttu-id="a01a1-113">Создание userSource</span><span class="sxs-lookup"><span data-stu-id="a01a1-113">Create userSource</span></span>](../api/ediscovery-custodian-post-usersources.md)|[<span data-ttu-id="a01a1-114">microsoft.graph.ediscovery.userSource</span><span class="sxs-lookup"><span data-stu-id="a01a1-114">microsoft.graph.ediscovery.userSource</span></span>](../resources/ediscovery-usersource.md)|<span data-ttu-id="a01a1-115">Создание нового **объекта userSource.**</span><span class="sxs-lookup"><span data-stu-id="a01a1-115">Create a new **userSource** object.</span></span>|
|[<span data-ttu-id="a01a1-116">Get userSource</span><span class="sxs-lookup"><span data-stu-id="a01a1-116">Get userSource</span></span>](../api/ediscovery-usersource-get.md)|[<span data-ttu-id="a01a1-117">microsoft.graph.ediscovery.userSource</span><span class="sxs-lookup"><span data-stu-id="a01a1-117">microsoft.graph.ediscovery.userSource</span></span>](../resources/ediscovery-usersource.md)|<span data-ttu-id="a01a1-118">Ознакомьтесь с свойствами и отношениями **объекта userSource.**</span><span class="sxs-lookup"><span data-stu-id="a01a1-118">Read the properties and relationships of a **userSource** object.</span></span>|
|[<span data-ttu-id="a01a1-119">Удаление userSource</span><span class="sxs-lookup"><span data-stu-id="a01a1-119">Delete userSource</span></span>](../api/ediscovery-usersource-delete.md)|<span data-ttu-id="a01a1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a01a1-120">None</span></span>|<span data-ttu-id="a01a1-121">Удаление **объекта userSource.**</span><span class="sxs-lookup"><span data-stu-id="a01a1-121">Delete a **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a01a1-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="a01a1-122">Properties</span></span>

|<span data-ttu-id="a01a1-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="a01a1-123">Property</span></span>|<span data-ttu-id="a01a1-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a01a1-124">Type</span></span>|<span data-ttu-id="a01a1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a01a1-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a01a1-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="a01a1-126">createdBy</span></span>|[<span data-ttu-id="a01a1-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="a01a1-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="a01a1-128">Пользователь, создавший **userSource**.</span><span class="sxs-lookup"><span data-stu-id="a01a1-128">The user who created the **userSource**.</span></span>|
|<span data-ttu-id="a01a1-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a01a1-129">createdDateTime</span></span>|<span data-ttu-id="a01a1-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a01a1-130">DateTimeOffset</span></span>|<span data-ttu-id="a01a1-131">Дата и время создания **userSource**</span><span class="sxs-lookup"><span data-stu-id="a01a1-131">The date and time the **userSource** was created</span></span>|
|<span data-ttu-id="a01a1-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a01a1-132">displayName</span></span>|<span data-ttu-id="a01a1-133">String</span><span class="sxs-lookup"><span data-stu-id="a01a1-133">String</span></span>|<span data-ttu-id="a01a1-134">Имя отображения, связанное с почтовым ящиком и сайтом.</span><span class="sxs-lookup"><span data-stu-id="a01a1-134">The display name associated with the mailbox and site.</span></span>|
|<span data-ttu-id="a01a1-135">email</span><span class="sxs-lookup"><span data-stu-id="a01a1-135">email</span></span>|<span data-ttu-id="a01a1-136">String</span><span class="sxs-lookup"><span data-stu-id="a01a1-136">String</span></span>|<span data-ttu-id="a01a1-137">Адрес электронной почты почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="a01a1-137">Email address of the user's mailbox.</span></span>|
|<span data-ttu-id="a01a1-138">id</span><span class="sxs-lookup"><span data-stu-id="a01a1-138">id</span></span>|<span data-ttu-id="a01a1-139">String</span><span class="sxs-lookup"><span data-stu-id="a01a1-139">String</span></span>|<span data-ttu-id="a01a1-140">ID **пользователяSource**.</span><span class="sxs-lookup"><span data-stu-id="a01a1-140">The ID of the **userSource**.</span></span> <span data-ttu-id="a01a1-141">Это не ID фактической группы</span><span class="sxs-lookup"><span data-stu-id="a01a1-141">This is not the ID of the actual group</span></span>|
|<span data-ttu-id="a01a1-142">includedSources</span><span class="sxs-lookup"><span data-stu-id="a01a1-142">includedSources</span></span>|<span data-ttu-id="a01a1-143">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="a01a1-143">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="a01a1-144">Указывает, какие источники включены в эту группу.</span><span class="sxs-lookup"><span data-stu-id="a01a1-144">Specifies which sources are included in this group.</span></span> <span data-ttu-id="a01a1-145">Возможные значения: `mailbox`, `site`.</span><span class="sxs-lookup"><span data-stu-id="a01a1-145">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="a01a1-146">значения sourceType</span><span class="sxs-lookup"><span data-stu-id="a01a1-146">sourceType values</span></span>

<span data-ttu-id="a01a1-147">Типы источников, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="a01a1-147">Types of source related to the user.</span></span> <span data-ttu-id="a01a1-148">Включает почтовый ящик и сайт по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a01a1-148">Includes mailbox and site by default.</span></span>

|<span data-ttu-id="a01a1-149">Member</span><span class="sxs-lookup"><span data-stu-id="a01a1-149">Member</span></span>|<span data-ttu-id="a01a1-150">Описание</span><span class="sxs-lookup"><span data-stu-id="a01a1-150">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="a01a1-151">mailbox</span><span class="sxs-lookup"><span data-stu-id="a01a1-151">mailbox</span></span>|<span data-ttu-id="a01a1-152">Представляет почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="a01a1-152">Represents a mailbox.</span></span>|
|<span data-ttu-id="a01a1-153">site</span><span class="sxs-lookup"><span data-stu-id="a01a1-153">site</span></span>|<span data-ttu-id="a01a1-154">Представляет сайт OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="a01a1-154">Represents a OneDrive for Business site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a01a1-155">Связи</span><span class="sxs-lookup"><span data-stu-id="a01a1-155">Relationships</span></span>

<span data-ttu-id="a01a1-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a01a1-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a01a1-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a01a1-157">JSON representation</span></span>

<span data-ttu-id="a01a1-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a01a1-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.userSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.userSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "email": "String",
  "includedSources": "String"
}
```
