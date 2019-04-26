---
title: тип общего ресурса
description: 'Понимание файлов, к которым предоставлен общий доступ, или определенного пользователя. Поддерживаются следующие общие файлы:'
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 11a6989e0130e7eedca7fff6f6cc9790d8109d84
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549491"
---
# <a name="shared-resource-type"></a><span data-ttu-id="95c9e-104">тип общего ресурса</span><span class="sxs-lookup"><span data-stu-id="95c9e-104">shared resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95c9e-105">Понимание файлов, к которым предоставлен общий доступ, или определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="95c9e-105">An insight representing files shared with or by a specific user.</span></span> <span data-ttu-id="95c9e-106">Поддерживаются следующие общие файлы:</span><span class="sxs-lookup"><span data-stu-id="95c9e-106">The following shared files are supported:</span></span>

- <span data-ttu-id="95c9e-107">Файлы, вложенные непосредственно в сообщение электронной почты или приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="95c9e-107">Files attached directly in an email or a meeting invite.</span></span>
- <span data-ttu-id="95c9e-108">OneDrive для Буссинесс и современных вложений SharePoint — файлы, хранящиеся в OneDrive для бизнеса и SharePoint, которые пользователи совместно используют как ссылки в сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="95c9e-108">OneDrive for Bussiness and SharePoint modern attachments - files stored in OneDrive for Business and SharePoint that users share as a links in an email.</span></span>

<span data-ttu-id="95c9e-109">**Note**: в настоящее время мы работаем над заполнением результатов общего API с данными.</span><span class="sxs-lookup"><span data-stu-id="95c9e-109">**Note**: We are currently working on populating the results of the Shared API with data.</span></span> <span data-ttu-id="95c9e-110">Некоторые данные могут отсутствовать в первых неделях после выпуска.</span><span class="sxs-lookup"><span data-stu-id="95c9e-110">There may be some data missing in the first weeks after release.</span></span>

## <a name="methods"></a><span data-ttu-id="95c9e-111">Методы</span><span class="sxs-lookup"><span data-stu-id="95c9e-111">Methods</span></span>

| <span data-ttu-id="95c9e-112">Метод</span><span class="sxs-lookup"><span data-stu-id="95c9e-112">Method</span></span>       | <span data-ttu-id="95c9e-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="95c9e-113">Return Type</span></span>  |<span data-ttu-id="95c9e-114">Описание</span><span class="sxs-lookup"><span data-stu-id="95c9e-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95c9e-115">Список "Общие"</span><span class="sxs-lookup"><span data-stu-id="95c9e-115">List shared</span></span>](../api/insights-list-shared.md) |<span data-ttu-id="95c9e-116">Коллекция [инсигхтс_шаред](insights-shared.md)</span><span class="sxs-lookup"><span data-stu-id="95c9e-116">[insights_shared](insights-shared.md) collection</span></span>| <span data-ttu-id="95c9e-117">Получение списка общих файлов.</span><span class="sxs-lookup"><span data-stu-id="95c9e-117">Get a list of shared files.</span></span>|

## <a name="properties"></a><span data-ttu-id="95c9e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="95c9e-118">Properties</span></span>

| <span data-ttu-id="95c9e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="95c9e-119">Property</span></span>              | <span data-ttu-id="95c9e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="95c9e-120">Type</span></span>                      | <span data-ttu-id="95c9e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="95c9e-121">Description</span></span>  |
| -------------         |---------------            | -------------|
| <span data-ttu-id="95c9e-122">id</span><span class="sxs-lookup"><span data-stu-id="95c9e-122">id</span></span>                    | <span data-ttu-id="95c9e-123">String</span><span class="sxs-lookup"><span data-stu-id="95c9e-123">String</span></span>                    | <span data-ttu-id="95c9e-124">Уникальный идентификатор связи.</span><span class="sxs-lookup"><span data-stu-id="95c9e-124">Unique identifier of the relationship.</span></span> <span data-ttu-id="95c9e-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95c9e-125">Read only.</span></span>        |
| <span data-ttu-id="95c9e-126">Ластшаред</span><span class="sxs-lookup"><span data-stu-id="95c9e-126">lastShared</span></span>            | [<span data-ttu-id="95c9e-127">sharingDetail</span><span class="sxs-lookup"><span data-stu-id="95c9e-127">sharingDetail</span></span>](insights-sharingdetail.md)                | <span data-ttu-id="95c9e-128">Сведения об общем элементе.</span><span class="sxs-lookup"><span data-stu-id="95c9e-128">Details about the shared item.</span></span> <span data-ttu-id="95c9e-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95c9e-129">Read only.</span></span>        |
| <span data-ttu-id="95c9e-130">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="95c9e-130">resourceVisualization</span></span> | [<span data-ttu-id="95c9e-131">Ресурсе resourcevisualization</span><span class="sxs-lookup"><span data-stu-id="95c9e-131">resourceVisualization</span></span>](insights-resourcevisualization.md)                | <span data-ttu-id="95c9e-132">Свойства, которые можно использовать для отображения документа в вашем интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="95c9e-132">Properties that you can use to visualize the document in your experience.</span></span> <span data-ttu-id="95c9e-133">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="95c9e-133">Read-only</span></span>      |
| <span data-ttu-id="95c9e-134">Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="95c9e-134">resourceReference</span></span>     | [<span data-ttu-id="95c9e-135">Ресаурцереференце</span><span class="sxs-lookup"><span data-stu-id="95c9e-135">resourceReference</span></span>](insights-resourcereference.md)                      | <span data-ttu-id="95c9e-136">Справочные свойства общего документа, например URL-адрес и тип документа.</span><span class="sxs-lookup"><span data-stu-id="95c9e-136">Reference properties of the shared document, such as the url and type of the document.</span></span> <span data-ttu-id="95c9e-137">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="95c9e-137">Read-only</span></span>       |

## <a name="relationships"></a><span data-ttu-id="95c9e-138">Связи</span><span class="sxs-lookup"><span data-stu-id="95c9e-138">Relationships</span></span>

| <span data-ttu-id="95c9e-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="95c9e-139">Property</span></span>      | <span data-ttu-id="95c9e-140">Тип</span><span class="sxs-lookup"><span data-stu-id="95c9e-140">Type</span></span>          | <span data-ttu-id="95c9e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="95c9e-141">Description</span></span>  |
| ------------- |---------------| -------------|
| <span data-ttu-id="95c9e-142">resource</span><span class="sxs-lookup"><span data-stu-id="95c9e-142">resource</span></span>      | <span data-ttu-id="95c9e-143">Объект</span><span class="sxs-lookup"><span data-stu-id="95c9e-143">Entity</span></span>        | <span data-ttu-id="95c9e-144">Используется для перехода к элементу, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="95c9e-144">Used for navigating to the item that was shared.</span></span> <span data-ttu-id="95c9e-145">Для вложений в файл используется тип *fileAttachment*.</span><span class="sxs-lookup"><span data-stu-id="95c9e-145">For file attachments, the type is *fileAttachment*.</span></span> <span data-ttu-id="95c9e-146">Для связанных вложений используется тип *driveItem*.</span><span class="sxs-lookup"><span data-stu-id="95c9e-146">For linked attachments, the type is *driveItem*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="95c9e-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95c9e-147">JSON representation</span></span>
<span data-ttu-id="95c9e-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95c9e-148">Here is a JSON representation of the resource</span></span>

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
