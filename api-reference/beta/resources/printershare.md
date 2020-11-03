---
title: Тип ресурса Принтершаре
description: Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4fc729a41105340cc4066ee238c8d1ace3490765
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848233"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="a1b19-103">Тип ресурса Принтершаре</span><span class="sxs-lookup"><span data-stu-id="a1b19-103">printerShare resource type</span></span>

<span data-ttu-id="a1b19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1b19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1b19-105">Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.</span><span class="sxs-lookup"><span data-stu-id="a1b19-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="a1b19-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a1b19-106">Methods</span></span>

| <span data-ttu-id="a1b19-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a1b19-107">Method</span></span>       | <span data-ttu-id="a1b19-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a1b19-108">Return Type</span></span> | <span data-ttu-id="a1b19-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a1b19-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a1b19-110">Список</span><span class="sxs-lookup"><span data-stu-id="a1b19-110">List</span></span>](../api/print-list-shares.md) | <span data-ttu-id="a1b19-111">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="a1b19-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="a1b19-112">Получение списка общих принтеров в клиенте.</span><span class="sxs-lookup"><span data-stu-id="a1b19-112">Get a list of printer shares in the tenant.</span></span> |
| <span data-ttu-id="a1b19-113">[получение](../api/printershare-get.md);</span><span class="sxs-lookup"><span data-stu-id="a1b19-113">[Get](../api/printershare-get.md)</span></span> | [<span data-ttu-id="a1b19-114">принтершаре</span><span class="sxs-lookup"><span data-stu-id="a1b19-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="a1b19-115">Чтение свойств и связей объекта **принтершаре** .</span><span class="sxs-lookup"><span data-stu-id="a1b19-115">Read properties and relationships of a **printerShare** object.</span></span> |
| <span data-ttu-id="a1b19-116">[обновление](../api/printershare-update.md).</span><span class="sxs-lookup"><span data-stu-id="a1b19-116">[Update](../api/printershare-update.md)</span></span> | [<span data-ttu-id="a1b19-117">принтершаре</span><span class="sxs-lookup"><span data-stu-id="a1b19-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="a1b19-118">Обновление объекта **принтершаре** .</span><span class="sxs-lookup"><span data-stu-id="a1b19-118">Update a **printerShare** object.</span></span> |
| <span data-ttu-id="a1b19-119">[удаление](../api/printershare-delete.md);</span><span class="sxs-lookup"><span data-stu-id="a1b19-119">[Delete](../api/printershare-delete.md)</span></span> | <span data-ttu-id="a1b19-120">Нет</span><span class="sxs-lookup"><span data-stu-id="a1b19-120">None</span></span> | <span data-ttu-id="a1b19-121">Отменяет общий доступ к принтеру.</span><span class="sxs-lookup"><span data-stu-id="a1b19-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="a1b19-122">Список заданий</span><span class="sxs-lookup"><span data-stu-id="a1b19-122">List jobs</span></span>](../api/printershare-list-jobs.md) | <span data-ttu-id="a1b19-123">Коллекция [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="a1b19-123">[printJob](printjob.md) collection</span></span> | <span data-ttu-id="a1b19-124">Получение списка заданий печати, помещенных в очередь для обработки с помощью Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="a1b19-124">Get a list of print jobs that are queued for processing by the printerShare.</span></span> |
| [<span data-ttu-id="a1b19-125">Создание задания</span><span class="sxs-lookup"><span data-stu-id="a1b19-125">Create job</span></span>](../api/printershare-post-jobs.md) | [<span data-ttu-id="a1b19-126">printJob</span><span class="sxs-lookup"><span data-stu-id="a1b19-126">printJob</span></span>](printjob.md) | <span data-ttu-id="a1b19-127">Создайте новое задание печати для Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="a1b19-127">Create a new print job for the printerShare.</span></span> <span data-ttu-id="a1b19-128">Чтобы начать печать задания, используйте [Start](../api/printjob-start.md).</span><span class="sxs-lookup"><span data-stu-id="a1b19-128">To start printing the job, use [start](../api/printjob-start.md).</span></span> |
| [<span data-ttu-id="a1b19-129">Список allowedUsers</span><span class="sxs-lookup"><span data-stu-id="a1b19-129">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="a1b19-130">Коллекция [принтусеридентити](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="a1b19-130">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="a1b19-131">Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="a1b19-131">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="a1b19-132">Добавление allowedUser</span><span class="sxs-lookup"><span data-stu-id="a1b19-132">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="a1b19-133">Нет</span><span class="sxs-lookup"><span data-stu-id="a1b19-133">None</span></span> | <span data-ttu-id="a1b19-134">Предоставьте заданному пользователю доступ на отправку заданий печати в соответствующую общую папку принтера.</span><span class="sxs-lookup"><span data-stu-id="a1b19-134">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="a1b19-135">Удаление allowedUser</span><span class="sxs-lookup"><span data-stu-id="a1b19-135">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="a1b19-136">Нет</span><span class="sxs-lookup"><span data-stu-id="a1b19-136">None</span></span> | <span data-ttu-id="a1b19-137">Отозвать доступ к общему принтеру для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a1b19-137">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="a1b19-138">Список allowedGroups</span><span class="sxs-lookup"><span data-stu-id="a1b19-138">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="a1b19-139">Коллекция [принтидентити](printidentity.md)</span><span class="sxs-lookup"><span data-stu-id="a1b19-139">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="a1b19-140">Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="a1b19-140">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="a1b19-141">Добавление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="a1b19-141">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="a1b19-142">Нет</span><span class="sxs-lookup"><span data-stu-id="a1b19-142">None</span></span> | <span data-ttu-id="a1b19-143">Предоставление указанному групповому доступу на отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="a1b19-143">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="a1b19-144">Удаление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="a1b19-144">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="a1b19-145">Нет</span><span class="sxs-lookup"><span data-stu-id="a1b19-145">None</span></span> | <span data-ttu-id="a1b19-146">Отзыв доступа к общему принтеру из указанной группы.</span><span class="sxs-lookup"><span data-stu-id="a1b19-146">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="a1b19-147">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1b19-147">Properties</span></span>
| <span data-ttu-id="a1b19-148">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1b19-148">Property</span></span>     | <span data-ttu-id="a1b19-149">Тип</span><span class="sxs-lookup"><span data-stu-id="a1b19-149">Type</span></span>        | <span data-ttu-id="a1b19-150">Описание</span><span class="sxs-lookup"><span data-stu-id="a1b19-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a1b19-151">id</span><span class="sxs-lookup"><span data-stu-id="a1b19-151">id</span></span>|<span data-ttu-id="a1b19-152">String</span><span class="sxs-lookup"><span data-stu-id="a1b19-152">String</span></span>| <span data-ttu-id="a1b19-153">Идентификатор Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="a1b19-153">The printerShare's identifier.</span></span> <span data-ttu-id="a1b19-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1b19-154">Read-only.</span></span>|
|<span data-ttu-id="a1b19-155">displayName</span><span class="sxs-lookup"><span data-stu-id="a1b19-155">displayName</span></span>|<span data-ttu-id="a1b19-156">String</span><span class="sxs-lookup"><span data-stu-id="a1b19-156">String</span></span>|<span data-ttu-id="a1b19-157">Имя общего принтера, который должен отображаться клиентами печати.</span><span class="sxs-lookup"><span data-stu-id="a1b19-157">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="a1b19-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1b19-158">createdDateTime</span></span>|<span data-ttu-id="a1b19-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1b19-159">DateTimeOffset</span></span>|<span data-ttu-id="a1b19-160">Значение DateTimeOffset при создании общего ресурса принтера.</span><span class="sxs-lookup"><span data-stu-id="a1b19-160">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="a1b19-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1b19-161">Read-only.</span></span>|
|<span data-ttu-id="a1b19-162">manufacturer</span><span class="sxs-lookup"><span data-stu-id="a1b19-162">manufacturer</span></span>|<span data-ttu-id="a1b19-163">String</span><span class="sxs-lookup"><span data-stu-id="a1b19-163">String</span></span>|<span data-ttu-id="a1b19-164">Производитель, сообщаемый принтером, связанным с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="a1b19-164">The manufacturer reported by the printer associated with this printer share.</span></span> <span data-ttu-id="a1b19-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1b19-165">Read-only.</span></span>|
|<span data-ttu-id="a1b19-166">model</span><span class="sxs-lookup"><span data-stu-id="a1b19-166">model</span></span>|<span data-ttu-id="a1b19-167">String</span><span class="sxs-lookup"><span data-stu-id="a1b19-167">String</span></span>|<span data-ttu-id="a1b19-168">Имя модели, сообщаемое принтером, связанным с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="a1b19-168">The model name reported by the printer associated with this printer share.</span></span> <span data-ttu-id="a1b19-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1b19-169">Read-only.</span></span>|
|<span data-ttu-id="a1b19-170">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="a1b19-170">isAcceptingJobs</span></span>|<span data-ttu-id="a1b19-171">Логический</span><span class="sxs-lookup"><span data-stu-id="a1b19-171">Boolean</span></span>|<span data-ttu-id="a1b19-172">Принимает ли принтер, связанный с этим общим принтером, новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="a1b19-172">Whether the printer associated with this printer share is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="a1b19-173">defaults</span><span class="sxs-lookup"><span data-stu-id="a1b19-173">defaults</span></span>|[<span data-ttu-id="a1b19-174">принтердефаултс</span><span class="sxs-lookup"><span data-stu-id="a1b19-174">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="a1b19-175">Параметры печати по умолчанию для принтера, связанного с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="a1b19-175">The default print settings of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="a1b19-176">capabilities</span><span class="sxs-lookup"><span data-stu-id="a1b19-176">capabilities</span></span>|[<span data-ttu-id="a1b19-177">принтеркапабилитиес</span><span class="sxs-lookup"><span data-stu-id="a1b19-177">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="a1b19-178">Возможности принтера, связанного с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="a1b19-178">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="a1b19-179">location</span><span class="sxs-lookup"><span data-stu-id="a1b19-179">location</span></span>|[<span data-ttu-id="a1b19-180">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="a1b19-180">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="a1b19-181">Физическое и/или организационное расположение принтера, связанного с общим ресурсом принтера.</span><span class="sxs-lookup"><span data-stu-id="a1b19-181">The physical and/or organizational location of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="a1b19-182">status</span><span class="sxs-lookup"><span data-stu-id="a1b19-182">status</span></span>|[<span data-ttu-id="a1b19-183">принтерстатус</span><span class="sxs-lookup"><span data-stu-id="a1b19-183">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="a1b19-184">Состояние обработки (включая ошибки) принтера, связанного с этим общим ресурсом принтера.</span><span class="sxs-lookup"><span data-stu-id="a1b19-184">The processing status, including any errors, of the printer associated with this printer share.</span></span> <span data-ttu-id="a1b19-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1b19-185">Read-only.</span></span>|
|<span data-ttu-id="a1b19-186">алловаллусерс</span><span class="sxs-lookup"><span data-stu-id="a1b19-186">allowAllUsers</span></span>|<span data-ttu-id="a1b19-187">Логический</span><span class="sxs-lookup"><span data-stu-id="a1b19-187">Boolean</span></span>|<span data-ttu-id="a1b19-188">Если этот параметр имеет значение true, всем пользователям и группам будет предоставлен доступ к этому общему ресурсу принтера.</span><span class="sxs-lookup"><span data-stu-id="a1b19-188">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="a1b19-189">Этот параметр заменяет списки разрешений, определенные свойствами навигации **алловедусерс** и **алловедграупс** .</span><span class="sxs-lookup"><span data-stu-id="a1b19-189">This supersedes the allow lists defined by the **allowedUsers** and **allowedGroups** navigation properties.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1b19-190">Связи</span><span class="sxs-lookup"><span data-stu-id="a1b19-190">Relationships</span></span>
| <span data-ttu-id="a1b19-191">Связь</span><span class="sxs-lookup"><span data-stu-id="a1b19-191">Relationship</span></span> | <span data-ttu-id="a1b19-192">Тип</span><span class="sxs-lookup"><span data-stu-id="a1b19-192">Type</span></span>        | <span data-ttu-id="a1b19-193">Описание</span><span class="sxs-lookup"><span data-stu-id="a1b19-193">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a1b19-194">Printer</span><span class="sxs-lookup"><span data-stu-id="a1b19-194">printer</span></span>|[<span data-ttu-id="a1b19-195">Printer</span><span class="sxs-lookup"><span data-stu-id="a1b19-195">printer</span></span>](printer.md)|<span data-ttu-id="a1b19-196">Принтер, с которым связан этот общий принтер.</span><span class="sxs-lookup"><span data-stu-id="a1b19-196">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="a1b19-197">алловедусерс</span><span class="sxs-lookup"><span data-stu-id="a1b19-197">allowedUsers</span></span>|<span data-ttu-id="a1b19-198">Коллекция [принтусеридентити](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="a1b19-198">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="a1b19-199">Пользователи, у которых есть доступ к печати с помощью принтера.</span><span class="sxs-lookup"><span data-stu-id="a1b19-199">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="a1b19-200">алловедграупс</span><span class="sxs-lookup"><span data-stu-id="a1b19-200">allowedGroups</span></span>|[<span data-ttu-id="a1b19-201">принтидентити</span><span class="sxs-lookup"><span data-stu-id="a1b19-201">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="a1b19-202">Группы, у которых пользователи имеют доступ к печати с помощью принтера.</span><span class="sxs-lookup"><span data-stu-id="a1b19-202">The groups whose users have access to print using the printer.</span></span>|
|<span data-ttu-id="a1b19-203">jobs</span><span class="sxs-lookup"><span data-stu-id="a1b19-203">jobs</span></span>|<span data-ttu-id="a1b19-204">Коллекция [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="a1b19-204">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="a1b19-205">Список заданий, помещенных в очередь для печати принтером, связанным с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="a1b19-205">The list of jobs that are queued for printing by the printer associated with this printer share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1b19-206">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a1b19-206">JSON representation</span></span>

<span data-ttu-id="a1b19-207">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1b19-207">The following is a JSON representation of the resource.</span></span>

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


