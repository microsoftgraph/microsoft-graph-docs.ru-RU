---
title: Тип ресурса Унифиедграупсаурце
description: Контейнер для группы хранитель.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 5fba2a994cda61f111739d98ea3a210c76ffeb23
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597813"
---
# <a name="unifiedgroupsource-resource-type"></a><span data-ttu-id="e4b81-103">Тип ресурса Унифиедграупсаурце</span><span class="sxs-lookup"><span data-stu-id="e4b81-103">unifiedGroupSource resource type</span></span>

<span data-ttu-id="e4b81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4b81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4b81-105">Контейнер для группы [хранитель](custodian.md) .</span><span class="sxs-lookup"><span data-stu-id="e4b81-105">The container for a [custodian's](custodian.md) group.</span></span>

## <a name="methods"></a><span data-ttu-id="e4b81-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e4b81-106">Methods</span></span>

|<span data-ttu-id="e4b81-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e4b81-107">Method</span></span>|<span data-ttu-id="e4b81-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="e4b81-108">Return type</span></span>|<span data-ttu-id="e4b81-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e4b81-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e4b81-110">Список Унифиедграупсаурцес</span><span class="sxs-lookup"><span data-stu-id="e4b81-110">List unifiedGroupSources</span></span>](../api/custodian-list-unifiedgroupsources.md)|<span data-ttu-id="e4b81-111">Коллекция [унифиедграупсаурце](../resources/unifiedgroupsource.md)</span><span class="sxs-lookup"><span data-stu-id="e4b81-111">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="e4b81-112">Получение списка объектов **унифиедграупсаурце** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="e4b81-112">Get a list of the **unifiedGroupSource** objects and their properties.</span></span>|
|[<span data-ttu-id="e4b81-113">Создание Унифиедграупсаурце</span><span class="sxs-lookup"><span data-stu-id="e4b81-113">Create unifiedGroupSource</span></span>](../api/custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="e4b81-114">унифиедграупсаурце</span><span class="sxs-lookup"><span data-stu-id="e4b81-114">unifiedGroupSource</span></span>](../resources/unifiedgroupsource.md)|<span data-ttu-id="e4b81-115">Создание нового объекта **унифиедграупсаурце** .</span><span class="sxs-lookup"><span data-stu-id="e4b81-115">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="e4b81-116">Получение Унифиедграупсаурце</span><span class="sxs-lookup"><span data-stu-id="e4b81-116">Get unifiedGroupSource</span></span>](../api/unifiedgroupsource-get.md)|[<span data-ttu-id="e4b81-117">унифиедграупсаурце</span><span class="sxs-lookup"><span data-stu-id="e4b81-117">unifiedGroupSource</span></span>](../resources/unifiedgroupsource.md)|<span data-ttu-id="e4b81-118">Чтение свойств и связей объекта **унифиедграупсаурце** .</span><span class="sxs-lookup"><span data-stu-id="e4b81-118">Read the properties and relationships of a **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="e4b81-119">Удаление Унифиедграупсаурце</span><span class="sxs-lookup"><span data-stu-id="e4b81-119">Delete unifiedGroupSource</span></span>](../api/unifiedgroupsource-delete.md)|<span data-ttu-id="e4b81-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e4b81-120">None</span></span>|<span data-ttu-id="e4b81-121">Удаление объекта **унифиедграупсаурце** .</span><span class="sxs-lookup"><span data-stu-id="e4b81-121">Delete a **unifiedGroupSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e4b81-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4b81-122">Properties</span></span>

|<span data-ttu-id="e4b81-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4b81-123">Property</span></span>|<span data-ttu-id="e4b81-124">Тип</span><span class="sxs-lookup"><span data-stu-id="e4b81-124">Type</span></span>|<span data-ttu-id="e4b81-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e4b81-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4b81-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="e4b81-126">createdBy</span></span>|[<span data-ttu-id="e4b81-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="e4b81-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="e4b81-128">Пользователь, создавший **унифиедграупсаурце**.</span><span class="sxs-lookup"><span data-stu-id="e4b81-128">The user who created the **unifiedGroupSource**.</span></span>|
|<span data-ttu-id="e4b81-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4b81-129">createdDateTime</span></span>|<span data-ttu-id="e4b81-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4b81-130">DateTimeOffset</span></span>|<span data-ttu-id="e4b81-131">Дата и время создания **унифиедграупсаурце** .</span><span class="sxs-lookup"><span data-stu-id="e4b81-131">The date and time the **unifiedGroupSource** was created.</span></span>|
|<span data-ttu-id="e4b81-132">displayName</span><span class="sxs-lookup"><span data-stu-id="e4b81-132">displayName</span></span>|<span data-ttu-id="e4b81-133">String</span><span class="sxs-lookup"><span data-stu-id="e4b81-133">String</span></span>|<span data-ttu-id="e4b81-134">Отображаемое имя единой группы — это имя группы.</span><span class="sxs-lookup"><span data-stu-id="e4b81-134">The display name of the unified group - This is the name of the group.</span></span>|
|<span data-ttu-id="e4b81-135">id</span><span class="sxs-lookup"><span data-stu-id="e4b81-135">id</span></span>|<span data-ttu-id="e4b81-136">String</span><span class="sxs-lookup"><span data-stu-id="e4b81-136">String</span></span>|<span data-ttu-id="e4b81-137">Идентификатор **унифиедграупсаурце**.</span><span class="sxs-lookup"><span data-stu-id="e4b81-137">The ID of the **unifiedGroupSource**.</span></span> <span data-ttu-id="e4b81-138">Это значение не является ИДЕНТИФИКАТОРом фактической группы.</span><span class="sxs-lookup"><span data-stu-id="e4b81-138">This is not the ID of the actual group.</span></span>|
|<span data-ttu-id="e4b81-139">инклудедсаурцес</span><span class="sxs-lookup"><span data-stu-id="e4b81-139">includedSources</span></span>|<span data-ttu-id="e4b81-140">sourceType</span><span class="sxs-lookup"><span data-stu-id="e4b81-140">sourceType</span></span>|<span data-ttu-id="e4b81-141">Указывает, какие источники включены в эту группу.</span><span class="sxs-lookup"><span data-stu-id="e4b81-141">Specifies which sources are included in this group.</span></span> <span data-ttu-id="e4b81-142">Возможные значения: `mailbox`, `site`.</span><span class="sxs-lookup"><span data-stu-id="e4b81-142">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="e4b81-143">значения sourceType</span><span class="sxs-lookup"><span data-stu-id="e4b81-143">sourceType values</span></span>

<span data-ttu-id="e4b81-144">Типы источника, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="e4b81-144">Types of source related to the user.</span></span> <span data-ttu-id="e4b81-145">По умолчанию включается почтовый ящик и сайт.</span><span class="sxs-lookup"><span data-stu-id="e4b81-145">Includes mailbox and site both by default.</span></span>

|<span data-ttu-id="e4b81-146">Member</span><span class="sxs-lookup"><span data-stu-id="e4b81-146">Member</span></span>|<span data-ttu-id="e4b81-147">Описание</span><span class="sxs-lookup"><span data-stu-id="e4b81-147">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="e4b81-148">mailbox</span><span class="sxs-lookup"><span data-stu-id="e4b81-148">mailbox</span></span>|<span data-ttu-id="e4b81-149">Представляет почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="e4b81-149">Represents a mailbox.</span></span>|
|<span data-ttu-id="e4b81-150">site</span><span class="sxs-lookup"><span data-stu-id="e4b81-150">site</span></span>|<span data-ttu-id="e4b81-151">Представляет сайт SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e4b81-151">Represents a SharePoint site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4b81-152">Связи</span><span class="sxs-lookup"><span data-stu-id="e4b81-152">Relationships</span></span>

|<span data-ttu-id="e4b81-153">Связь</span><span class="sxs-lookup"><span data-stu-id="e4b81-153">Relationship</span></span>|<span data-ttu-id="e4b81-154">Тип</span><span class="sxs-lookup"><span data-stu-id="e4b81-154">Type</span></span>|<span data-ttu-id="e4b81-155">Описание</span><span class="sxs-lookup"><span data-stu-id="e4b81-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4b81-156">group</span><span class="sxs-lookup"><span data-stu-id="e4b81-156">group</span></span>|[<span data-ttu-id="e4b81-157">group</span><span class="sxs-lookup"><span data-stu-id="e4b81-157">group</span></span>](../resources/group.md)|<span data-ttu-id="e4b81-158">Группа, связанная с **унифиедграупсаурце**.</span><span class="sxs-lookup"><span data-stu-id="e4b81-158">The group associated with the **unifiedGroupSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4b81-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4b81-159">JSON representation</span></span>

<span data-ttu-id="e4b81-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4b81-160">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedGroupSource",
  "baseType": "microsoft.graph.dataSource",
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
