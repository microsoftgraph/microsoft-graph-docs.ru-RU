---
title: Тип ресурса Линкедресаурце
description: Представляет источник Тодотаск
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 70303742db1dabb866585be7099cb222f8a428bd
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797356"
---
# <a name="linkedresource-resource-type"></a><span data-ttu-id="e4518-103">Тип ресурса Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="e4518-103">linkedResource resource type</span></span>

<span data-ttu-id="e4518-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4518-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="e4518-105">Представляет элемент партнерского приложения, связанный с [тодотаск](./todotask.md).</span><span class="sxs-lookup"><span data-stu-id="e4518-105">Represents an item in a partner application related to a [todoTask](./todotask.md).</span></span> <span data-ttu-id="e4518-106">Примером является сообщение электронной почты, из которого была создана задача.</span><span class="sxs-lookup"><span data-stu-id="e4518-106">An example is an email from where the task was created.</span></span> <span data-ttu-id="e4518-107">Объект **линкедресаурце** хранит сведения об этом исходном приложении и позволяет вернуться обратно к связанному элементу.</span><span class="sxs-lookup"><span data-stu-id="e4518-107">A **linkedResource** object stores information about that source application, and lets you link back to the related item.</span></span> <span data-ttu-id="e4518-108">**Линкедресаурце** можно просмотреть в представлении "сведения о задаче", как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="e4518-108">You can see the **linkedResource** in the task details view, as shown.</span></span>

![Связанный ресурс в области сведений о задаче](/graph/images/todo-linkedresource-taskdetail.png)

<span data-ttu-id="e4518-110">Некоторые объекты **линкедресаурце** не связаны ни с одним из веб-URL-адресов, в этом случае свойство **webUrl** не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e4518-110">Some **linkedResource** objects are not associated with any web URLs, in which case, the **webUrl** property is not required.</span></span> <span data-ttu-id="e4518-111">Например, связанный элемент может относиться к пользовательскому бизнес-приложению или собственному приложению платформы, например к приложению SMS на мобильном телефоне.</span><span class="sxs-lookup"><span data-stu-id="e4518-111">For example, the linked item can be from a custom business app or native platform app, such as an SMS app on a mobile phone.</span></span> <span data-ttu-id="e4518-112">Ниже показано, как отображается **линкедресаурце** с URL-адресом и без него.</span><span class="sxs-lookup"><span data-stu-id="e4518-112">Here is how a **linkedResource** appears with and without a URL.</span></span>

![Связанный ресурс с URL-адресом и без него](/graph/images/todo-linkedresource.png)

## <a name="methods"></a><span data-ttu-id="e4518-114">Методы</span><span class="sxs-lookup"><span data-stu-id="e4518-114">Methods</span></span>
|<span data-ttu-id="e4518-115">Метод</span><span class="sxs-lookup"><span data-stu-id="e4518-115">Method</span></span>|<span data-ttu-id="e4518-116">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="e4518-116">Return type</span></span>|<span data-ttu-id="e4518-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e4518-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e4518-118">Список Линкедресаурцес</span><span class="sxs-lookup"><span data-stu-id="e4518-118">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="e4518-119">Коллекция [линкедресаурце](../resources/linkedresource.md)</span><span class="sxs-lookup"><span data-stu-id="e4518-119">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="e4518-120">Получение Линкедресаурцес из свойства навигации Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="e4518-120">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="e4518-121">Создание Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="e4518-121">Create linkedResource</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="e4518-122">линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="e4518-122">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="e4518-123">Создание нового объекта Линкедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="e4518-123">Create a new linkedResources object.</span></span>|
|[<span data-ttu-id="e4518-124">Получение Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="e4518-124">Get linkedResource</span></span>](../api/linkedresource-get.md)|[<span data-ttu-id="e4518-125">линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="e4518-125">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="e4518-126">Чтение свойств и связей объекта [линкедресаурце](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="e4518-126">Read the properties and relationships of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="e4518-127">Обновление Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="e4518-127">Update linkedResource</span></span>](../api/linkedresource-update.md)|[<span data-ttu-id="e4518-128">линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="e4518-128">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="e4518-129">Обновление свойств объекта [линкедресаурце](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="e4518-129">Update the properties of a [linkedResource](../resources/linkedresource.md) object.</span></span>|
|[<span data-ttu-id="e4518-130">Удаление Линкедресаурце</span><span class="sxs-lookup"><span data-stu-id="e4518-130">Delete linkedResource</span></span>](../api/linkedresource-delete.md)|<span data-ttu-id="e4518-131">Нет</span><span class="sxs-lookup"><span data-stu-id="e4518-131">None</span></span>|<span data-ttu-id="e4518-132">Удаляет объект [линкедресаурце](../resources/linkedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="e4518-132">Deletes a [linkedResource](../resources/linkedresource.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e4518-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4518-133">Properties</span></span>
|<span data-ttu-id="e4518-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4518-134">Property</span></span>|<span data-ttu-id="e4518-135">Тип</span><span class="sxs-lookup"><span data-stu-id="e4518-135">Type</span></span>|<span data-ttu-id="e4518-136">Описание</span><span class="sxs-lookup"><span data-stu-id="e4518-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4518-137">applicationName</span><span class="sxs-lookup"><span data-stu-id="e4518-137">applicationName</span></span>|<span data-ttu-id="e4518-138">String</span><span class="sxs-lookup"><span data-stu-id="e4518-138">String</span></span>|<span data-ttu-id="e4518-139">Поле, указывающее имя приложения источника, отправляющего **линкедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="e4518-139">Field indicating the app name of the source that is sending the **linkedResource** .</span></span>|
|<span data-ttu-id="e4518-140">displayName</span><span class="sxs-lookup"><span data-stu-id="e4518-140">displayName</span></span>|<span data-ttu-id="e4518-141">String</span><span class="sxs-lookup"><span data-stu-id="e4518-141">String</span></span>|<span data-ttu-id="e4518-142">Поле, указывающее название **линкедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="e4518-142">Field indicating the title of the **linkedResource** .</span></span>|
|<span data-ttu-id="e4518-143">externalId</span><span class="sxs-lookup"><span data-stu-id="e4518-143">externalId</span></span>|<span data-ttu-id="e4518-144">String</span><span class="sxs-lookup"><span data-stu-id="e4518-144">String</span></span>|<span data-ttu-id="e4518-145">Идентификатор объекта, связанного с этой задачей в сторонней системе или партнерской системе.</span><span class="sxs-lookup"><span data-stu-id="e4518-145">Id of the object that is associated with this task on the third-party/partner system.</span></span>|
|<span data-ttu-id="e4518-146">id</span><span class="sxs-lookup"><span data-stu-id="e4518-146">id</span></span>|<span data-ttu-id="e4518-147">String</span><span class="sxs-lookup"><span data-stu-id="e4518-147">String</span></span>|<span data-ttu-id="e4518-148">Созданный сервером идентификатор **линкедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="e4518-148">Server generated ID for the **linkedResource** .</span></span> <span data-ttu-id="e4518-149">Наследуется от [объекта Entity](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="e4518-149">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="e4518-150">webUrl</span><span class="sxs-lookup"><span data-stu-id="e4518-150">webUrl</span></span>|<span data-ttu-id="e4518-151">String</span><span class="sxs-lookup"><span data-stu-id="e4518-151">String</span></span>|<span data-ttu-id="e4518-152">Глубокая ссылка на **линкедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="e4518-152">Deep link to the **linkedResource** .</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4518-153">Связи</span><span class="sxs-lookup"><span data-stu-id="e4518-153">Relationships</span></span>
<span data-ttu-id="e4518-154">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e4518-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4518-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e4518-155">JSON representation</span></span>
<span data-ttu-id="e4518-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4518-156">The following is a JSON representation of the resource.</span></span>
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



