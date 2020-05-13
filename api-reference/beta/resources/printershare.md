---
title: Тип ресурса Принтершаре
description: Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5acbcdc58b730404a39af1f3069b3433fac54ed3
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217349"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="4a70f-103">Тип ресурса Принтершаре</span><span class="sxs-lookup"><span data-stu-id="4a70f-103">printerShare resource type</span></span>

<span data-ttu-id="4a70f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a70f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a70f-105">Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.</span><span class="sxs-lookup"><span data-stu-id="4a70f-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="4a70f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4a70f-106">Methods</span></span>

| <span data-ttu-id="4a70f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4a70f-107">Method</span></span>       | <span data-ttu-id="4a70f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4a70f-108">Return Type</span></span> | <span data-ttu-id="4a70f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4a70f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4a70f-110">Список</span><span class="sxs-lookup"><span data-stu-id="4a70f-110">List</span></span>](../api/print-list-shares.md) | <span data-ttu-id="4a70f-111">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="4a70f-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="4a70f-112">Получение списка общих принтеров в клиенте.</span><span class="sxs-lookup"><span data-stu-id="4a70f-112">Get a list of printer shares in the tenant.</span></span> |
| <span data-ttu-id="4a70f-113">[получение](../api/printershare-get.md);</span><span class="sxs-lookup"><span data-stu-id="4a70f-113">[Get](../api/printershare-get.md)</span></span> | [<span data-ttu-id="4a70f-114">принтершаре</span><span class="sxs-lookup"><span data-stu-id="4a70f-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="4a70f-115">Чтение свойств и связей объекта **принтершаре** .</span><span class="sxs-lookup"><span data-stu-id="4a70f-115">Read properties and relationships of a **printerShare** object.</span></span> |
| <span data-ttu-id="4a70f-116">[обновление](../api/printershare-update.md).</span><span class="sxs-lookup"><span data-stu-id="4a70f-116">[Update](../api/printershare-update.md)</span></span> | [<span data-ttu-id="4a70f-117">принтершаре</span><span class="sxs-lookup"><span data-stu-id="4a70f-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="4a70f-118">Обновление объекта **принтершаре** .</span><span class="sxs-lookup"><span data-stu-id="4a70f-118">Update a **printerShare** object.</span></span> |
| <span data-ttu-id="4a70f-119">[удаление](../api/printershare-delete.md);</span><span class="sxs-lookup"><span data-stu-id="4a70f-119">[Delete](../api/printershare-delete.md)</span></span> | <span data-ttu-id="4a70f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4a70f-120">None</span></span> | <span data-ttu-id="4a70f-121">Отменяет общий доступ к принтеру.</span><span class="sxs-lookup"><span data-stu-id="4a70f-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="4a70f-122">Список allowedUsers</span><span class="sxs-lookup"><span data-stu-id="4a70f-122">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="4a70f-123">Коллекция [принтусеридентити](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="4a70f-123">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="4a70f-124">Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="4a70f-124">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="4a70f-125">Добавление allowedUser</span><span class="sxs-lookup"><span data-stu-id="4a70f-125">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="4a70f-126">Нет</span><span class="sxs-lookup"><span data-stu-id="4a70f-126">None</span></span> | <span data-ttu-id="4a70f-127">Предоставьте заданному пользователю доступ на отправку заданий печати в соответствующую общую папку принтера.</span><span class="sxs-lookup"><span data-stu-id="4a70f-127">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="4a70f-128">Удаление allowedUser</span><span class="sxs-lookup"><span data-stu-id="4a70f-128">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="4a70f-129">Нет</span><span class="sxs-lookup"><span data-stu-id="4a70f-129">None</span></span> | <span data-ttu-id="4a70f-130">Отозвать доступ к общему принтеру для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4a70f-130">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="4a70f-131">Список allowedGroups</span><span class="sxs-lookup"><span data-stu-id="4a70f-131">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="4a70f-132">Коллекция [принтидентити](printidentity.md)</span><span class="sxs-lookup"><span data-stu-id="4a70f-132">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="4a70f-133">Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="4a70f-133">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="4a70f-134">Добавление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="4a70f-134">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="4a70f-135">Нет</span><span class="sxs-lookup"><span data-stu-id="4a70f-135">None</span></span> | <span data-ttu-id="4a70f-136">Предоставление указанному групповому доступу на отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="4a70f-136">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="4a70f-137">Удаление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="4a70f-137">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="4a70f-138">Нет</span><span class="sxs-lookup"><span data-stu-id="4a70f-138">None</span></span> | <span data-ttu-id="4a70f-139">Отзыв доступа к общему принтеру из указанной группы.</span><span class="sxs-lookup"><span data-stu-id="4a70f-139">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="4a70f-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a70f-140">Properties</span></span>
| <span data-ttu-id="4a70f-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a70f-141">Property</span></span>     | <span data-ttu-id="4a70f-142">Тип</span><span class="sxs-lookup"><span data-stu-id="4a70f-142">Type</span></span>        | <span data-ttu-id="4a70f-143">Описание</span><span class="sxs-lookup"><span data-stu-id="4a70f-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a70f-144">id</span><span class="sxs-lookup"><span data-stu-id="4a70f-144">id</span></span>|<span data-ttu-id="4a70f-145">String</span><span class="sxs-lookup"><span data-stu-id="4a70f-145">String</span></span>| <span data-ttu-id="4a70f-146">Идентификатор Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="4a70f-146">The printerShare's identifier.</span></span> <span data-ttu-id="4a70f-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a70f-147">Read-only.</span></span>|
|<span data-ttu-id="4a70f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="4a70f-148">displayName</span></span>|<span data-ttu-id="4a70f-149">Строка</span><span class="sxs-lookup"><span data-stu-id="4a70f-149">String</span></span>|<span data-ttu-id="4a70f-150">Имя общего принтера, который должен отображаться клиентами печати.</span><span class="sxs-lookup"><span data-stu-id="4a70f-150">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="4a70f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a70f-151">createdDateTime</span></span>|<span data-ttu-id="4a70f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a70f-152">DateTimeOffset</span></span>|<span data-ttu-id="4a70f-153">Значение DateTimeOffset при создании общего ресурса принтера.</span><span class="sxs-lookup"><span data-stu-id="4a70f-153">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="4a70f-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a70f-154">Read-only.</span></span>|
|<span data-ttu-id="4a70f-155">manufacturer</span><span class="sxs-lookup"><span data-stu-id="4a70f-155">manufacturer</span></span>|<span data-ttu-id="4a70f-156">String</span><span class="sxs-lookup"><span data-stu-id="4a70f-156">String</span></span>|<span data-ttu-id="4a70f-157">Производитель, сообщаемый принтером, связанным с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="4a70f-157">The manufacturer reported by the printer associated with this printer share.</span></span> <span data-ttu-id="4a70f-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a70f-158">Read-only.</span></span>|
|<span data-ttu-id="4a70f-159">model</span><span class="sxs-lookup"><span data-stu-id="4a70f-159">model</span></span>|<span data-ttu-id="4a70f-160">String</span><span class="sxs-lookup"><span data-stu-id="4a70f-160">String</span></span>|<span data-ttu-id="4a70f-161">Имя модели, сообщаемое принтером, связанным с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="4a70f-161">The model name reported by the printer associated with this printer share.</span></span> <span data-ttu-id="4a70f-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a70f-162">Read-only.</span></span>|
|<span data-ttu-id="4a70f-163">исакцептингжобс</span><span class="sxs-lookup"><span data-stu-id="4a70f-163">isAcceptingJobs</span></span>|<span data-ttu-id="4a70f-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a70f-164">Boolean</span></span>|<span data-ttu-id="4a70f-165">Принимает ли принтер, связанный с этим общим принтером, новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="4a70f-165">Whether the printer associated with this printer share is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="4a70f-166">по умолчанию</span><span class="sxs-lookup"><span data-stu-id="4a70f-166">defaults</span></span>|[<span data-ttu-id="4a70f-167">принтердефаултс</span><span class="sxs-lookup"><span data-stu-id="4a70f-167">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="4a70f-168">Параметры печати по умолчанию для принтера, связанного с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="4a70f-168">The default print settings of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="4a70f-169">capabilities</span><span class="sxs-lookup"><span data-stu-id="4a70f-169">capabilities</span></span>|[<span data-ttu-id="4a70f-170">принтеркапабилитиес</span><span class="sxs-lookup"><span data-stu-id="4a70f-170">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="4a70f-171">Возможности принтера, связанного с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="4a70f-171">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="4a70f-172">location</span><span class="sxs-lookup"><span data-stu-id="4a70f-172">location</span></span>|[<span data-ttu-id="4a70f-173">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="4a70f-173">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="4a70f-174">Физическое и/или организационное расположение принтера, связанного с общим ресурсом принтера.</span><span class="sxs-lookup"><span data-stu-id="4a70f-174">The physical and/or organizational location of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="4a70f-175">status</span><span class="sxs-lookup"><span data-stu-id="4a70f-175">status</span></span>|[<span data-ttu-id="4a70f-176">принтерстатус</span><span class="sxs-lookup"><span data-stu-id="4a70f-176">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="4a70f-177">Состояние обработки (включая ошибки) принтера, связанного с этим общим ресурсом принтера.</span><span class="sxs-lookup"><span data-stu-id="4a70f-177">The processing status, including any errors, of the printer associated with this printer share.</span></span> <span data-ttu-id="4a70f-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4a70f-178">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a70f-179">Отношения</span><span class="sxs-lookup"><span data-stu-id="4a70f-179">Relationships</span></span>
| <span data-ttu-id="4a70f-180">Связь</span><span class="sxs-lookup"><span data-stu-id="4a70f-180">Relationship</span></span> | <span data-ttu-id="4a70f-181">Тип</span><span class="sxs-lookup"><span data-stu-id="4a70f-181">Type</span></span>        | <span data-ttu-id="4a70f-182">Описание</span><span class="sxs-lookup"><span data-stu-id="4a70f-182">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a70f-183">Printer</span><span class="sxs-lookup"><span data-stu-id="4a70f-183">printer</span></span>|[<span data-ttu-id="4a70f-184">Printer</span><span class="sxs-lookup"><span data-stu-id="4a70f-184">printer</span></span>](printer.md)|<span data-ttu-id="4a70f-185">Принтер, с которым связан этот общий принтер.</span><span class="sxs-lookup"><span data-stu-id="4a70f-185">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="4a70f-186">алловедусерс</span><span class="sxs-lookup"><span data-stu-id="4a70f-186">allowedUsers</span></span>|<span data-ttu-id="4a70f-187">Коллекция [принтусеридентити](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="4a70f-187">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="4a70f-188">Пользователи, у которых есть доступ к печати с помощью принтера.</span><span class="sxs-lookup"><span data-stu-id="4a70f-188">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="4a70f-189">алловедграупс</span><span class="sxs-lookup"><span data-stu-id="4a70f-189">allowedGroups</span></span>|[<span data-ttu-id="4a70f-190">принтидентити</span><span class="sxs-lookup"><span data-stu-id="4a70f-190">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="4a70f-191">Группы, у которых пользователи имеют доступ к печати с помощью принтера.</span><span class="sxs-lookup"><span data-stu-id="4a70f-191">The groups whose users have access to print using the printer.</span></span>|
|<span data-ttu-id="4a70f-192">работе</span><span class="sxs-lookup"><span data-stu-id="4a70f-192">jobs</span></span>|<span data-ttu-id="4a70f-193">Коллекция [printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="4a70f-193">[printJob](printjob.md) collection</span></span>| <span data-ttu-id="4a70f-194">Список заданий, помещенных в очередь для печати принтером, связанным с этим общим принтером.</span><span class="sxs-lookup"><span data-stu-id="4a70f-194">The list of jobs that are queued for printing by the printer associated with this printer share.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a70f-195">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a70f-195">JSON representation</span></span>

<span data-ttu-id="4a70f-196">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a70f-196">The following is a JSON representation of the resource.</span></span>

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
