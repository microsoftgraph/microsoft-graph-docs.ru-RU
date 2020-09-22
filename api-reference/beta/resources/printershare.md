---
title: Тип ресурса Принтершаре
description: Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 90f69ca6db0a84c0025caf4fff0ae07324703380
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048770"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="b2d1e-103">Тип ресурса Принтершаре</span><span class="sxs-lookup"><span data-stu-id="b2d1e-103">printerShare resource type</span></span>

<span data-ttu-id="b2d1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2d1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2d1e-105">Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="b2d1e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b2d1e-106">Methods</span></span>

| <span data-ttu-id="b2d1e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b2d1e-107">Method</span></span>       | <span data-ttu-id="b2d1e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b2d1e-108">Return Type</span></span> | <span data-ttu-id="b2d1e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b2d1e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b2d1e-110">Перечисление</span><span class="sxs-lookup"><span data-stu-id="b2d1e-110">List</span></span>](../api/print-list-shares.md) | <span data-ttu-id="b2d1e-111">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="b2d1e-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="b2d1e-112">Получение списка общих принтеров в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="b2d1e-113">Получение</span><span class="sxs-lookup"><span data-stu-id="b2d1e-113">Get</span></span>](../api/printershare-get.md) | [<span data-ttu-id="b2d1e-114">принтершаре</span><span class="sxs-lookup"><span data-stu-id="b2d1e-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="b2d1e-115">Чтение свойств и связей объекта **принтершаре** .</span><span class="sxs-lookup"><span data-stu-id="b2d1e-115">Read properties and relationships of a **printerShare** object.</span></span> |
| [<span data-ttu-id="b2d1e-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="b2d1e-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="b2d1e-117">принтершаре</span><span class="sxs-lookup"><span data-stu-id="b2d1e-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="b2d1e-118">Обновление объекта **принтершаре** .</span><span class="sxs-lookup"><span data-stu-id="b2d1e-118">Update a **printerShare** object.</span></span> |
| [<span data-ttu-id="b2d1e-119">Удаление</span><span class="sxs-lookup"><span data-stu-id="b2d1e-119">Delete</span></span>](../api/printershare-delete.md) | <span data-ttu-id="b2d1e-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b2d1e-120">None</span></span> | <span data-ttu-id="b2d1e-121">Отменяет общий доступ к принтеру.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="b2d1e-122">Список allowedUsers</span><span class="sxs-lookup"><span data-stu-id="b2d1e-122">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="b2d1e-123">Коллекция [принтусеридентити](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="b2d1e-123">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="b2d1e-124">Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-124">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="b2d1e-125">Добавление allowedUser</span><span class="sxs-lookup"><span data-stu-id="b2d1e-125">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="b2d1e-126">Нет</span><span class="sxs-lookup"><span data-stu-id="b2d1e-126">None</span></span> | <span data-ttu-id="b2d1e-127">Предоставьте заданному пользователю доступ на отправку заданий печати в соответствующую общую папку принтера.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-127">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="b2d1e-128">Удаление allowedUser</span><span class="sxs-lookup"><span data-stu-id="b2d1e-128">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="b2d1e-129">Нет</span><span class="sxs-lookup"><span data-stu-id="b2d1e-129">None</span></span> | <span data-ttu-id="b2d1e-130">Отозвать доступ к общему принтеру для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-130">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="b2d1e-131">Список allowedGroups</span><span class="sxs-lookup"><span data-stu-id="b2d1e-131">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="b2d1e-132">Коллекция [принтидентити](printidentity.md)</span><span class="sxs-lookup"><span data-stu-id="b2d1e-132">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="b2d1e-133">Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-133">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="b2d1e-134">Добавление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="b2d1e-134">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="b2d1e-135">Нет</span><span class="sxs-lookup"><span data-stu-id="b2d1e-135">None</span></span> | <span data-ttu-id="b2d1e-136">Предоставление указанному групповому доступу на отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-136">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="b2d1e-137">Удаление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="b2d1e-137">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="b2d1e-138">Нет</span><span class="sxs-lookup"><span data-stu-id="b2d1e-138">None</span></span> | <span data-ttu-id="b2d1e-139">Отзыв доступа к общему принтеру из указанной группы.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-139">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="b2d1e-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2d1e-140">Properties</span></span>
| <span data-ttu-id="b2d1e-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2d1e-141">Property</span></span>     | <span data-ttu-id="b2d1e-142">Тип</span><span class="sxs-lookup"><span data-stu-id="b2d1e-142">Type</span></span>        | <span data-ttu-id="b2d1e-143">Описание</span><span class="sxs-lookup"><span data-stu-id="b2d1e-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b2d1e-144">id</span><span class="sxs-lookup"><span data-stu-id="b2d1e-144">id</span></span>|<span data-ttu-id="b2d1e-145">Строка</span><span class="sxs-lookup"><span data-stu-id="b2d1e-145">String</span></span>| <span data-ttu-id="b2d1e-146">Идентификатор Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-146">The printerShare's identifier.</span></span> <span data-ttu-id="b2d1e-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-147">Read-only.</span></span>|
|<span data-ttu-id="b2d1e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="b2d1e-148">displayName</span></span>|<span data-ttu-id="b2d1e-149">Строка</span><span class="sxs-lookup"><span data-stu-id="b2d1e-149">String</span></span>|<span data-ttu-id="b2d1e-150">Имя общего принтера, который должен отображаться клиентами печати.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-150">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="b2d1e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2d1e-151">createdDateTime</span></span>|<span data-ttu-id="b2d1e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2d1e-152">DateTimeOffset</span></span>|<span data-ttu-id="b2d1e-153">Значение DateTimeOffset при создании общего ресурса принтера.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-153">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="b2d1e-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-154">Read-only.</span></span>|
|<span data-ttu-id="b2d1e-155">manufacturer</span><span class="sxs-lookup"><span data-stu-id="b2d1e-155">manufacturer</span></span>|<span data-ttu-id="b2d1e-156">String</span><span class="sxs-lookup"><span data-stu-id="b2d1e-156">String</span></span>|<span data-ttu-id="b2d1e-157">Производитель, сообщаемый принтером, связанным с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-157">The manufacturer reported by the printer associated with this printer share.</span></span> <span data-ttu-id="b2d1e-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-158">Read-only.</span></span>|
|<span data-ttu-id="b2d1e-159">model</span><span class="sxs-lookup"><span data-stu-id="b2d1e-159">model</span></span>|<span data-ttu-id="b2d1e-160">String</span><span class="sxs-lookup"><span data-stu-id="b2d1e-160">String</span></span>|<span data-ttu-id="b2d1e-161">Имя модели, сообщаемое принтером, связанным с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-161">The model name reported by the printer associated with this printer share.</span></span> <span data-ttu-id="b2d1e-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-162">Read-only.</span></span>|
|<span data-ttu-id="b2d1e-163">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="b2d1e-163">isAcceptingJobs</span></span>|<span data-ttu-id="b2d1e-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2d1e-164">Boolean</span></span>|<span data-ttu-id="b2d1e-165">Принимает ли принтер, связанный с этим общим принтером, новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-165">Whether the printer associated with this printer share is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="b2d1e-166">defaults</span><span class="sxs-lookup"><span data-stu-id="b2d1e-166">defaults</span></span>|[<span data-ttu-id="b2d1e-167">принтердефаултс</span><span class="sxs-lookup"><span data-stu-id="b2d1e-167">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="b2d1e-168">Параметры печати по умолчанию для принтера, связанного с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-168">The default print settings of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="b2d1e-169">capabilities</span><span class="sxs-lookup"><span data-stu-id="b2d1e-169">capabilities</span></span>|[<span data-ttu-id="b2d1e-170">принтеркапабилитиес</span><span class="sxs-lookup"><span data-stu-id="b2d1e-170">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="b2d1e-171">Возможности принтера, связанного с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-171">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="b2d1e-172">location</span><span class="sxs-lookup"><span data-stu-id="b2d1e-172">location</span></span>|[<span data-ttu-id="b2d1e-173">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="b2d1e-173">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="b2d1e-174">Физическое и/или организационное расположение принтера, связанного с общим ресурсом принтера.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-174">The physical and/or organizational location of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="b2d1e-175">status</span><span class="sxs-lookup"><span data-stu-id="b2d1e-175">status</span></span>|[<span data-ttu-id="b2d1e-176">принтерстатус</span><span class="sxs-lookup"><span data-stu-id="b2d1e-176">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="b2d1e-177">Состояние обработки (включая ошибки) принтера, связанного с этим общим ресурсом принтера.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-177">The processing status, including any errors, of the printer associated with this printer share.</span></span> <span data-ttu-id="b2d1e-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-178">Read-only.</span></span>|
|<span data-ttu-id="b2d1e-179">алловаллусерс</span><span class="sxs-lookup"><span data-stu-id="b2d1e-179">allowAllUsers</span></span>|<span data-ttu-id="b2d1e-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2d1e-180">Boolean</span></span>|<span data-ttu-id="b2d1e-181">Если этот параметр имеет значение true, всем пользователям и группам будет предоставлен доступ к этому общему ресурсу принтера.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-181">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="b2d1e-182">Этот параметр заменяет списки разрешений, определенные свойствами навигации **алловедусерс** и **алловедграупс** .</span><span class="sxs-lookup"><span data-stu-id="b2d1e-182">This supersedes the allow lists defined by the **allowedUsers** and **allowedGroups** navigation properties.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2d1e-183">Связи</span><span class="sxs-lookup"><span data-stu-id="b2d1e-183">Relationships</span></span>
| <span data-ttu-id="b2d1e-184">Связь</span><span class="sxs-lookup"><span data-stu-id="b2d1e-184">Relationship</span></span> | <span data-ttu-id="b2d1e-185">Тип</span><span class="sxs-lookup"><span data-stu-id="b2d1e-185">Type</span></span>        | <span data-ttu-id="b2d1e-186">Описание</span><span class="sxs-lookup"><span data-stu-id="b2d1e-186">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b2d1e-187">Printer</span><span class="sxs-lookup"><span data-stu-id="b2d1e-187">printer</span></span>|[<span data-ttu-id="b2d1e-188">Printer</span><span class="sxs-lookup"><span data-stu-id="b2d1e-188">printer</span></span>](printer.md)|<span data-ttu-id="b2d1e-189">Принтер, с которым связан этот общий принтер.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-189">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="b2d1e-190">алловедусерс</span><span class="sxs-lookup"><span data-stu-id="b2d1e-190">allowedUsers</span></span>|<span data-ttu-id="b2d1e-191">Коллекция [принтусеридентити](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="b2d1e-191">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="b2d1e-192">Пользователи, у которых есть доступ к печати с помощью принтера.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-192">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="b2d1e-193">алловедграупс</span><span class="sxs-lookup"><span data-stu-id="b2d1e-193">allowedGroups</span></span>|[<span data-ttu-id="b2d1e-194">принтидентити</span><span class="sxs-lookup"><span data-stu-id="b2d1e-194">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="b2d1e-195">Группы, у которых пользователи имеют доступ к печати с помощью принтера.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-195">The groups whose users have access to print using the printer.</span></span>|
|<span data-ttu-id="b2d1e-196">jobs</span><span class="sxs-lookup"><span data-stu-id="b2d1e-196">jobs</span></span>|<span data-ttu-id="b2d1e-197">Коллекция [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="b2d1e-197">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="b2d1e-198">Список заданий, помещенных в очередь для печати принтером, связанным с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-198">The list of jobs that are queued for printing by the printer associated with this printer share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2d1e-199">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2d1e-199">JSON representation</span></span>

<span data-ttu-id="b2d1e-200">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2d1e-200">The following is a JSON representation of the resource.</span></span>

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
  "name": "String",
  "createdDateTime": "String (timestamp)"
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


