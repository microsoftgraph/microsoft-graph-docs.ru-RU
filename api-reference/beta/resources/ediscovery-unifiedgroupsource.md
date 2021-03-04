---
title: тип ресурсов unifiedGroupSource
description: Контейнер для группы хранителя.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b6d1b1d1a7d3abee2516e170fcead20c73235f1f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447543"
---
# <a name="unifiedgroupsource-resource-type"></a><span data-ttu-id="628c0-103">тип ресурсов unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="628c0-103">unifiedGroupSource resource type</span></span>

<span data-ttu-id="628c0-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="628c0-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="628c0-105">Контейнер для [группы](ediscovery-custodian.md) хранителя.</span><span class="sxs-lookup"><span data-stu-id="628c0-105">The container for a [custodian's](ediscovery-custodian.md) group.</span></span>

## <a name="methods"></a><span data-ttu-id="628c0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="628c0-106">Methods</span></span>

|<span data-ttu-id="628c0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="628c0-107">Method</span></span>|<span data-ttu-id="628c0-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="628c0-108">Return type</span></span>|<span data-ttu-id="628c0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="628c0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="628c0-110">Список унифицированныхGroupSources</span><span class="sxs-lookup"><span data-stu-id="628c0-110">List unifiedGroupSources</span></span>](../api/ediscovery-custodian-list-unifiedgroupsources.md)|<span data-ttu-id="628c0-111">[коллекция microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="628c0-111">[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="628c0-112">Получите список объектов **unifiedGroupSource** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="628c0-112">Get a list of the **unifiedGroupSource** objects and their properties.</span></span>|
|[<span data-ttu-id="628c0-113">Создание unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="628c0-113">Create unifiedGroupSource</span></span>](../api/ediscovery-custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="628c0-114">microsoft.graph.ediscovery.unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="628c0-114">microsoft.graph.ediscovery.unifiedGroupSource</span></span>](../resources/ediscovery-unifiedgroupsource.md)|<span data-ttu-id="628c0-115">Создание нового **объекта unifiedGroupSource.**</span><span class="sxs-lookup"><span data-stu-id="628c0-115">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="628c0-116">Get unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="628c0-116">Get unifiedGroupSource</span></span>](../api/ediscovery-unifiedgroupsource-get.md)|[<span data-ttu-id="628c0-117">microsoft.graph.ediscovery.unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="628c0-117">microsoft.graph.ediscovery.unifiedGroupSource</span></span>](../resources/ediscovery-unifiedgroupsource.md)|<span data-ttu-id="628c0-118">Ознакомьтесь с свойствами и отношениями объекта **unifiedGroupSource.**</span><span class="sxs-lookup"><span data-stu-id="628c0-118">Read the properties and relationships of a **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="628c0-119">Удаление unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="628c0-119">Delete unifiedGroupSource</span></span>](../api/ediscovery-unifiedgroupsource-delete.md)|<span data-ttu-id="628c0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="628c0-120">None</span></span>|<span data-ttu-id="628c0-121">Удаление **объекта unifiedGroupSource.**</span><span class="sxs-lookup"><span data-stu-id="628c0-121">Delete a **unifiedGroupSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="628c0-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="628c0-122">Properties</span></span>

|<span data-ttu-id="628c0-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="628c0-123">Property</span></span>|<span data-ttu-id="628c0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="628c0-124">Type</span></span>|<span data-ttu-id="628c0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="628c0-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="628c0-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="628c0-126">createdBy</span></span>|[<span data-ttu-id="628c0-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="628c0-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="628c0-128">Пользователь, создавший **унифицированнуюGroupSource.**</span><span class="sxs-lookup"><span data-stu-id="628c0-128">The user who created the **unifiedGroupSource**.</span></span>|
|<span data-ttu-id="628c0-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="628c0-129">createdDateTime</span></span>|<span data-ttu-id="628c0-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="628c0-130">DateTimeOffset</span></span>|<span data-ttu-id="628c0-131">Дата и время создания **unifiedGroupSource.**</span><span class="sxs-lookup"><span data-stu-id="628c0-131">The date and time the **unifiedGroupSource** was created.</span></span>|
|<span data-ttu-id="628c0-132">displayName</span><span class="sxs-lookup"><span data-stu-id="628c0-132">displayName</span></span>|<span data-ttu-id="628c0-133">String</span><span class="sxs-lookup"><span data-stu-id="628c0-133">String</span></span>|<span data-ttu-id="628c0-134">Отображаемое имя единой группы — это имя группы.</span><span class="sxs-lookup"><span data-stu-id="628c0-134">The display name of the unified group - This is the name of the group.</span></span>|
|<span data-ttu-id="628c0-135">id</span><span class="sxs-lookup"><span data-stu-id="628c0-135">id</span></span>|<span data-ttu-id="628c0-136">String</span><span class="sxs-lookup"><span data-stu-id="628c0-136">String</span></span>|<span data-ttu-id="628c0-137">ID **единойGroupSource**.</span><span class="sxs-lookup"><span data-stu-id="628c0-137">The ID of the **unifiedGroupSource**.</span></span> <span data-ttu-id="628c0-138">Это не ID фактической группы.</span><span class="sxs-lookup"><span data-stu-id="628c0-138">This is not the ID of the actual group.</span></span>|
|<span data-ttu-id="628c0-139">includedSources</span><span class="sxs-lookup"><span data-stu-id="628c0-139">includedSources</span></span>|<span data-ttu-id="628c0-140">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="628c0-140">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="628c0-141">Указывает, какие источники включены в эту группу.</span><span class="sxs-lookup"><span data-stu-id="628c0-141">Specifies which sources are included in this group.</span></span> <span data-ttu-id="628c0-142">Возможные значения: `mailbox`, `site`.</span><span class="sxs-lookup"><span data-stu-id="628c0-142">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="628c0-143">значения sourceType</span><span class="sxs-lookup"><span data-stu-id="628c0-143">sourceType values</span></span>

<span data-ttu-id="628c0-144">Типы источников, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="628c0-144">Types of source related to the user.</span></span> <span data-ttu-id="628c0-145">Включает почтовый ящик и сайт по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="628c0-145">Includes mailbox and site both by default.</span></span>

|<span data-ttu-id="628c0-146">Member</span><span class="sxs-lookup"><span data-stu-id="628c0-146">Member</span></span>|<span data-ttu-id="628c0-147">Описание</span><span class="sxs-lookup"><span data-stu-id="628c0-147">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="628c0-148">mailbox</span><span class="sxs-lookup"><span data-stu-id="628c0-148">mailbox</span></span>|<span data-ttu-id="628c0-149">Представляет почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="628c0-149">Represents a mailbox.</span></span>|
|<span data-ttu-id="628c0-150">site</span><span class="sxs-lookup"><span data-stu-id="628c0-150">site</span></span>|<span data-ttu-id="628c0-151">Представляет сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="628c0-151">Represents a SharePoint site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="628c0-152">Связи</span><span class="sxs-lookup"><span data-stu-id="628c0-152">Relationships</span></span>

|<span data-ttu-id="628c0-153">Связь</span><span class="sxs-lookup"><span data-stu-id="628c0-153">Relationship</span></span>|<span data-ttu-id="628c0-154">Тип</span><span class="sxs-lookup"><span data-stu-id="628c0-154">Type</span></span>|<span data-ttu-id="628c0-155">Описание</span><span class="sxs-lookup"><span data-stu-id="628c0-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="628c0-156">group</span><span class="sxs-lookup"><span data-stu-id="628c0-156">group</span></span>|[<span data-ttu-id="628c0-157">group</span><span class="sxs-lookup"><span data-stu-id="628c0-157">group</span></span>](../resources/group.md)|<span data-ttu-id="628c0-158">Группа, связанная с **унифицированнойGroupSource**.</span><span class="sxs-lookup"><span data-stu-id="628c0-158">The group associated with the **unifiedGroupSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="628c0-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="628c0-159">JSON representation</span></span>

<span data-ttu-id="628c0-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="628c0-160">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.unifiedGroupSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "value": [
        {
            "displayName": "Developers group",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "33434233-3030-3739-3043-393039324633",
            "includedSources": "mailbox,site",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
