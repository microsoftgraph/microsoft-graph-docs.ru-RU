---
title: Тип ресурса "журнал"
description: Журнал в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 041de72a3372fd80063b96ba73d10272247c4fdb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503749"
---
# <a name="journal-resource-type"></a><span data-ttu-id="9fb35-103">Тип ресурса "журнал"</span><span class="sxs-lookup"><span data-stu-id="9fb35-103">journal resource type</span></span>

<span data-ttu-id="9fb35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fb35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fb35-105">Представляет журнал в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="9fb35-105">Represents a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="9fb35-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9fb35-106">Methods</span></span>

| <span data-ttu-id="9fb35-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9fb35-107">Method</span></span>                                            |<span data-ttu-id="9fb35-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9fb35-108">Return Type</span></span>|<span data-ttu-id="9fb35-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9fb35-109">Description</span></span>    |
|:--------------------------------------------------|:----------|:--------------|
|[<span data-ttu-id="9fb35-110">Получение журнала</span><span class="sxs-lookup"><span data-stu-id="9fb35-110">Get journal</span></span>](../api/dynamics-journal-get.md)      |<span data-ttu-id="9fb35-111">Фин</span><span class="sxs-lookup"><span data-stu-id="9fb35-111">journal</span></span>    |<span data-ttu-id="9fb35-112">Получает журнал.</span><span class="sxs-lookup"><span data-stu-id="9fb35-112">Gets a journal.</span></span>   |
|[<span data-ttu-id="9fb35-113">Разноска журнала</span><span class="sxs-lookup"><span data-stu-id="9fb35-113">Post journal</span></span>](../api/dynamics-create-journal.md)  |<span data-ttu-id="9fb35-114">Фин</span><span class="sxs-lookup"><span data-stu-id="9fb35-114">journal</span></span>    |<span data-ttu-id="9fb35-115">Создает журнал.</span><span class="sxs-lookup"><span data-stu-id="9fb35-115">Creates a journal.</span></span>|
|[<span data-ttu-id="9fb35-116">Журнал исправлений</span><span class="sxs-lookup"><span data-stu-id="9fb35-116">Patch journal</span></span>](../api/dynamics-journal-update.md) |<span data-ttu-id="9fb35-117">Фин</span><span class="sxs-lookup"><span data-stu-id="9fb35-117">journal</span></span>    |<span data-ttu-id="9fb35-118">Обновляет журнал.</span><span class="sxs-lookup"><span data-stu-id="9fb35-118">Updates a journal.</span></span>|
|[<span data-ttu-id="9fb35-119">Удаление журнала</span><span class="sxs-lookup"><span data-stu-id="9fb35-119">Delete journal</span></span>](../api/dynamics-journal-delete.md)|<span data-ttu-id="9fb35-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9fb35-120">none</span></span>       |<span data-ttu-id="9fb35-121">Удаляет журнал.</span><span class="sxs-lookup"><span data-stu-id="9fb35-121">Deletes a journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="9fb35-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fb35-122">Properties</span></span>
| <span data-ttu-id="9fb35-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fb35-123">Property</span></span>           | <span data-ttu-id="9fb35-124">Тип</span><span class="sxs-lookup"><span data-stu-id="9fb35-124">Type</span></span>                  |<span data-ttu-id="9fb35-125">Описание</span><span class="sxs-lookup"><span data-stu-id="9fb35-125">Description</span></span>                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|<span data-ttu-id="9fb35-126">id</span><span class="sxs-lookup"><span data-stu-id="9fb35-126">id</span></span>                  |<span data-ttu-id="9fb35-127">GUID</span><span class="sxs-lookup"><span data-stu-id="9fb35-127">GUID</span></span>                   |<span data-ttu-id="9fb35-128">Уникальный идентификатор журнала.</span><span class="sxs-lookup"><span data-stu-id="9fb35-128">The unique ID of the journal.</span></span> <span data-ttu-id="9fb35-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="9fb35-129">Non-editable.</span></span>           |
|<span data-ttu-id="9fb35-130">code</span><span class="sxs-lookup"><span data-stu-id="9fb35-130">code</span></span>                |<span data-ttu-id="9fb35-131">Строка, максимальный размер 10</span><span class="sxs-lookup"><span data-stu-id="9fb35-131">string, maximum size 10</span></span>| <span data-ttu-id="9fb35-132">Код журнала.</span><span class="sxs-lookup"><span data-stu-id="9fb35-132">The code of the journal.</span></span>                             |
|<span data-ttu-id="9fb35-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9fb35-133">displayName</span></span>         |<span data-ttu-id="9fb35-134">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="9fb35-134">string, maximum size 50</span></span>| <span data-ttu-id="9fb35-135">Отображаемое имя журнала.</span><span class="sxs-lookup"><span data-stu-id="9fb35-135">The display name of the journal.</span></span>                     |
|<span data-ttu-id="9fb35-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fb35-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9fb35-137">datetime</span><span class="sxs-lookup"><span data-stu-id="9fb35-137">datetime</span></span>               |<span data-ttu-id="9fb35-138">Дата и время последнего изменения, внесенные в журнал.</span><span class="sxs-lookup"><span data-stu-id="9fb35-138">The last datetime the journal was modified.</span></span> <span data-ttu-id="9fb35-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9fb35-139">Read-Only.</span></span>|

## <a name="bound-actions"></a><span data-ttu-id="9fb35-140">Связанные действия</span><span class="sxs-lookup"><span data-stu-id="9fb35-140">Bound actions</span></span>
<span data-ttu-id="9fb35-141">Тип ресурса журнал предоставляет связанное действие `post` , которое отправляет соответствующий раздел общего журнала.</span><span class="sxs-lookup"><span data-stu-id="9fb35-141">The journal resource type offers a bound action called `post` which posts the corresponding general journal batch.</span></span>

<span data-ttu-id="9fb35-142">Учет раздела общего журнала показано в следующем примере:</span><span class="sxs-lookup"><span data-stu-id="9fb35-142">Posting the general journal batch is illustrated in the following example:</span></span>  
<span data-ttu-id="9fb35-143">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span><span class="sxs-lookup"><span data-stu-id="9fb35-143">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span></span>

<span data-ttu-id="9fb35-144">Ответ не имеет контента; код ответа — 204.</span><span class="sxs-lookup"><span data-stu-id="9fb35-144">The response has no content; the response code is 204.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fb35-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fb35-145">JSON representation</span></span>

<span data-ttu-id="9fb35-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fb35-146">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

