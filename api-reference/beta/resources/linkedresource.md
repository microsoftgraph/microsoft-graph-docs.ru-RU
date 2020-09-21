---
title: Тип ресурса Линкедресаурце
description: Представляет источник Тодотаск
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3cbfaa0bf809a1996fe7a7c7df7014324406bcf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058111"
---
# <a name="linkedresource-resource-type"></a><span data-ttu-id="59cf6-103">Тип ресурса Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="59cf6-103">linkedResource resource type</span></span>

<span data-ttu-id="59cf6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59cf6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59cf6-105">Представляет элемент партнерского приложения, связанный с [тодотаск](./todotask.md).</span><span class="sxs-lookup"><span data-stu-id="59cf6-105">Represents an item in a partner application related to a [todoTask](./todotask.md).</span></span> <span data-ttu-id="59cf6-106">Примером является сообщение электронной почты, создавшее задачу.</span><span class="sxs-lookup"><span data-stu-id="59cf6-106">An example is an email that created the task.</span></span> <span data-ttu-id="59cf6-107">Объект **линкедресаурце** хранит сведения об этом исходном приложении и позволяет вернуться обратно к связанному элементу.</span><span class="sxs-lookup"><span data-stu-id="59cf6-107">A **linkedResource** object stores information about that source application, and lets you link back to the related item.</span></span>

## <a name="methods"></a><span data-ttu-id="59cf6-108">Методы</span><span class="sxs-lookup"><span data-stu-id="59cf6-108">Methods</span></span>
|<span data-ttu-id="59cf6-109">Метод</span><span class="sxs-lookup"><span data-stu-id="59cf6-109">Method</span></span>|<span data-ttu-id="59cf6-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="59cf6-110">Return type</span></span>|<span data-ttu-id="59cf6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="59cf6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="59cf6-112">Список Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="59cf6-112">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="59cf6-113">Коллекция [линкедресаурце](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="59cf6-113">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="59cf6-114">Получение Линкедресаурцес из свойства навигации Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="59cf6-114">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="59cf6-115">Создание Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="59cf6-115">Create linkedResource</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="59cf6-116">линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="59cf6-116">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="59cf6-117">Создание нового объекта Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="59cf6-117">Create a new linkedResources object.</span></span>|
|[<span data-ttu-id="59cf6-118">Получение Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="59cf6-118">Get linkedResource</span></span>](../api/linkedresource-get.md)|[<span data-ttu-id="59cf6-119">линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="59cf6-119">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="59cf6-120">Чтение свойств и связей объекта [линкедресаурце](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="59cf6-120">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="59cf6-121">Обновление Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="59cf6-121">Update linkedResource</span></span>](../api/linkedresource-update.md)|[<span data-ttu-id="59cf6-122">линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="59cf6-122">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="59cf6-123">Обновление свойств объекта [линкедресаурце](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="59cf6-123">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="59cf6-124">Удаление Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="59cf6-124">Delete linkedResource</span></span>](../api/linkedresource-delete.md)|<span data-ttu-id="59cf6-125">Нет</span><span class="sxs-lookup"><span data-stu-id="59cf6-125">None</span></span>|<span data-ttu-id="59cf6-126">Удаляет объект [линкедресаурце](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="59cf6-126">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="59cf6-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="59cf6-127">Properties</span></span>
|<span data-ttu-id="59cf6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="59cf6-128">Property</span></span>|<span data-ttu-id="59cf6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="59cf6-129">Type</span></span>|<span data-ttu-id="59cf6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="59cf6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59cf6-131">applicationName</span><span class="sxs-lookup"><span data-stu-id="59cf6-131">applicationName</span></span>|<span data-ttu-id="59cf6-132">String</span><span class="sxs-lookup"><span data-stu-id="59cf6-132">String</span></span>|<span data-ttu-id="59cf6-133">Поле, указывающее имя приложения источника, отправляющего **линкедресаурце**.</span><span class="sxs-lookup"><span data-stu-id="59cf6-133">Field indicating the app name of the source that is sending the **linkedResource**.</span></span>|
|<span data-ttu-id="59cf6-134">displayName</span><span class="sxs-lookup"><span data-stu-id="59cf6-134">displayName</span></span>|<span data-ttu-id="59cf6-135">String</span><span class="sxs-lookup"><span data-stu-id="59cf6-135">String</span></span>|<span data-ttu-id="59cf6-136">Поле, указывающее название **линкедресаурце**.</span><span class="sxs-lookup"><span data-stu-id="59cf6-136">Field indicating the title of the **linkedResource**.</span></span>|
|<span data-ttu-id="59cf6-137">externalId</span><span class="sxs-lookup"><span data-stu-id="59cf6-137">externalId</span></span>|<span data-ttu-id="59cf6-138">String</span><span class="sxs-lookup"><span data-stu-id="59cf6-138">String</span></span>|<span data-ttu-id="59cf6-139">Идентификатор объекта, связанного с этой задачей в сторонней системе или партнерской системе.</span><span class="sxs-lookup"><span data-stu-id="59cf6-139">Id of the object that is associated with this task on the third-party/partner system.</span></span>|
|<span data-ttu-id="59cf6-140">id</span><span class="sxs-lookup"><span data-stu-id="59cf6-140">id</span></span>|<span data-ttu-id="59cf6-141">String</span><span class="sxs-lookup"><span data-stu-id="59cf6-141">String</span></span>|<span data-ttu-id="59cf6-142">Созданный сервером идентификатор **линкедресаурце**.</span><span class="sxs-lookup"><span data-stu-id="59cf6-142">Server generated ID for the **linkedResource**.</span></span> <span data-ttu-id="59cf6-143">Наследуется от [объекта Entity](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="59cf6-143">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="59cf6-144">webUrl</span><span class="sxs-lookup"><span data-stu-id="59cf6-144">webUrl</span></span>|<span data-ttu-id="59cf6-145">String</span><span class="sxs-lookup"><span data-stu-id="59cf6-145">String</span></span>|<span data-ttu-id="59cf6-146">Глубокая ссылка на **линкедресаурце**.</span><span class="sxs-lookup"><span data-stu-id="59cf6-146">Deep link to the **linkedResource**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59cf6-147">Связи</span><span class="sxs-lookup"><span data-stu-id="59cf6-147">Relationships</span></span>
<span data-ttu-id="59cf6-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="59cf6-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59cf6-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="59cf6-149">JSON representation</span></span>
<span data-ttu-id="59cf6-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59cf6-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.linkedResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.linkedResource",
  "id": "String (identifier)",
  "webUrl": "String",
  "applicationName": "String",
  "displayName": "String",
  "externalId": "String"
}
```



