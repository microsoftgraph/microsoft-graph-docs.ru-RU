---
title: Тип ресурса Таксграупс
description: Объект налоговой группы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 373e4785d19a7983f890ee3c3574533323829954
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027043"
---
# <a name="taxgroups-resource-type"></a><span data-ttu-id="13ba0-103">Тип ресурса Таксграупс</span><span class="sxs-lookup"><span data-stu-id="13ba0-103">taxGroups resource type</span></span>

<span data-ttu-id="13ba0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13ba0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13ba0-105">Представляет тип ресурса Таксграупс в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="13ba0-105">Represents a taxGroups resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="13ba0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="13ba0-106">Methods</span></span>
| <span data-ttu-id="13ba0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="13ba0-107">Method</span></span>       | <span data-ttu-id="13ba0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="13ba0-108">Return Type</span></span>  |<span data-ttu-id="13ba0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="13ba0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="13ba0-110">Получение Таксграупс</span><span class="sxs-lookup"><span data-stu-id="13ba0-110">Get taxGroups</span></span>](../api/dynamics-taxgroups-get.md)|<span data-ttu-id="13ba0-111">таксграупс</span><span class="sxs-lookup"><span data-stu-id="13ba0-111">taxGroups</span></span>|<span data-ttu-id="13ba0-112">Получает объект налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="13ba0-112">Gets a tax group object.</span></span>|
|[<span data-ttu-id="13ba0-113">POST Таксграупс</span><span class="sxs-lookup"><span data-stu-id="13ba0-113">Post taxGroups</span></span>](../api/dynamics-create-taxgroups.md)|<span data-ttu-id="13ba0-114">таксграупс</span><span class="sxs-lookup"><span data-stu-id="13ba0-114">taxGroups</span></span>|<span data-ttu-id="13ba0-115">Создает объект налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="13ba0-115">Creates a tax group object.</span></span>|
|[<span data-ttu-id="13ba0-116">Исправление Таксграупс</span><span class="sxs-lookup"><span data-stu-id="13ba0-116">Patch taxGroups</span></span>](../api/dynamics-taxgroups-update.md)|<span data-ttu-id="13ba0-117">таксграупс</span><span class="sxs-lookup"><span data-stu-id="13ba0-117">taxGroups</span></span>|<span data-ttu-id="13ba0-118">Обновляет объект налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="13ba0-118">Updates a tax group object.</span></span>|
|[<span data-ttu-id="13ba0-119">Удаление Таксграупс</span><span class="sxs-lookup"><span data-stu-id="13ba0-119">Delete taxGroups</span></span>](../api/dynamics-taxgroups-delete.md)|<span data-ttu-id="13ba0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="13ba0-120">none</span></span>|<span data-ttu-id="13ba0-121">Удаляет объект налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="13ba0-121">Deletes a tax group object.</span></span>|

## <a name="properties"></a><span data-ttu-id="13ba0-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="13ba0-122">Properties</span></span>
| <span data-ttu-id="13ba0-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="13ba0-123">Property</span></span>     | <span data-ttu-id="13ba0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="13ba0-124">Type</span></span>   |<span data-ttu-id="13ba0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="13ba0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13ba0-126">id</span><span class="sxs-lookup"><span data-stu-id="13ba0-126">id</span></span>|<span data-ttu-id="13ba0-127">GUID</span><span class="sxs-lookup"><span data-stu-id="13ba0-127">GUID</span></span>|<span data-ttu-id="13ba0-128">Уникальный идентификатор Таксграуп.</span><span class="sxs-lookup"><span data-stu-id="13ba0-128">The unique ID of the taxGroup.</span></span> <span data-ttu-id="13ba0-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13ba0-129">Read-Only.</span></span>|
|<span data-ttu-id="13ba0-130">code</span><span class="sxs-lookup"><span data-stu-id="13ba0-130">code</span></span>|<span data-ttu-id="13ba0-131">string</span><span class="sxs-lookup"><span data-stu-id="13ba0-131">string</span></span>|<span data-ttu-id="13ba0-132">Указывает налоговую группу.</span><span class="sxs-lookup"><span data-stu-id="13ba0-132">Specifies the tax group.</span></span>|
|<span data-ttu-id="13ba0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="13ba0-133">displayName</span></span>|<span data-ttu-id="13ba0-134">string</span><span class="sxs-lookup"><span data-stu-id="13ba0-134">string</span></span>|<span data-ttu-id="13ba0-135">Задает отображаемое имя налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="13ba0-135">Specifies the tax group display name.</span></span>|
|<span data-ttu-id="13ba0-136">такстипе</span><span class="sxs-lookup"><span data-stu-id="13ba0-136">taxType</span></span>|<span data-ttu-id="13ba0-137">string</span><span class="sxs-lookup"><span data-stu-id="13ba0-137">string</span></span>|<span data-ttu-id="13ba0-138">Указывает тип налога для группы.</span><span class="sxs-lookup"><span data-stu-id="13ba0-138">Specifies the tax type for the group.</span></span>|
|<span data-ttu-id="13ba0-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13ba0-139">lastModifiedDateTime</span></span>|<span data-ttu-id="13ba0-140">datetime</span><span class="sxs-lookup"><span data-stu-id="13ba0-140">datetime</span></span>|<span data-ttu-id="13ba0-141">Дата и время последнего изменения налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="13ba0-141">The last datetime the tax group was modified.</span></span> <span data-ttu-id="13ba0-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13ba0-142">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="13ba0-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="13ba0-143">Relationships</span></span>
<span data-ttu-id="13ba0-144">Нет</span><span class="sxs-lookup"><span data-stu-id="13ba0-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13ba0-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13ba0-145">JSON representation</span></span>

<span data-ttu-id="13ba0-146">Ниже показано представление объекта Таксграуп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13ba0-146">Here is a JSON representation of the taxGroup.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```




