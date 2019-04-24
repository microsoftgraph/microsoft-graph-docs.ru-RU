---
title: Тип ресурса Каунтриесрегионс
description: Объект страны и регионы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: b6f50ba3046a402f2b8729529675653286808459
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507268"
---
# <a name="countriesregions-resource-type"></a><span data-ttu-id="db213-103">Тип ресурса Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="db213-103">countriesRegions resource type</span></span>
<span data-ttu-id="db213-104">Представляет объект Каунтриесрегионс в Dynamics 365 Business Central, который является частью адреса.</span><span class="sxs-lookup"><span data-stu-id="db213-104">Represents a countriesRegions object in Dynamics 365 Business Central, which is part of an address.</span></span>

## <a name="methods"></a><span data-ttu-id="db213-105">Методы</span><span class="sxs-lookup"><span data-stu-id="db213-105">Methods</span></span>

| <span data-ttu-id="db213-106">Метод</span><span class="sxs-lookup"><span data-stu-id="db213-106">Method</span></span>                                                              | <span data-ttu-id="db213-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="db213-107">Return Type</span></span>    |<span data-ttu-id="db213-108">Описание</span><span class="sxs-lookup"><span data-stu-id="db213-108">Description</span></span>                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[<span data-ttu-id="db213-109">Получение Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="db213-109">Get countriesRegions</span></span>](../api/dynamics-countriesregions-get.md)      |<span data-ttu-id="db213-110">Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="db213-110">countriesRegions</span></span>|<span data-ttu-id="db213-111">Получение стран и регионов.</span><span class="sxs-lookup"><span data-stu-id="db213-111">Get a Countries/Regions.</span></span>   |
|[<span data-ttu-id="db213-112">POST Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="db213-112">Post countriesRegions</span></span>](../api/dynamics-create-countriesregions.md)  |<span data-ttu-id="db213-113">Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="db213-113">countriesRegions</span></span>|<span data-ttu-id="db213-114">Создание стран и регионов.</span><span class="sxs-lookup"><span data-stu-id="db213-114">Create a Countries/Regions.</span></span>|
|[<span data-ttu-id="db213-115">Исправление Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="db213-115">Patch countriesRegions</span></span>](../api/dynamics-countriesregions-update.md) |<span data-ttu-id="db213-116">Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="db213-116">countriesRegions</span></span>|<span data-ttu-id="db213-117">Обновление стран и регионов.</span><span class="sxs-lookup"><span data-stu-id="db213-117">Update a Countries/Regions.</span></span>|
|[<span data-ttu-id="db213-118">Удаление Каунтриесрегионс</span><span class="sxs-lookup"><span data-stu-id="db213-118">Delete countriesRegions</span></span>](../api/dynamics-countriesregions-delete.md)|<span data-ttu-id="db213-119">Нет</span><span class="sxs-lookup"><span data-stu-id="db213-119">none</span></span>            |<span data-ttu-id="db213-120">Удаление стран и регионов.</span><span class="sxs-lookup"><span data-stu-id="db213-120">Delete a Countries/Regions.</span></span>|

## <a name="properties"></a><span data-ttu-id="db213-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="db213-121">Properties</span></span>
| <span data-ttu-id="db213-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="db213-122">Property</span></span>       | <span data-ttu-id="db213-123">Тип</span><span class="sxs-lookup"><span data-stu-id="db213-123">Type</span></span>       |<span data-ttu-id="db213-124">Описание</span><span class="sxs-lookup"><span data-stu-id="db213-124">Description</span></span>                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|<span data-ttu-id="db213-125">id</span><span class="sxs-lookup"><span data-stu-id="db213-125">id</span></span>              |<span data-ttu-id="db213-126">GUID</span><span class="sxs-lookup"><span data-stu-id="db213-126">GUID</span></span>        |<span data-ttu-id="db213-127">Уникальный идентификатор страны или региона.</span><span class="sxs-lookup"><span data-stu-id="db213-127">The unique ID of the country/region.</span></span> <span data-ttu-id="db213-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="db213-128">Non-editable.</span></span>           |
|<span data-ttu-id="db213-129">code</span><span class="sxs-lookup"><span data-stu-id="db213-129">code</span></span>            |<span data-ttu-id="db213-130">string</span><span class="sxs-lookup"><span data-stu-id="db213-130">string</span></span>      |<span data-ttu-id="db213-131">Указывает код страны или региона.</span><span class="sxs-lookup"><span data-stu-id="db213-131">Specifies the code of the country/region.</span></span>                    |
|<span data-ttu-id="db213-132">displayName</span><span class="sxs-lookup"><span data-stu-id="db213-132">displayName</span></span>     |<span data-ttu-id="db213-133">string</span><span class="sxs-lookup"><span data-stu-id="db213-133">string</span></span>      |<span data-ttu-id="db213-134">Задает отображаемое имя страны или региона.</span><span class="sxs-lookup"><span data-stu-id="db213-134">Specifies the display name of the country/region.</span></span>            |
|<span data-ttu-id="db213-135">Аддрессформат</span><span class="sxs-lookup"><span data-stu-id="db213-135">addressFormat</span></span>   |<span data-ttu-id="db213-136">строка</span><span class="sxs-lookup"><span data-stu-id="db213-136">string</span></span>      |<span data-ttu-id="db213-137">Указывает формат адреса, отображаемого в документах с внешними разворотами.</span><span class="sxs-lookup"><span data-stu-id="db213-137">Specifies the format of the address that is displayed on external-facing documents.</span></span> <span data-ttu-id="db213-138">Вы связываете формат адреса с кодом страны или региона, чтобы документы с внешними разворотами на основе карточек или документов с этим кодом страны или региона использовали указанный формат адреса.</span><span class="sxs-lookup"><span data-stu-id="db213-138">You link an address format to a country/region code so that external-facing documents based on cards or documents with that country/region code use the specified address format.</span></span>|
|<span data-ttu-id="db213-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db213-139">lastModifiedDateTime</span></span>|<span data-ttu-id="db213-140">отличным</span><span class="sxs-lookup"><span data-stu-id="db213-140">datetime</span></span>|<span data-ttu-id="db213-141">Дата и время последнего изменения страны или региона.</span><span class="sxs-lookup"><span data-stu-id="db213-141">The last datetime the country/region was modified.</span></span> <span data-ttu-id="db213-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db213-142">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="db213-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="db213-143">Relationships</span></span>
<span data-ttu-id="db213-144">Нет</span><span class="sxs-lookup"><span data-stu-id="db213-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db213-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db213-145">JSON representation</span></span>

<span data-ttu-id="db213-146">Ниже показано представление объекта Каунтриесрегионс в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db213-146">Here is a JSON representation of the countriesRegions.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "addressFormat": "string",
  "lastModifiedDateTime": "datetime"
}

```


