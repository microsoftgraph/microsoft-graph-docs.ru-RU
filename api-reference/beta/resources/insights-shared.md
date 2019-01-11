---
title: тип общего ресурса
description: 'Возможность получения, представляющих файлы совместно с помощью или отдельного пользователя. Поддерживаются следующие общие файлы:'
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 289523f836d7b8080f7317e4d11301c71314ba93
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880614"
---
# <a name="shared-resource-type"></a><span data-ttu-id="ed35e-104">тип общего ресурса</span><span class="sxs-lookup"><span data-stu-id="ed35e-104">shared resource type</span></span>

> <span data-ttu-id="ed35e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ed35e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed35e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed35e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed35e-107">Возможность получения, представляющих файлы совместно с помощью или отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ed35e-107">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="ed35e-108">Поддерживаются следующие общие файлы:</span><span class="sxs-lookup"><span data-stu-id="ed35e-108">The following shared files are supported:</span></span>

- <span data-ttu-id="ed35e-109">Приглашение файлами, вложенными непосредственно в сообщение электронной почты или встрече.</span><span class="sxs-lookup"><span data-stu-id="ed35e-109">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="ed35e-110">OneDrive для Bussiness и SharePoint современных вложения - файлов, хранящихся в OneDrive для бизнеса и SharePoint, которые пользователи совместно использовать как ссылки в сообщении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ed35e-110">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="ed35e-111">**Примечание**: Корпорация Майкрософт в настоящее время работает на заполнение результатов API совместно с данными.</span><span class="sxs-lookup"><span data-stu-id="ed35e-111">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="ed35e-112">Возможно, некоторые данные, отсутствующие в первой недели после выпуска.</span><span class="sxs-lookup"><span data-stu-id="ed35e-112">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="ed35e-113">Методы</span><span class="sxs-lookup"><span data-stu-id="ed35e-113">Methods</span></span>

| <span data-ttu-id="ed35e-114">Метод</span><span class="sxs-lookup"><span data-stu-id="ed35e-114">Method</span></span>       | <span data-ttu-id="ed35e-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ed35e-115">Return Type</span></span>  |<span data-ttu-id="ed35e-116">Описание</span><span class="sxs-lookup"><span data-stu-id="ed35e-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed35e-117">Список общих</span><span class="sxs-lookup"><span data-stu-id="ed35e-117">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="ed35e-118">[insights_shared](insights-shared.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ed35e-118">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="ed35e-119">Получите список общих файлов.</span><span class="sxs-lookup"><span data-stu-id="ed35e-119">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed35e-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed35e-120">Properties</span></span>

| <span data-ttu-id="ed35e-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed35e-121">Property</span></span>              | <span data-ttu-id="ed35e-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ed35e-122">Type</span></span>                      | <span data-ttu-id="ed35e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ed35e-123">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="ed35e-124">id</span><span class="sxs-lookup"><span data-stu-id="ed35e-124">id</span></span>                    | <span data-ttu-id="ed35e-125">Строка</span><span class="sxs-lookup"><span data-stu-id="ed35e-125">String</span></span>                    | <span data-ttu-id="ed35e-126">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="ed35e-126">Unique identifier of the relationship.</span></span> <span data-ttu-id="ed35e-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed35e-127">Read only.</span></span>        |
| <span data-ttu-id="ed35e-128">lastShared</span><span class="sxs-lookup"><span data-stu-id="ed35e-128">lastShared</span></span>            | [<span data-ttu-id="ed35e-129">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="ed35e-129">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="ed35e-130">Сведения об общих элементов.</span><span class="sxs-lookup"><span data-stu-id="ed35e-130">Details about the shared item.</span></span> <span data-ttu-id="ed35e-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed35e-131">Read only.</span></span>        |
| <span data-ttu-id="ed35e-132">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="ed35e-132">resourceVisualization</span></span> | [<span data-ttu-id="ed35e-133">resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="ed35e-133">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="ed35e-134">Свойства, которые можно использовать для визуализации документа в работу.</span><span class="sxs-lookup"><span data-stu-id="ed35e-134">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="ed35e-135">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="ed35e-135">Read-only</span></span>      |
| <span data-ttu-id="ed35e-136">resourceReference</span><span class="sxs-lookup"><span data-stu-id="ed35e-136">resourceReference</span></span>     | [<span data-ttu-id="ed35e-137">resourceReference</span><span class="sxs-lookup"><span data-stu-id="ed35e-137">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="ed35e-138">Свойства ссылки общих документов, таких как URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="ed35e-138">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="ed35e-139">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="ed35e-139">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="ed35e-140">Связи</span><span class="sxs-lookup"><span data-stu-id="ed35e-140">Relationships</span></span>

| <span data-ttu-id="ed35e-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed35e-141">Property</span></span>      | <span data-ttu-id="ed35e-142">Тип</span><span class="sxs-lookup"><span data-stu-id="ed35e-142">Type</span></span>          | <span data-ttu-id="ed35e-143">Описание</span><span class="sxs-lookup"><span data-stu-id="ed35e-143">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="ed35e-144">resource</span><span class="sxs-lookup"><span data-stu-id="ed35e-144">resource</span></span>      | <span data-ttu-id="ed35e-145">Entity</span><span class="sxs-lookup"><span data-stu-id="ed35e-145">Entity</span></span>        | <span data-ttu-id="ed35e-146">Используется для перехода к элементу, предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="ed35e-146">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="ed35e-147">Для файлов вложений тип — *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="ed35e-147">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="ed35e-148">Для связанного вложения тип — *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="ed35e-148">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ed35e-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed35e-149">JSON representation</span></span>
<span data-ttu-id="ed35e-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed35e-150">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
