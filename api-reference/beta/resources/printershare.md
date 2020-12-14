---
title: Тип ресурса printerShare
description: Представляет принтер, который должен быть обнаруживаемым пользователями и приложениями печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5f8b8ad8446d37c73ddfd2b55b8ca544f1f926cd
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49664081"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="9a047-103">Тип ресурса printerShare</span><span class="sxs-lookup"><span data-stu-id="9a047-103">printerShare resource type</span></span>

<span data-ttu-id="9a047-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a047-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a047-105">Представляет принтер, который должен быть обнаруживаемым пользователями и приложениями печати.</span><span class="sxs-lookup"><span data-stu-id="9a047-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="9a047-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9a047-106">Methods</span></span>

| <span data-ttu-id="9a047-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9a047-107">Method</span></span>       | <span data-ttu-id="9a047-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9a047-108">Return Type</span></span> | <span data-ttu-id="9a047-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9a047-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9a047-110">Список</span><span class="sxs-lookup"><span data-stu-id="9a047-110">List</span></span>](../api/print-list-shares.md) | <span data-ttu-id="9a047-111">[Коллекция printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="9a047-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="9a047-112">Получите список принтеров в клиенте.</span><span class="sxs-lookup"><span data-stu-id="9a047-112">Get a list of printer shares in the tenant.</span></span> |
| <span data-ttu-id="9a047-113">[получение](../api/printershare-get.md);</span><span class="sxs-lookup"><span data-stu-id="9a047-113">[Get](../api/printershare-get.md)</span></span> | [<span data-ttu-id="9a047-114">printerShare</span><span class="sxs-lookup"><span data-stu-id="9a047-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="9a047-115">Чтение свойств и связей объекта **printerShare.**</span><span class="sxs-lookup"><span data-stu-id="9a047-115">Read properties and relationships of a **printerShare** object.</span></span> |
| [<span data-ttu-id="9a047-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="9a047-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="9a047-117">printerShare</span><span class="sxs-lookup"><span data-stu-id="9a047-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="9a047-118">Обновление объекта **printerShare.**</span><span class="sxs-lookup"><span data-stu-id="9a047-118">Update a **printerShare** object.</span></span> |
| <span data-ttu-id="9a047-119">[удаление](../api/printershare-delete.md);</span><span class="sxs-lookup"><span data-stu-id="9a047-119">[Delete](../api/printershare-delete.md)</span></span> | <span data-ttu-id="9a047-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9a047-120">None</span></span> | <span data-ttu-id="9a047-121">Отобрьь принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="9a047-122">Список заданий</span><span class="sxs-lookup"><span data-stu-id="9a047-122">List jobs</span></span>](../api/printershare-list-jobs.md) | <span data-ttu-id="9a047-123">[Коллекция printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="9a047-123">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="9a047-124">Получите список заданий печати, которые находятся в очереди для обработки принтеромShare.</span><span class="sxs-lookup"><span data-stu-id="9a047-124">Get a list of print jobs that are queued for processing by the printerShare.</span></span> |
| [<span data-ttu-id="9a047-125">Создание задания</span><span class="sxs-lookup"><span data-stu-id="9a047-125">Create job</span></span>](../api/printershare-post-jobs.md) | [<span data-ttu-id="9a047-126">printJob</span><span class="sxs-lookup"><span data-stu-id="9a047-126">printJob</span></span>](printjob.md) | <span data-ttu-id="9a047-127">Создайте новое задание печати для printerShare.</span><span class="sxs-lookup"><span data-stu-id="9a047-127">Create a new print job for the printerShare.</span></span> <span data-ttu-id="9a047-128">Чтобы начать печать задания, [используйте](../api/printjob-start.md)start .</span><span class="sxs-lookup"><span data-stu-id="9a047-128">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="9a047-129">Список allowedUsers</span><span class="sxs-lookup"><span data-stu-id="9a047-129">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="9a047-130">Коллекция объектов [user](user.md)</span><span class="sxs-lookup"><span data-stu-id="9a047-130">[user](user.md) collection</span></span> | <span data-ttu-id="9a047-131">Получить список пользователей, которым предоставлен доступ для отправки заданий печати в связанную обойму принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-131">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="9a047-132">Добавление allowedUser</span><span class="sxs-lookup"><span data-stu-id="9a047-132">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="9a047-133">Нет</span><span class="sxs-lookup"><span data-stu-id="9a047-133">None</span></span> | <span data-ttu-id="9a047-134">Предодайте указанному пользователю доступ для отправки заданий печати в связанную обойму принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-134">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="9a047-135">Удаление allowedUser</span><span class="sxs-lookup"><span data-stu-id="9a047-135">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="9a047-136">Нет</span><span class="sxs-lookup"><span data-stu-id="9a047-136">None</span></span> | <span data-ttu-id="9a047-137">Отозовет доступ к принтеру для доступа к данным у указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9a047-137">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="9a047-138">Список allowedGroups</span><span class="sxs-lookup"><span data-stu-id="9a047-138">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="9a047-139">Коллекция [group](group.md)</span><span class="sxs-lookup"><span data-stu-id="9a047-139">[group](group.md) collection</span></span> | <span data-ttu-id="9a047-140">Получить список групп, которые получили доступ для отправки заданий печати в связанную обойму принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-140">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="9a047-141">Добавление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="9a047-141">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="9a047-142">Нет</span><span class="sxs-lookup"><span data-stu-id="9a047-142">None</span></span> | <span data-ttu-id="9a047-143">Предодайте указанной группе доступ для отправки заданий печати в связанную обную долю принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-143">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="9a047-144">Удаление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="9a047-144">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="9a047-145">Нет</span><span class="sxs-lookup"><span data-stu-id="9a047-145">None</span></span> | <span data-ttu-id="9a047-146">Отозовет доступ к принтеру для доступа к данным из указанной группы.</span><span class="sxs-lookup"><span data-stu-id="9a047-146">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="9a047-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a047-147">Properties</span></span>
| <span data-ttu-id="9a047-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a047-148">Property</span></span>     | <span data-ttu-id="9a047-149">Тип</span><span class="sxs-lookup"><span data-stu-id="9a047-149">Type</span></span>        | <span data-ttu-id="9a047-150">Описание</span><span class="sxs-lookup"><span data-stu-id="9a047-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a047-151">id</span><span class="sxs-lookup"><span data-stu-id="9a047-151">id</span></span>|<span data-ttu-id="9a047-152">String</span><span class="sxs-lookup"><span data-stu-id="9a047-152">String</span></span>| <span data-ttu-id="9a047-153">Идентификатор printerShare.</span><span class="sxs-lookup"><span data-stu-id="9a047-153">The printerShare's identifier.</span></span> <span data-ttu-id="9a047-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a047-154">Read-only.</span></span>|
|<span data-ttu-id="9a047-155">displayName</span><span class="sxs-lookup"><span data-stu-id="9a047-155">displayName</span></span>|<span data-ttu-id="9a047-156">String</span><span class="sxs-lookup"><span data-stu-id="9a047-156">String</span></span>|<span data-ttu-id="9a047-157">Имя обоймы принтера, которую должны отображать клиенты печати.</span><span class="sxs-lookup"><span data-stu-id="9a047-157">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="9a047-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a047-158">createdDateTime</span></span>|<span data-ttu-id="9a047-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a047-159">DateTimeOffset</span></span>|<span data-ttu-id="9a047-160">DateTimeOffset, когда была создана обойма принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-160">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="9a047-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a047-161">Read-only.</span></span>|
|<span data-ttu-id="9a047-162">manufacturer</span><span class="sxs-lookup"><span data-stu-id="9a047-162">manufacturer</span></span>|<span data-ttu-id="9a047-163">String</span><span class="sxs-lookup"><span data-stu-id="9a047-163">String</span></span>|<span data-ttu-id="9a047-164">Производитель, о чем сообщил принтер, связанный с этой обоймой принтером.</span><span class="sxs-lookup"><span data-stu-id="9a047-164">The manufacturer reported by the printer associated with this printer share.</span></span> <span data-ttu-id="9a047-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a047-165">Read-only.</span></span>|
|<span data-ttu-id="9a047-166">model</span><span class="sxs-lookup"><span data-stu-id="9a047-166">model</span></span>|<span data-ttu-id="9a047-167">String</span><span class="sxs-lookup"><span data-stu-id="9a047-167">String</span></span>|<span data-ttu-id="9a047-168">Имя модели, сообщаемая принтером, связанным с этой обоймой принтером.</span><span class="sxs-lookup"><span data-stu-id="9a047-168">The model name reported by the printer associated with this printer share.</span></span> <span data-ttu-id="9a047-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a047-169">Read-only.</span></span>|
|<span data-ttu-id="9a047-170">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="9a047-170">isAcceptingJobs</span></span>|<span data-ttu-id="9a047-171">Логический</span><span class="sxs-lookup"><span data-stu-id="9a047-171">Boolean</span></span>|<span data-ttu-id="9a047-172">Принимает ли принтер, связанный с этой обоймой принтера, в настоящее время принимает новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="9a047-172">Whether the printer associated with this printer share is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="9a047-173">defaults</span><span class="sxs-lookup"><span data-stu-id="9a047-173">defaults</span></span>|[<span data-ttu-id="9a047-174">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="9a047-174">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="9a047-175">Параметры печати по умолчанию для принтера, связанного с этой обоймой.</span><span class="sxs-lookup"><span data-stu-id="9a047-175">The default print settings of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="9a047-176">capabilities</span><span class="sxs-lookup"><span data-stu-id="9a047-176">capabilities</span></span>|[<span data-ttu-id="9a047-177">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="9a047-177">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="9a047-178">Возможности принтера, связанного с этой обойдной частью принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-178">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="9a047-179">расположение</span><span class="sxs-lookup"><span data-stu-id="9a047-179">location</span></span>|[<span data-ttu-id="9a047-180">printerLocation</span><span class="sxs-lookup"><span data-stu-id="9a047-180">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="9a047-181">Физическое и/или организационное расположение принтера, связанного с этой обоймой принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-181">The physical and/or organizational location of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="9a047-182">status</span><span class="sxs-lookup"><span data-stu-id="9a047-182">status</span></span>|[<span data-ttu-id="9a047-183">printerStatus</span><span class="sxs-lookup"><span data-stu-id="9a047-183">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="9a047-184">Состояние обработки, включая все ошибки, принтера, связанного с этой обоймой принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-184">The processing status, including any errors, of the printer associated with this printer share.</span></span> <span data-ttu-id="9a047-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a047-185">Read-only.</span></span>|
|<span data-ttu-id="9a047-186">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="9a047-186">allowAllUsers</span></span>|<span data-ttu-id="9a047-187">Логический</span><span class="sxs-lookup"><span data-stu-id="9a047-187">Boolean</span></span>|<span data-ttu-id="9a047-188">Если задана истина, всем пользователям и группам будет предоставлен доступ к этой обойме принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-188">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="9a047-189">Это замеает списки разрешенных, определенные свойствами **навигации allowedUsers** и **allowedGroups.**</span><span class="sxs-lookup"><span data-stu-id="9a047-189">This supersedes the allow lists defined by the **allowedUsers** and **allowedGroups** navigation properties.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a047-190">Связи</span><span class="sxs-lookup"><span data-stu-id="9a047-190">Relationships</span></span>
| <span data-ttu-id="9a047-191">Связь</span><span class="sxs-lookup"><span data-stu-id="9a047-191">Relationship</span></span> | <span data-ttu-id="9a047-192">Тип</span><span class="sxs-lookup"><span data-stu-id="9a047-192">Type</span></span>        | <span data-ttu-id="9a047-193">Описание</span><span class="sxs-lookup"><span data-stu-id="9a047-193">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a047-194">printer</span><span class="sxs-lookup"><span data-stu-id="9a047-194">printer</span></span>|[<span data-ttu-id="9a047-195">printer</span><span class="sxs-lookup"><span data-stu-id="9a047-195">printer</span></span>](printer.md)|<span data-ttu-id="9a047-196">Принтер, с который связан этот принтер.</span><span class="sxs-lookup"><span data-stu-id="9a047-196">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="9a047-197">allowedUsers</span><span class="sxs-lookup"><span data-stu-id="9a047-197">allowedUsers</span></span>|<span data-ttu-id="9a047-198">Коллекция объектов [user](user.md)</span><span class="sxs-lookup"><span data-stu-id="9a047-198">[user](user.md) collection</span></span>|<span data-ttu-id="9a047-199">Пользователи, у которых есть доступ к печати с помощью принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-199">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="9a047-200">allowedGroups</span><span class="sxs-lookup"><span data-stu-id="9a047-200">allowedGroups</span></span>|[<span data-ttu-id="9a047-201">group</span><span class="sxs-lookup"><span data-stu-id="9a047-201">group</span></span>](group.md)|<span data-ttu-id="9a047-202">Группы, пользователи которых имеют доступ к печати с помощью принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-202">The groups whose users have access to print using the printer.</span></span>|
|<span data-ttu-id="9a047-203">jobs</span><span class="sxs-lookup"><span data-stu-id="9a047-203">jobs</span></span>|<span data-ttu-id="9a047-204">[Коллекция printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="9a047-204">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="9a047-205">Список заданий, которые находятся в очереди для печати принтером, связанным с этой обоймой принтера.</span><span class="sxs-lookup"><span data-stu-id="9a047-205">The list of jobs that are queued for printing by the printer associated with this printer share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a047-206">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a047-206">JSON representation</span></span>

<span data-ttu-id="9a047-207">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a047-207">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "createdDateTime": "String (timestamp)",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"},
  "capabilities": {"@odata.type": "microsoft.graph.printerCapabilities"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


