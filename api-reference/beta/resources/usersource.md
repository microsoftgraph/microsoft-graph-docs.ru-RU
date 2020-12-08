---
title: Тип ресурса Усерсаурце
description: Контейнер для почтового ящика хранитель и сайта OneDrive для бизнеса.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 2ce5448947bded580cc4896ba549d7cc6fab95f9
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597742"
---
# <a name="usersource-resource-type"></a><span data-ttu-id="1894b-103">Тип ресурса Усерсаурце</span><span class="sxs-lookup"><span data-stu-id="1894b-103">userSource resource type</span></span>

<span data-ttu-id="1894b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1894b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1894b-105">Контейнер для почтового ящика [хранитель](custodian.md) и сайта OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1894b-105">The container for a [custodian's](custodian.md) mailbox and OneDrive for Business site.</span></span>

## <a name="methods"></a><span data-ttu-id="1894b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1894b-106">Methods</span></span>

|<span data-ttu-id="1894b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1894b-107">Method</span></span>|<span data-ttu-id="1894b-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="1894b-108">Return type</span></span>|<span data-ttu-id="1894b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1894b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1894b-110">Список Усерсаурцес</span><span class="sxs-lookup"><span data-stu-id="1894b-110">List userSources</span></span>](../api/custodian-list-usersources.md)|<span data-ttu-id="1894b-111">Коллекция [усерсаурце](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="1894b-111">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="1894b-112">Получение списка объектов **усерсаурце** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="1894b-112">Get a list of the **userSource** objects and their properties.</span></span>|
|[<span data-ttu-id="1894b-113">Создание Усерсаурце</span><span class="sxs-lookup"><span data-stu-id="1894b-113">Create userSource</span></span>](../api/custodian-post-usersources.md)|[<span data-ttu-id="1894b-114">усерсаурце</span><span class="sxs-lookup"><span data-stu-id="1894b-114">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="1894b-115">Создание нового объекта **усерсаурце** .</span><span class="sxs-lookup"><span data-stu-id="1894b-115">Create a new **userSource** object.</span></span>|
|[<span data-ttu-id="1894b-116">Получение Усерсаурце</span><span class="sxs-lookup"><span data-stu-id="1894b-116">Get userSource</span></span>](../api/usersource-get.md)|[<span data-ttu-id="1894b-117">усерсаурце</span><span class="sxs-lookup"><span data-stu-id="1894b-117">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="1894b-118">Чтение свойств и связей объекта **усерсаурце** .</span><span class="sxs-lookup"><span data-stu-id="1894b-118">Read the properties and relationships of a **userSource** object.</span></span>|
|[<span data-ttu-id="1894b-119">Удаление Усерсаурце</span><span class="sxs-lookup"><span data-stu-id="1894b-119">Delete userSource</span></span>](../api/usersource-delete.md)|<span data-ttu-id="1894b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="1894b-120">None</span></span>|<span data-ttu-id="1894b-121">Удаление объекта **усерсаурце** .</span><span class="sxs-lookup"><span data-stu-id="1894b-121">Delete a **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1894b-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="1894b-122">Properties</span></span>

|<span data-ttu-id="1894b-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="1894b-123">Property</span></span>|<span data-ttu-id="1894b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="1894b-124">Type</span></span>|<span data-ttu-id="1894b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1894b-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1894b-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="1894b-126">createdBy</span></span>|[<span data-ttu-id="1894b-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="1894b-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="1894b-128">Пользователь, создавший **усерсаурце**.</span><span class="sxs-lookup"><span data-stu-id="1894b-128">The user who created the **userSource**.</span></span>|
|<span data-ttu-id="1894b-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1894b-129">createdDateTime</span></span>|<span data-ttu-id="1894b-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1894b-130">DateTimeOffset</span></span>|<span data-ttu-id="1894b-131">Дата и время создания ерсаурце **усерсаурце** для США</span><span class="sxs-lookup"><span data-stu-id="1894b-131">The date and time the us **userSource** erSource was created</span></span>|
|<span data-ttu-id="1894b-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1894b-132">displayName</span></span>|<span data-ttu-id="1894b-133">String</span><span class="sxs-lookup"><span data-stu-id="1894b-133">String</span></span>|<span data-ttu-id="1894b-134">Отображаемое имя, связанное с почтовым ящиком и сайтом.</span><span class="sxs-lookup"><span data-stu-id="1894b-134">The display name associated with the mailbox and site.</span></span>|
|<span data-ttu-id="1894b-135">email</span><span class="sxs-lookup"><span data-stu-id="1894b-135">email</span></span>|<span data-ttu-id="1894b-136">String</span><span class="sxs-lookup"><span data-stu-id="1894b-136">String</span></span>|<span data-ttu-id="1894b-137">Адрес электронной почты почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="1894b-137">Email address of the user's mailbox.</span></span>|
|<span data-ttu-id="1894b-138">id</span><span class="sxs-lookup"><span data-stu-id="1894b-138">id</span></span>|<span data-ttu-id="1894b-139">String</span><span class="sxs-lookup"><span data-stu-id="1894b-139">String</span></span>|<span data-ttu-id="1894b-140">Идентификатор **усерсаурце**.</span><span class="sxs-lookup"><span data-stu-id="1894b-140">The ID of the **userSource**.</span></span> <span data-ttu-id="1894b-141">Это значение не является ИДЕНТИФИКАТОРом фактической группы</span><span class="sxs-lookup"><span data-stu-id="1894b-141">This is not the ID of the actual group</span></span>|
|<span data-ttu-id="1894b-142">инклудедсаурцес</span><span class="sxs-lookup"><span data-stu-id="1894b-142">includedSources</span></span>|<span data-ttu-id="1894b-143">sourceType</span><span class="sxs-lookup"><span data-stu-id="1894b-143">sourceType</span></span>|<span data-ttu-id="1894b-144">Указывает, какие источники включены в эту группу.</span><span class="sxs-lookup"><span data-stu-id="1894b-144">Specifies which sources are included in this group.</span></span> <span data-ttu-id="1894b-145">Возможные значения: `mailbox`, `site`.</span><span class="sxs-lookup"><span data-stu-id="1894b-145">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="1894b-146">значения sourceType</span><span class="sxs-lookup"><span data-stu-id="1894b-146">sourceType values</span></span>

<span data-ttu-id="1894b-147">Типы источника, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="1894b-147">Types of source related to the user.</span></span> <span data-ttu-id="1894b-148">Включает почтовый ящик и сайт по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1894b-148">Includes mailbox and site by default.</span></span>

|<span data-ttu-id="1894b-149">Member</span><span class="sxs-lookup"><span data-stu-id="1894b-149">Member</span></span>|<span data-ttu-id="1894b-150">Описание</span><span class="sxs-lookup"><span data-stu-id="1894b-150">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="1894b-151">mailbox</span><span class="sxs-lookup"><span data-stu-id="1894b-151">mailbox</span></span>|<span data-ttu-id="1894b-152">Представляет почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="1894b-152">Represents a mailbox.</span></span>|
|<span data-ttu-id="1894b-153">site</span><span class="sxs-lookup"><span data-stu-id="1894b-153">site</span></span>|<span data-ttu-id="1894b-154">Представляет сайт OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1894b-154">Represents a OneDrive for Business site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1894b-155">Связи</span><span class="sxs-lookup"><span data-stu-id="1894b-155">Relationships</span></span>

<span data-ttu-id="1894b-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1894b-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1894b-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1894b-157">JSON representation</span></span>

<span data-ttu-id="1894b-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1894b-158">The following is a JSON representation of the resource.</span></span>
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
