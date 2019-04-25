---
title: Тип ресурса Таксграупс
description: Объект налоговой группы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: bdfbec8f5373637924262388dab0e9c74c363af9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543128"
---
# <a name="taxgroups-resource-type"></a><span data-ttu-id="8772f-103">Тип ресурса Таксграупс</span><span class="sxs-lookup"><span data-stu-id="8772f-103">taxGroups resource type</span></span>
<span data-ttu-id="8772f-104">Представляет тип ресурса Таксграупс в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="8772f-104">Represents a taxGroups resource type in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="8772f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="8772f-105">Methods</span></span>
| <span data-ttu-id="8772f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="8772f-106">Method</span></span>       | <span data-ttu-id="8772f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8772f-107">Return Type</span></span>  |<span data-ttu-id="8772f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8772f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8772f-109">Получение Таксграупс</span><span class="sxs-lookup"><span data-stu-id="8772f-109">Get taxGroups</span></span>](../api/dynamics-taxgroups-get.md)|<span data-ttu-id="8772f-110">Таксграупс</span><span class="sxs-lookup"><span data-stu-id="8772f-110">taxGroups</span></span>|<span data-ttu-id="8772f-111">Получает объект налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="8772f-111">Gets a tax group object.</span></span>|
|[<span data-ttu-id="8772f-112">POST Таксграупс</span><span class="sxs-lookup"><span data-stu-id="8772f-112">Post taxGroups</span></span>](../api/dynamics-create-taxgroups.md)|<span data-ttu-id="8772f-113">Таксграупс</span><span class="sxs-lookup"><span data-stu-id="8772f-113">taxGroups</span></span>|<span data-ttu-id="8772f-114">Создает объект налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="8772f-114">Creates a tax group object.</span></span>|
|[<span data-ttu-id="8772f-115">Исправление Таксграупс</span><span class="sxs-lookup"><span data-stu-id="8772f-115">Patch taxGroups</span></span>](../api/dynamics-taxgroups-update.md)|<span data-ttu-id="8772f-116">Таксграупс</span><span class="sxs-lookup"><span data-stu-id="8772f-116">taxGroups</span></span>|<span data-ttu-id="8772f-117">Обновляет объект налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="8772f-117">Updates a tax group object.</span></span>|
|[<span data-ttu-id="8772f-118">Удаление Таксграупс</span><span class="sxs-lookup"><span data-stu-id="8772f-118">Delete taxGroups</span></span>](../api/dynamics-taxgroups-delete.md)|<span data-ttu-id="8772f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8772f-119">none</span></span>|<span data-ttu-id="8772f-120">Удаляет объект налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="8772f-120">Deletes a tax group object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8772f-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="8772f-121">Properties</span></span>
| <span data-ttu-id="8772f-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="8772f-122">Property</span></span>     | <span data-ttu-id="8772f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8772f-123">Type</span></span>   |<span data-ttu-id="8772f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8772f-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8772f-125">id</span><span class="sxs-lookup"><span data-stu-id="8772f-125">id</span></span>|<span data-ttu-id="8772f-126">Глобальный уникальный идентификатор (GUID)</span><span class="sxs-lookup"><span data-stu-id="8772f-126">GUID</span></span>|<span data-ttu-id="8772f-127">Уникальный идентификатор Таксграуп.</span><span class="sxs-lookup"><span data-stu-id="8772f-127">The unique ID of the taxGroup.</span></span> <span data-ttu-id="8772f-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8772f-128">Read-Only.</span></span>|
|<span data-ttu-id="8772f-129">code</span><span class="sxs-lookup"><span data-stu-id="8772f-129">code</span></span>|<span data-ttu-id="8772f-130">string</span><span class="sxs-lookup"><span data-stu-id="8772f-130">string</span></span>|<span data-ttu-id="8772f-131">Указывает налоговую группу.</span><span class="sxs-lookup"><span data-stu-id="8772f-131">Specifies the tax group.</span></span>|
|<span data-ttu-id="8772f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8772f-132">displayName</span></span>|<span data-ttu-id="8772f-133">string</span><span class="sxs-lookup"><span data-stu-id="8772f-133">string</span></span>|<span data-ttu-id="8772f-134">Задает отображаемое имя налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="8772f-134">Specifies the tax group display name.</span></span>|
|<span data-ttu-id="8772f-135">Такстипе</span><span class="sxs-lookup"><span data-stu-id="8772f-135">taxType</span></span>|<span data-ttu-id="8772f-136">string</span><span class="sxs-lookup"><span data-stu-id="8772f-136">string</span></span>|<span data-ttu-id="8772f-137">Указывает тип налога для группы.</span><span class="sxs-lookup"><span data-stu-id="8772f-137">Specifies the tax type for the group.</span></span>|
|<span data-ttu-id="8772f-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8772f-138">lastModifiedDateTime</span></span>|<span data-ttu-id="8772f-139">отличным</span><span class="sxs-lookup"><span data-stu-id="8772f-139">datetime</span></span>|<span data-ttu-id="8772f-140">Дата и время последнего изменения налоговой группы.</span><span class="sxs-lookup"><span data-stu-id="8772f-140">The last datetime the tax group was modified.</span></span> <span data-ttu-id="8772f-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8772f-141">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="8772f-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="8772f-142">Relationships</span></span>
<span data-ttu-id="8772f-143">Нет</span><span class="sxs-lookup"><span data-stu-id="8772f-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8772f-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8772f-144">JSON representation</span></span>

<span data-ttu-id="8772f-145">Ниже показано представление объекта Таксграуп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8772f-145">Here is a JSON representation of the taxGroup.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "taxType": "string",
  "lastModifiedDateTime": "datetime"
}

```


