---
title: Тип ресурса Каунтриесрегионс
description: Объект страны и регионы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 73f60a48e1b7b3564851271209e195ecbbf171e2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012634"
---
# <a name="countriesregions-resource-type"></a><span data-ttu-id="fbe0f-103">Тип ресурса Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="fbe0f-103">countriesRegions resource type</span></span>
<span data-ttu-id="fbe0f-104">Представляет объект Каунтриесрегионс в Dynamics 365 Business Central, который является частью адреса.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-104">Represents a countriesRegions object in Dynamics 365 Business Central, which is part of an address.</span></span>

## <a name="methods"></a><span data-ttu-id="fbe0f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="fbe0f-105">Methods</span></span>

| <span data-ttu-id="fbe0f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="fbe0f-106">Method</span></span>                                                              | <span data-ttu-id="fbe0f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fbe0f-107">Return Type</span></span>    |<span data-ttu-id="fbe0f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fbe0f-108">Description</span></span>                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[<span data-ttu-id="fbe0f-109">Получение Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="fbe0f-109">Get countriesRegions</span></span>](../api/dynamics-countriesregions-get.md)      |<span data-ttu-id="fbe0f-110">Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="fbe0f-110">countriesRegions</span></span>|<span data-ttu-id="fbe0f-111">Получение стран и регионов.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-111">Get a Countries/Regions.</span></span>   |
|[<span data-ttu-id="fbe0f-112">POST Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="fbe0f-112">Post countriesRegions</span></span>](../api/dynamics-create-countriesregions.md)  |<span data-ttu-id="fbe0f-113">Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="fbe0f-113">countriesRegions</span></span>|<span data-ttu-id="fbe0f-114">Создание стран и регионов.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-114">Create a Countries/Regions.</span></span>|
|[<span data-ttu-id="fbe0f-115">Исправление Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="fbe0f-115">Patch countriesRegions</span></span>](../api/dynamics-countriesregions-update.md) |<span data-ttu-id="fbe0f-116">Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="fbe0f-116">countriesRegions</span></span>|<span data-ttu-id="fbe0f-117">Обновление стран и регионов.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-117">Update a Countries/Regions.</span></span>|
|[<span data-ttu-id="fbe0f-118">Удаление Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="fbe0f-118">Delete countriesRegions</span></span>](../api/dynamics-countriesregions-delete.md)|<span data-ttu-id="fbe0f-119">none</span><span class="sxs-lookup"><span data-stu-id="fbe0f-119">none</span></span>            |<span data-ttu-id="fbe0f-120">Удаление стран и регионов.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-120">Delete a Countries/Regions.</span></span>|

## <a name="properties"></a><span data-ttu-id="fbe0f-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="fbe0f-121">Properties</span></span>
| <span data-ttu-id="fbe0f-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbe0f-122">Property</span></span>       | <span data-ttu-id="fbe0f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="fbe0f-123">Type</span></span>       |<span data-ttu-id="fbe0f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fbe0f-124">Description</span></span>                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|<span data-ttu-id="fbe0f-125">id</span><span class="sxs-lookup"><span data-stu-id="fbe0f-125">id</span></span>              |<span data-ttu-id="fbe0f-126">GUID</span><span class="sxs-lookup"><span data-stu-id="fbe0f-126">GUID</span></span>        |<span data-ttu-id="fbe0f-127">Уникальный идентификатор страны или региона.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-127">The unique ID of the country/region.</span></span> <span data-ttu-id="fbe0f-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-128">Non-editable.</span></span>           |
|<span data-ttu-id="fbe0f-129">code</span><span class="sxs-lookup"><span data-stu-id="fbe0f-129">code</span></span>            |<span data-ttu-id="fbe0f-130">string</span><span class="sxs-lookup"><span data-stu-id="fbe0f-130">string</span></span>      |<span data-ttu-id="fbe0f-131">Указывает код страны или региона.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-131">Specifies the code of the country/region.</span></span>                    |
|<span data-ttu-id="fbe0f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="fbe0f-132">displayName</span></span>     |<span data-ttu-id="fbe0f-133">string</span><span class="sxs-lookup"><span data-stu-id="fbe0f-133">string</span></span>      |<span data-ttu-id="fbe0f-134">Задает отображаемое имя страны или региона.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-134">Specifies the display name of the country/region.</span></span>            |
|<span data-ttu-id="fbe0f-135">Аддрессформат</span><span class="sxs-lookup"><span data-stu-id="fbe0f-135">addressFormat</span></span>   |<span data-ttu-id="fbe0f-136">string</span><span class="sxs-lookup"><span data-stu-id="fbe0f-136">string</span></span>      |<span data-ttu-id="fbe0f-137">Указывает формат адреса, отображаемого в документах с внешними разворотами.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-137">Specifies the format of the address that is displayed on external-facing documents.</span></span> <span data-ttu-id="fbe0f-138">Вы связываете формат адреса с кодом страны или региона, чтобы документы с внешними разворотами на основе карточек или документов с этим кодом страны или региона использовали указанный формат адреса.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-138">You link an address format to a country/region code so that external-facing documents based on cards or documents with that country/region code use the specified address format.</span></span>|
|<span data-ttu-id="fbe0f-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbe0f-139">lastModifiedDateTime</span></span>|<span data-ttu-id="fbe0f-140">отличным</span><span class="sxs-lookup"><span data-stu-id="fbe0f-140">datetime</span></span>|<span data-ttu-id="fbe0f-141">Дата и время последнего изменения страны или региона.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-141">The last datetime the country/region was modified.</span></span> <span data-ttu-id="fbe0f-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-142">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="fbe0f-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="fbe0f-143">Relationships</span></span>
<span data-ttu-id="fbe0f-144">Нет</span><span class="sxs-lookup"><span data-stu-id="fbe0f-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbe0f-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fbe0f-145">JSON representation</span></span>

<span data-ttu-id="fbe0f-146">Ниже показано представление объекта Каунтриесрегионс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbe0f-146">Here is a JSON representation of the countriesRegions.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "addressFormat": "string",
  "lastModifiedDateTime": "datetime"
}

```


