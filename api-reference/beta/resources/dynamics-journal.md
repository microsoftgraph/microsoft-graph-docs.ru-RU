---
title: Тип ресурса "журнал"
description: Журнал в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 7cfc723a4370c2b30440dcd4e33b50ed066ac89b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006594"
---
# <a name="journal-resource-type"></a><span data-ttu-id="a0c5e-103">Тип ресурса "журнал"</span><span class="sxs-lookup"><span data-stu-id="a0c5e-103">journal resource type</span></span>
<span data-ttu-id="a0c5e-104">Представляет журнал в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-104">Represents a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="a0c5e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a0c5e-105">Methods</span></span>

| <span data-ttu-id="a0c5e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a0c5e-106">Method</span></span>                                            |<span data-ttu-id="a0c5e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a0c5e-107">Return Type</span></span>|<span data-ttu-id="a0c5e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a0c5e-108">Description</span></span>    |
|:--------------------------------------------------|:----------|:--------------|
|[<span data-ttu-id="a0c5e-109">Получение журнала</span><span class="sxs-lookup"><span data-stu-id="a0c5e-109">Get journal</span></span>](../api/dynamics-journal-get.md)      |<span data-ttu-id="a0c5e-110">Фин</span><span class="sxs-lookup"><span data-stu-id="a0c5e-110">journal</span></span>    |<span data-ttu-id="a0c5e-111">Получает журнал.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-111">Gets a journal.</span></span>   |
|[<span data-ttu-id="a0c5e-112">Разноска журнала</span><span class="sxs-lookup"><span data-stu-id="a0c5e-112">Post journal</span></span>](../api/dynamics-create-journal.md)  |<span data-ttu-id="a0c5e-113">Фин</span><span class="sxs-lookup"><span data-stu-id="a0c5e-113">journal</span></span>    |<span data-ttu-id="a0c5e-114">Создает журнал.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-114">Creates a journal.</span></span>|
|[<span data-ttu-id="a0c5e-115">Журнал исправлений</span><span class="sxs-lookup"><span data-stu-id="a0c5e-115">Patch journal</span></span>](../api/dynamics-journal-update.md) |<span data-ttu-id="a0c5e-116">Фин</span><span class="sxs-lookup"><span data-stu-id="a0c5e-116">journal</span></span>    |<span data-ttu-id="a0c5e-117">Обновляет журнал.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-117">Updates a journal.</span></span>|
|[<span data-ttu-id="a0c5e-118">Удаление журнала</span><span class="sxs-lookup"><span data-stu-id="a0c5e-118">Delete journal</span></span>](../api/dynamics-journal-delete.md)|<span data-ttu-id="a0c5e-119">none</span><span class="sxs-lookup"><span data-stu-id="a0c5e-119">none</span></span>       |<span data-ttu-id="a0c5e-120">Удаляет журнал.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-120">Deletes a journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="a0c5e-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0c5e-121">Properties</span></span>
| <span data-ttu-id="a0c5e-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0c5e-122">Property</span></span>           | <span data-ttu-id="a0c5e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="a0c5e-123">Type</span></span>                  |<span data-ttu-id="a0c5e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a0c5e-124">Description</span></span>                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|<span data-ttu-id="a0c5e-125">id</span><span class="sxs-lookup"><span data-stu-id="a0c5e-125">id</span></span>                  |<span data-ttu-id="a0c5e-126">GUID</span><span class="sxs-lookup"><span data-stu-id="a0c5e-126">GUID</span></span>                   |<span data-ttu-id="a0c5e-127">Уникальный идентификатор журнала.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-127">The unique ID of the journal.</span></span> <span data-ttu-id="a0c5e-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-128">Non-editable.</span></span>           |
|<span data-ttu-id="a0c5e-129">code</span><span class="sxs-lookup"><span data-stu-id="a0c5e-129">code</span></span>                |<span data-ttu-id="a0c5e-130">Строка, максимальный размер 10</span><span class="sxs-lookup"><span data-stu-id="a0c5e-130">string, maximum size 10</span></span>| <span data-ttu-id="a0c5e-131">Код журнала.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-131">The code of the journal.</span></span>                             |
|<span data-ttu-id="a0c5e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a0c5e-132">displayName</span></span>         |<span data-ttu-id="a0c5e-133">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="a0c5e-133">string, maximum size 50</span></span>| <span data-ttu-id="a0c5e-134">Отображаемое имя журнала.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-134">The display name of the journal.</span></span>                     |
|<span data-ttu-id="a0c5e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0c5e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a0c5e-136">отличным</span><span class="sxs-lookup"><span data-stu-id="a0c5e-136">datetime</span></span>               |<span data-ttu-id="a0c5e-137">Дата и время последнего изменения, внесенные в журнал.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-137">The last datetime the journal was modified.</span></span> <span data-ttu-id="a0c5e-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-138">Read-Only.</span></span>|

## <a name="bound-actions"></a><span data-ttu-id="a0c5e-139">Связанные действия</span><span class="sxs-lookup"><span data-stu-id="a0c5e-139">Bound actions</span></span>
<span data-ttu-id="a0c5e-140">Тип ресурса журнал предоставляет связанное действие `post` , которое отправляет соответствующий раздел общего журнала.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-140">The journal resource type offers a bound action called `post` which posts the corresponding general journal batch.</span></span>

<span data-ttu-id="a0c5e-141">Учет раздела общего журнала показано в следующем примере:</span><span class="sxs-lookup"><span data-stu-id="a0c5e-141">Posting the general journal batch is illustrated in the following example:</span></span>  
<span data-ttu-id="a0c5e-142">`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-142"></span></span>

<span data-ttu-id="a0c5e-143">Ответ не имеет контента; код ответа — 204.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-143">The response has no content; the response code is 204.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0c5e-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0c5e-144">JSON representation</span></span>

<span data-ttu-id="a0c5e-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0c5e-145">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

