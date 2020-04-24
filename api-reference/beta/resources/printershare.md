---
title: Тип ресурса Принтершаре
description: Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8aa9312bf8b7e8f9a2cec049b8275d4ce7a04012
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43806844"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="650ef-103">Тип ресурса Принтершаре</span><span class="sxs-lookup"><span data-stu-id="650ef-103">printerShare resource type</span></span>

<span data-ttu-id="650ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="650ef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="650ef-105">Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.</span><span class="sxs-lookup"><span data-stu-id="650ef-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="650ef-106">Методы</span><span class="sxs-lookup"><span data-stu-id="650ef-106">Methods</span></span>

| <span data-ttu-id="650ef-107">Метод</span><span class="sxs-lookup"><span data-stu-id="650ef-107">Method</span></span>       | <span data-ttu-id="650ef-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="650ef-108">Return Type</span></span> | <span data-ttu-id="650ef-109">Описание</span><span class="sxs-lookup"><span data-stu-id="650ef-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="650ef-110">List</span><span class="sxs-lookup"><span data-stu-id="650ef-110">List</span></span>](../api/print-list-printershares.md) | <span data-ttu-id="650ef-111">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="650ef-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="650ef-112">Получение списка общих принтеров в клиенте.</span><span class="sxs-lookup"><span data-stu-id="650ef-112">Get a list of printer shares in the tenant.</span></span> |
| <span data-ttu-id="650ef-113">[получение](../api/printershare-get.md);</span><span class="sxs-lookup"><span data-stu-id="650ef-113">[Get](../api/printershare-get.md)</span></span> | [<span data-ttu-id="650ef-114">принтершаре</span><span class="sxs-lookup"><span data-stu-id="650ef-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="650ef-115">Чтение свойств и связей объекта **принтершаре** .</span><span class="sxs-lookup"><span data-stu-id="650ef-115">Read properties and relationships of a **printerShare** object.</span></span> |
| [<span data-ttu-id="650ef-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="650ef-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="650ef-117">принтершаре</span><span class="sxs-lookup"><span data-stu-id="650ef-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="650ef-118">Обновление объекта **принтершаре** .</span><span class="sxs-lookup"><span data-stu-id="650ef-118">Update a **printerShare** object.</span></span> |
| <span data-ttu-id="650ef-119">[удаление](../api/printershare-delete.md);</span><span class="sxs-lookup"><span data-stu-id="650ef-119">[Delete](../api/printershare-delete.md)</span></span> | <span data-ttu-id="650ef-120">Нет</span><span class="sxs-lookup"><span data-stu-id="650ef-120">None</span></span> | <span data-ttu-id="650ef-121">Отменяет общий доступ к принтеру.</span><span class="sxs-lookup"><span data-stu-id="650ef-121">Unshare a printer.</span></span> |
| [<span data-ttu-id="650ef-122">Список allowedUsers</span><span class="sxs-lookup"><span data-stu-id="650ef-122">List allowedUsers</span></span>](../api/printershare-list-allowedusers.md) | <span data-ttu-id="650ef-123">Коллекция [userIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="650ef-123">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="650ef-124">Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="650ef-124">Retrieve a list of users who have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="650ef-125">Добавление allowedUser</span><span class="sxs-lookup"><span data-stu-id="650ef-125">Add allowedUser</span></span>](../api/printershare-post-allowedusers.md) | <span data-ttu-id="650ef-126">Нет</span><span class="sxs-lookup"><span data-stu-id="650ef-126">None</span></span> | <span data-ttu-id="650ef-127">Предоставьте заданному пользователю доступ на отправку заданий печати в соответствующую общую папку принтера.</span><span class="sxs-lookup"><span data-stu-id="650ef-127">Grant the specified user access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="650ef-128">Удаление allowedUser</span><span class="sxs-lookup"><span data-stu-id="650ef-128">Remove allowedUser</span></span>](../api/printershare-delete-alloweduser.md) | <span data-ttu-id="650ef-129">Нет</span><span class="sxs-lookup"><span data-stu-id="650ef-129">None</span></span> | <span data-ttu-id="650ef-130">Отозвать доступ к общему принтеру для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="650ef-130">Revoke printer share access from the specified user.</span></span> |
| [<span data-ttu-id="650ef-131">Список allowedGroups</span><span class="sxs-lookup"><span data-stu-id="650ef-131">List allowedGroups</span></span>](../api/printershare-list-allowedgroups.md) | <span data-ttu-id="650ef-132">Коллекция [удостоверений](identity.md)</span><span class="sxs-lookup"><span data-stu-id="650ef-132">[identity](identity.md) collection</span></span> | <span data-ttu-id="650ef-133">Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="650ef-133">Retrieve a list of groups that have been granted access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="650ef-134">Добавление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="650ef-134">Add allowedGroup</span></span>](../api/printershare-post-allowedgroups.md) | <span data-ttu-id="650ef-135">Нет</span><span class="sxs-lookup"><span data-stu-id="650ef-135">None</span></span> | <span data-ttu-id="650ef-136">Предоставление указанному групповому доступу на отправку заданий печати на связанный общий принтер.</span><span class="sxs-lookup"><span data-stu-id="650ef-136">Grant the specified group access to submit print jobs to the associated printer share.</span></span> |
| [<span data-ttu-id="650ef-137">Удаление allowedGroup</span><span class="sxs-lookup"><span data-stu-id="650ef-137">Remove allowedGroup</span></span>](../api/printershare-delete-allowedgroup.md) | <span data-ttu-id="650ef-138">Нет</span><span class="sxs-lookup"><span data-stu-id="650ef-138">None</span></span> | <span data-ttu-id="650ef-139">Отзыв доступа к общему принтеру из указанной группы.</span><span class="sxs-lookup"><span data-stu-id="650ef-139">Revoke printer share access from the specified group.</span></span> |

## <a name="properties"></a><span data-ttu-id="650ef-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="650ef-140">Properties</span></span>
| <span data-ttu-id="650ef-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="650ef-141">Property</span></span>     | <span data-ttu-id="650ef-142">Тип</span><span class="sxs-lookup"><span data-stu-id="650ef-142">Type</span></span>        | <span data-ttu-id="650ef-143">Описание</span><span class="sxs-lookup"><span data-stu-id="650ef-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="650ef-144">id</span><span class="sxs-lookup"><span data-stu-id="650ef-144">id</span></span>|<span data-ttu-id="650ef-145">Строка</span><span class="sxs-lookup"><span data-stu-id="650ef-145">String</span></span>| <span data-ttu-id="650ef-146">Идентификатор Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="650ef-146">The printerShare's identifier.</span></span> <span data-ttu-id="650ef-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="650ef-147">Read-only.</span></span>|
|<span data-ttu-id="650ef-148">name</span><span class="sxs-lookup"><span data-stu-id="650ef-148">name</span></span>|<span data-ttu-id="650ef-149">String</span><span class="sxs-lookup"><span data-stu-id="650ef-149">String</span></span>|<span data-ttu-id="650ef-150">Имя общего принтера, который должен отображаться клиентами печати.</span><span class="sxs-lookup"><span data-stu-id="650ef-150">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="650ef-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="650ef-151">createdDateTime</span></span>|<span data-ttu-id="650ef-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="650ef-152">DateTimeOffset</span></span>|<span data-ttu-id="650ef-153">Значение DateTimeOffset при создании общего ресурса принтера.</span><span class="sxs-lookup"><span data-stu-id="650ef-153">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="650ef-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="650ef-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="650ef-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="650ef-155">Relationships</span></span>
| <span data-ttu-id="650ef-156">Связь</span><span class="sxs-lookup"><span data-stu-id="650ef-156">Relationship</span></span> | <span data-ttu-id="650ef-157">Тип</span><span class="sxs-lookup"><span data-stu-id="650ef-157">Type</span></span>        | <span data-ttu-id="650ef-158">Описание</span><span class="sxs-lookup"><span data-stu-id="650ef-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="650ef-159">Printer</span><span class="sxs-lookup"><span data-stu-id="650ef-159">printer</span></span>|[<span data-ttu-id="650ef-160">Printer</span><span class="sxs-lookup"><span data-stu-id="650ef-160">printer</span></span>](printer.md)|<span data-ttu-id="650ef-161">Принтер, с которым связан этот общий принтер.</span><span class="sxs-lookup"><span data-stu-id="650ef-161">The printer that this printer share is related to.</span></span> |
|<span data-ttu-id="650ef-162">алловедусерс</span><span class="sxs-lookup"><span data-stu-id="650ef-162">allowedUsers</span></span>|<span data-ttu-id="650ef-163">Коллекция [userIdentity](useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="650ef-163">[userIdentity](useridentity.md) collection</span></span>|<span data-ttu-id="650ef-164">Пользователи, у которых есть доступ к печати с помощью принтера.</span><span class="sxs-lookup"><span data-stu-id="650ef-164">The users who have access to print using the printer.</span></span>|
|<span data-ttu-id="650ef-165">алловедграупс</span><span class="sxs-lookup"><span data-stu-id="650ef-165">allowedGroups</span></span>|[<span data-ttu-id="650ef-166">identity</span><span class="sxs-lookup"><span data-stu-id="650ef-166">identity</span></span>](identity.md)|<span data-ttu-id="650ef-167">Группы, у которых пользователи имеют доступ к печати с помощью принтера.</span><span class="sxs-lookup"><span data-stu-id="650ef-167">The groups whose users have access to print using the printer.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="650ef-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="650ef-168">JSON representation</span></span>

<span data-ttu-id="650ef-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="650ef-169">The following is a JSON representation of the resource.</span></span>

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
