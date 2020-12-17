---
title: Тип ресурса userSource
description: Контейнер для почтового ящика хранителя и сайта OneDrive для бизнеса.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 10184e053a0c62aaba6599f7d6f9bb6a33de8828
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706042"
---
# <a name="usersource-resource-type"></a><span data-ttu-id="7b9c4-103">Тип ресурса userSource</span><span class="sxs-lookup"><span data-stu-id="7b9c4-103">userSource resource type</span></span>

<span data-ttu-id="7b9c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b9c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b9c4-105">Контейнер для почтового [ящика хранителя](custodian.md) и сайта OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7b9c4-105">The container for a [custodian's](custodian.md) mailbox and OneDrive for Business site.</span></span>

## <a name="methods"></a><span data-ttu-id="7b9c4-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7b9c4-106">Methods</span></span>

|<span data-ttu-id="7b9c4-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7b9c4-107">Method</span></span>|<span data-ttu-id="7b9c4-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="7b9c4-108">Return type</span></span>|<span data-ttu-id="7b9c4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7b9c4-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7b9c4-110">Список userSources</span><span class="sxs-lookup"><span data-stu-id="7b9c4-110">List userSources</span></span>](../api/custodian-list-usersources.md)|<span data-ttu-id="7b9c4-111">[Коллекция userSource](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="7b9c4-111">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="7b9c4-112">Получите список объектов **userSource** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="7b9c4-112">Get a list of the **userSource** objects and their properties.</span></span>|
|[<span data-ttu-id="7b9c4-113">Создание userSource</span><span class="sxs-lookup"><span data-stu-id="7b9c4-113">Create userSource</span></span>](../api/custodian-post-usersources.md)|[<span data-ttu-id="7b9c4-114">userSource</span><span class="sxs-lookup"><span data-stu-id="7b9c4-114">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="7b9c4-115">Создание объекта **userSource.**</span><span class="sxs-lookup"><span data-stu-id="7b9c4-115">Create a new **userSource** object.</span></span>|
|[<span data-ttu-id="7b9c4-116">Get userSource</span><span class="sxs-lookup"><span data-stu-id="7b9c4-116">Get userSource</span></span>](../api/usersource-get.md)|[<span data-ttu-id="7b9c4-117">userSource</span><span class="sxs-lookup"><span data-stu-id="7b9c4-117">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="7b9c4-118">Чтение свойств и связей объекта **userSource.**</span><span class="sxs-lookup"><span data-stu-id="7b9c4-118">Read the properties and relationships of a **userSource** object.</span></span>|
|[<span data-ttu-id="7b9c4-119">Удаление userSource</span><span class="sxs-lookup"><span data-stu-id="7b9c4-119">Delete userSource</span></span>](../api/usersource-delete.md)|<span data-ttu-id="7b9c4-120">Нет</span><span class="sxs-lookup"><span data-stu-id="7b9c4-120">None</span></span>|<span data-ttu-id="7b9c4-121">Удаление объекта **userSource.**</span><span class="sxs-lookup"><span data-stu-id="7b9c4-121">Delete a **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b9c4-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b9c4-122">Properties</span></span>

|<span data-ttu-id="7b9c4-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b9c4-123">Property</span></span>|<span data-ttu-id="7b9c4-124">Тип</span><span class="sxs-lookup"><span data-stu-id="7b9c4-124">Type</span></span>|<span data-ttu-id="7b9c4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7b9c4-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b9c4-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="7b9c4-126">createdBy</span></span>|[<span data-ttu-id="7b9c4-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="7b9c4-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="7b9c4-128">Пользователь, создавший **userSource.**</span><span class="sxs-lookup"><span data-stu-id="7b9c4-128">The user who created the **userSource**.</span></span>|
|<span data-ttu-id="7b9c4-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b9c4-129">createdDateTime</span></span>|<span data-ttu-id="7b9c4-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b9c4-130">DateTimeOffset</span></span>|<span data-ttu-id="7b9c4-131">Дата и время создания **userSource**</span><span class="sxs-lookup"><span data-stu-id="7b9c4-131">The date and time the **userSource** was created</span></span>|
|<span data-ttu-id="7b9c4-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7b9c4-132">displayName</span></span>|<span data-ttu-id="7b9c4-133">String</span><span class="sxs-lookup"><span data-stu-id="7b9c4-133">String</span></span>|<span data-ttu-id="7b9c4-134">Отображаемая фамилия, связанная с почтовым ящиком и сайтом.</span><span class="sxs-lookup"><span data-stu-id="7b9c4-134">The display name associated with the mailbox and site.</span></span>|
|<span data-ttu-id="7b9c4-135">email</span><span class="sxs-lookup"><span data-stu-id="7b9c4-135">email</span></span>|<span data-ttu-id="7b9c4-136">String</span><span class="sxs-lookup"><span data-stu-id="7b9c4-136">String</span></span>|<span data-ttu-id="7b9c4-137">Адрес электронной почты почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="7b9c4-137">Email address of the user's mailbox.</span></span>|
|<span data-ttu-id="7b9c4-138">id</span><span class="sxs-lookup"><span data-stu-id="7b9c4-138">id</span></span>|<span data-ttu-id="7b9c4-139">String</span><span class="sxs-lookup"><span data-stu-id="7b9c4-139">String</span></span>|<span data-ttu-id="7b9c4-140">ИД **userSource.**</span><span class="sxs-lookup"><span data-stu-id="7b9c4-140">The ID of the **userSource**.</span></span> <span data-ttu-id="7b9c4-141">Это не ИД фактической группы</span><span class="sxs-lookup"><span data-stu-id="7b9c4-141">This is not the ID of the actual group</span></span>|
|<span data-ttu-id="7b9c4-142">includedSources</span><span class="sxs-lookup"><span data-stu-id="7b9c4-142">includedSources</span></span>|<span data-ttu-id="7b9c4-143">sourceType</span><span class="sxs-lookup"><span data-stu-id="7b9c4-143">sourceType</span></span>|<span data-ttu-id="7b9c4-144">Указывает источники, включенные в эту группу.</span><span class="sxs-lookup"><span data-stu-id="7b9c4-144">Specifies which sources are included in this group.</span></span> <span data-ttu-id="7b9c4-145">Возможные значения: `mailbox`, `site`.</span><span class="sxs-lookup"><span data-stu-id="7b9c4-145">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="7b9c4-146">значения sourceType</span><span class="sxs-lookup"><span data-stu-id="7b9c4-146">sourceType values</span></span>

<span data-ttu-id="7b9c4-147">Типы источников, связанных с пользователем.</span><span class="sxs-lookup"><span data-stu-id="7b9c4-147">Types of source related to the user.</span></span> <span data-ttu-id="7b9c4-148">Включает почтовый ящик и сайт по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7b9c4-148">Includes mailbox and site by default.</span></span>

|<span data-ttu-id="7b9c4-149">Member</span><span class="sxs-lookup"><span data-stu-id="7b9c4-149">Member</span></span>|<span data-ttu-id="7b9c4-150">Описание</span><span class="sxs-lookup"><span data-stu-id="7b9c4-150">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="7b9c4-151">mailbox</span><span class="sxs-lookup"><span data-stu-id="7b9c4-151">mailbox</span></span>|<span data-ttu-id="7b9c4-152">Представляет почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="7b9c4-152">Represents a mailbox.</span></span>|
|<span data-ttu-id="7b9c4-153">site</span><span class="sxs-lookup"><span data-stu-id="7b9c4-153">site</span></span>|<span data-ttu-id="7b9c4-154">Представляет сайт OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="7b9c4-154">Represents a OneDrive for Business site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b9c4-155">Связи</span><span class="sxs-lookup"><span data-stu-id="7b9c4-155">Relationships</span></span>

<span data-ttu-id="7b9c4-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7b9c4-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b9c4-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7b9c4-157">JSON representation</span></span>

<span data-ttu-id="7b9c4-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b9c4-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userSource",
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
