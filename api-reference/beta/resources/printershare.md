---
title: Тип ресурса Принтершаре
description: Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 26715bb8eed9c671b88951bd1deb875f1d11d467
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917574"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="386f8-103">Тип ресурса Принтершаре</span><span class="sxs-lookup"><span data-stu-id="386f8-103">printerShare resource type</span></span>

<span data-ttu-id="386f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="386f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="386f8-105">Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.</span><span class="sxs-lookup"><span data-stu-id="386f8-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="386f8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="386f8-106">Methods</span></span>

| <span data-ttu-id="386f8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="386f8-107">Method</span></span>       | <span data-ttu-id="386f8-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="386f8-108">Return Type</span></span> | <span data-ttu-id="386f8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="386f8-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="386f8-110">List</span><span class="sxs-lookup"><span data-stu-id="386f8-110">List</span></span>](../api/print-list-printershares.md) | <span data-ttu-id="386f8-111">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="386f8-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="386f8-112">Получение списка общих принтеров в клиенте.</span><span class="sxs-lookup"><span data-stu-id="386f8-112">Get a list of printer shares in the tenant.</span></span> |
| <span data-ttu-id="386f8-113">[получение](../api/printershare-get.md);</span><span class="sxs-lookup"><span data-stu-id="386f8-113">[Get](../api/printershare-get.md)</span></span> | [<span data-ttu-id="386f8-114">принтершаре</span><span class="sxs-lookup"><span data-stu-id="386f8-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="386f8-115">Чтение свойств и связей объекта **принтершаре** .</span><span class="sxs-lookup"><span data-stu-id="386f8-115">Read properties and relationships of a **printerShare** object.</span></span> |
| <span data-ttu-id="386f8-116">[обновление](../api/printershare-update.md).</span><span class="sxs-lookup"><span data-stu-id="386f8-116">[Update](../api/printershare-update.md)</span></span> | [<span data-ttu-id="386f8-117">принтершаре</span><span class="sxs-lookup"><span data-stu-id="386f8-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="386f8-118">Обновление объекта **принтершаре** .</span><span class="sxs-lookup"><span data-stu-id="386f8-118">Update a **printerShare** object.</span></span> |
| <span data-ttu-id="386f8-119">[удаление](../api/printershare-delete.md);</span><span class="sxs-lookup"><span data-stu-id="386f8-119">[Delete](../api/printershare-delete.md)</span></span> | <span data-ttu-id="386f8-120">Нет</span><span class="sxs-lookup"><span data-stu-id="386f8-120">None</span></span> | <span data-ttu-id="386f8-121">Отменяет общий доступ к принтеру.</span><span class="sxs-lookup"><span data-stu-id="386f8-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="386f8-122">Список allowedUsers</span><span class="sxs-lookup"><span data-stu-id="386f8-122">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="386f8-123">Коллекция [принтусеридентити](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="386f8-123">[printUserIdentity](printuseridentity.md) collection</span></span> | <span data-ttu-id="386f8-124">Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="386f8-124">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="386f8-125">Добавление allowedUser</span><span class="sxs-lookup"><span data-stu-id="386f8-125">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="386f8-126">Нет</span><span class="sxs-lookup"><span data-stu-id="386f8-126">None</span></span> | <span data-ttu-id="386f8-127">Предоставьте заданному пользователю доступ на отправку заданий печати в соответствующую общую папку принтера.</span><span class="sxs-lookup"><span data-stu-id="386f8-127">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="386f8-128">Удаление allowedUser</span><span class="sxs-lookup"><span data-stu-id="386f8-128">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="386f8-129">Нет</span><span class="sxs-lookup"><span data-stu-id="386f8-129">None</span></span> | <span data-ttu-id="386f8-130">Отозвать доступ к общему принтеру для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="386f8-130">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="386f8-131">Список allowedGroups</span><span class="sxs-lookup"><span data-stu-id="386f8-131">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="386f8-132">Коллекция [принтидентити](printidentity.md)</span><span class="sxs-lookup"><span data-stu-id="386f8-132">[printIdentity](printidentity.md) collection</span></span> | <span data-ttu-id="386f8-133">Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="386f8-133">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="386f8-134">Добавление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="386f8-134">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="386f8-135">Нет</span><span class="sxs-lookup"><span data-stu-id="386f8-135">None</span></span> | <span data-ttu-id="386f8-136">Предоставление указанному групповому доступу на отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="386f8-136">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="386f8-137">Удаление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="386f8-137">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="386f8-138">Нет</span><span class="sxs-lookup"><span data-stu-id="386f8-138">None</span></span> | <span data-ttu-id="386f8-139">Отзыв доступа к общему принтеру из указанной группы.</span><span class="sxs-lookup"><span data-stu-id="386f8-139">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="386f8-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="386f8-140">Properties</span></span>
| <span data-ttu-id="386f8-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="386f8-141">Property</span></span>     | <span data-ttu-id="386f8-142">Тип</span><span class="sxs-lookup"><span data-stu-id="386f8-142">Type</span></span>        | <span data-ttu-id="386f8-143">Описание</span><span class="sxs-lookup"><span data-stu-id="386f8-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="386f8-144">id</span><span class="sxs-lookup"><span data-stu-id="386f8-144">id</span></span>|<span data-ttu-id="386f8-145">Строка</span><span class="sxs-lookup"><span data-stu-id="386f8-145">String</span></span>| <span data-ttu-id="386f8-146">Идентификатор Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="386f8-146">The printerShare's identifier.</span></span> <span data-ttu-id="386f8-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="386f8-147">Read-only.</span></span>|
|<span data-ttu-id="386f8-148">name</span><span class="sxs-lookup"><span data-stu-id="386f8-148">name</span></span>|<span data-ttu-id="386f8-149">String</span><span class="sxs-lookup"><span data-stu-id="386f8-149">String</span></span>|<span data-ttu-id="386f8-150">Имя общего принтера, который должен отображаться клиентами печати.</span><span class="sxs-lookup"><span data-stu-id="386f8-150">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="386f8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="386f8-151">createdDateTime</span></span>|<span data-ttu-id="386f8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="386f8-152">DateTimeOffset</span></span>|<span data-ttu-id="386f8-153">Значение DateTimeOffset при создании общего ресурса принтера.</span><span class="sxs-lookup"><span data-stu-id="386f8-153">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="386f8-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="386f8-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="386f8-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="386f8-155">Relationships</span></span>
| <span data-ttu-id="386f8-156">Связь</span><span class="sxs-lookup"><span data-stu-id="386f8-156">Relationship</span></span> | <span data-ttu-id="386f8-157">Тип</span><span class="sxs-lookup"><span data-stu-id="386f8-157">Type</span></span>        | <span data-ttu-id="386f8-158">Описание</span><span class="sxs-lookup"><span data-stu-id="386f8-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="386f8-159">Printer</span><span class="sxs-lookup"><span data-stu-id="386f8-159">printer</span></span>|[<span data-ttu-id="386f8-160">Printer</span><span class="sxs-lookup"><span data-stu-id="386f8-160">printer</span></span>](printer.md)|<span data-ttu-id="386f8-161">Принтер, с которым связан этот общий принтер.</span><span class="sxs-lookup"><span data-stu-id="386f8-161">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="386f8-162">алловедусерс</span><span class="sxs-lookup"><span data-stu-id="386f8-162">allowedUsers</span></span>|<span data-ttu-id="386f8-163">Коллекция [принтусеридентити](printuseridentity.md)</span><span class="sxs-lookup"><span data-stu-id="386f8-163">[printUserIdentity](printuseridentity.md) collection</span></span>|<span data-ttu-id="386f8-164">Пользователи, у которых есть доступ к печати с помощью принтера.</span><span class="sxs-lookup"><span data-stu-id="386f8-164">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="386f8-165">алловедграупс</span><span class="sxs-lookup"><span data-stu-id="386f8-165">allowedGroups</span></span>|[<span data-ttu-id="386f8-166">принтидентити</span><span class="sxs-lookup"><span data-stu-id="386f8-166">printIdentity</span></span>](printidentity.md)|<span data-ttu-id="386f8-167">Группы, у которых пользователи имеют доступ к печати с помощью принтера.</span><span class="sxs-lookup"><span data-stu-id="386f8-167">The groups whose users have access to print using the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="386f8-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="386f8-168">JSON representation</span></span>

<span data-ttu-id="386f8-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="386f8-169">The following is a JSON representation of the resource.</span></span>

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
