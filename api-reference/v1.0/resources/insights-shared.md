---
title: Тип ресурса Шарединсигхт
description: 'Понимание файлов, к которым предоставлен общий доступ, или определенного пользователя. Поддерживаются следующие общие файлы:'
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 9b7bb8c2a69ebab16171ff4a74283d0993aefc8a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532872"
---
# <a name="sharedinsight-resource-type"></a><span data-ttu-id="fabdd-104">Тип ресурса Шарединсигхт</span><span class="sxs-lookup"><span data-stu-id="fabdd-104">sharedInsight resource type</span></span>

<span data-ttu-id="fabdd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fabdd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fabdd-106">Понимание файлов, к которым предоставлен общий доступ, или определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="fabdd-106">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="fabdd-107">Поддерживаются следующие общие файлы:</span><span class="sxs-lookup"><span data-stu-id="fabdd-107">The following shared files are supported:</span></span>

- <span data-ttu-id="fabdd-108">Файлы, вложенные непосредственно в сообщение электронной почты или приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="fabdd-108">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="fabdd-109">OneDrive для бизнеса и самые современные вложения SharePoint — файлы, хранящиеся в OneDrive для бизнеса и SharePoint, которые пользователи совместно используют как ссылки в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fabdd-109">OneDrive for Business and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="fabdd-110">**Note**: в настоящее время мы работаем над заполнением результатов общего API с данными.</span><span class="sxs-lookup"><span data-stu-id="fabdd-110">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="fabdd-111">Некоторые данные могут отсутствовать в первых неделях после выпуска.</span><span class="sxs-lookup"><span data-stu-id="fabdd-111">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="fabdd-112">Методы</span><span class="sxs-lookup"><span data-stu-id="fabdd-112">Methods</span></span>

| <span data-ttu-id="fabdd-113">Метод</span><span class="sxs-lookup"><span data-stu-id="fabdd-113">Method</span></span>       | <span data-ttu-id="fabdd-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fabdd-114">Return Type</span></span>  |<span data-ttu-id="fabdd-115">Описание</span><span class="sxs-lookup"><span data-stu-id="fabdd-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fabdd-116">Список "Общие"</span><span class="sxs-lookup"><span data-stu-id="fabdd-116">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="fabdd-117">Коллекция объектов [sharedInsight](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="fabdd-117">[sharedInsight](insights-shared.md) collection</span></span>| <span data-ttu-id="fabdd-118">Получение списка общих файлов.</span><span class="sxs-lookup"><span data-stu-id="fabdd-118">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="fabdd-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="fabdd-119">Properties</span></span>

| <span data-ttu-id="fabdd-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="fabdd-120">Property</span></span>              | <span data-ttu-id="fabdd-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fabdd-121">Type</span></span>                      | <span data-ttu-id="fabdd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fabdd-122">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="fabdd-123">id</span><span class="sxs-lookup"><span data-stu-id="fabdd-123">id</span></span>                    | <span data-ttu-id="fabdd-124">String</span><span class="sxs-lookup"><span data-stu-id="fabdd-124">String</span></span>                    | <span data-ttu-id="fabdd-125">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="fabdd-125">Unique identifier of the relationship.</span></span> <span data-ttu-id="fabdd-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fabdd-126">Read only.</span></span>        |
| <span data-ttu-id="fabdd-127">ластшаред</span><span class="sxs-lookup"><span data-stu-id="fabdd-127">lastShared</span></span>            | [<span data-ttu-id="fabdd-128">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="fabdd-128">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="fabdd-129">Сведения об общем элементе.</span><span class="sxs-lookup"><span data-stu-id="fabdd-129">Details about the shared item.</span></span> <span data-ttu-id="fabdd-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fabdd-130">Read only.</span></span>        |
| <span data-ttu-id="fabdd-131">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="fabdd-131">resourceVisualization</span></span> | [<span data-ttu-id="fabdd-132">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="fabdd-132">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="fabdd-133">Свойства, которые можно использовать для отображения документа в вашем интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="fabdd-133">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="fabdd-134">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="fabdd-134">Read-only</span></span>      |
| <span data-ttu-id="fabdd-135">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="fabdd-135">resourceReference</span></span>     | [<span data-ttu-id="fabdd-136">ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="fabdd-136">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="fabdd-137">Справочные свойства общего документа, например URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="fabdd-137">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="fabdd-138">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="fabdd-138">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="fabdd-139">Связи</span><span class="sxs-lookup"><span data-stu-id="fabdd-139">Relationships</span></span>

| <span data-ttu-id="fabdd-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="fabdd-140">Property</span></span>      | <span data-ttu-id="fabdd-141">Тип</span><span class="sxs-lookup"><span data-stu-id="fabdd-141">Type</span></span>          | <span data-ttu-id="fabdd-142">Описание</span><span class="sxs-lookup"><span data-stu-id="fabdd-142">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="fabdd-143">resource</span><span class="sxs-lookup"><span data-stu-id="fabdd-143">resource</span></span>      | <span data-ttu-id="fabdd-144">Коллекция объектов</span><span class="sxs-lookup"><span data-stu-id="fabdd-144">entity collection</span></span> | <span data-ttu-id="fabdd-145">Используется для перехода к элементу, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="fabdd-145">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="fabdd-146">Для вложений в файл используется тип *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="fabdd-146">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="fabdd-147">Для связанных вложений используется тип *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="fabdd-147">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fabdd-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fabdd-148">JSON representation</span></span>
<span data-ttu-id="fabdd-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fabdd-149">Here is a JSON representation of the resource</span></span>
<!--{
  "blockType":"resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedInsight"
}-->
```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
