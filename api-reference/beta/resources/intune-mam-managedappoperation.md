---
title: Тип ресурса managedAppOperation
description: Представляет операцию, примененную к регистрации приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a8c7ee3f49ad9b98d680662834911c2d20984d8d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951798"
---
# <a name="managedappoperation-resource-type"></a><span data-ttu-id="50998-103">Тип ресурса managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="50998-103">managedAppOperation resource type</span></span>

> <span data-ttu-id="50998-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="50998-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50998-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50998-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50998-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="50998-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50998-107">Представляет операцию, примененную к регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="50998-107">Represents an operation applied against an app registration.</span></span>
## <a name="methods"></a><span data-ttu-id="50998-108">Методы</span><span class="sxs-lookup"><span data-stu-id="50998-108">Methods</span></span>
|<span data-ttu-id="50998-109">Метод</span><span class="sxs-lookup"><span data-stu-id="50998-109">Method</span></span>|<span data-ttu-id="50998-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="50998-110">Return Type</span></span>|<span data-ttu-id="50998-111">Описание</span><span class="sxs-lookup"><span data-stu-id="50998-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50998-112">Список объектов List managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="50998-112">List managedAppOperations</span></span>](../api/intune-mam-managedappoperation-list.md)|<span data-ttu-id="50998-113">Коллекция [managedAppOperation](../resources/intune-mam-managedappoperation.md)</span><span class="sxs-lookup"><span data-stu-id="50998-113">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="50998-114">Список свойств и связей объектов [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="50998-114">List properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) objects.</span></span>|
|[<span data-ttu-id="50998-115">Получение объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="50998-115">Get managedAppOperation</span></span>](../api/intune-mam-managedappoperation-get.md)|[<span data-ttu-id="50998-116">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="50998-116">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="50998-117">Чтение свойств и связей объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="50998-117">Read properties and relationships of the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="50998-118">Создание объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="50998-118">Create managedAppOperation</span></span>](../api/intune-mam-managedappoperation-create.md)|[<span data-ttu-id="50998-119">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="50998-119">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="50998-120">Создание объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="50998-120">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|
|[<span data-ttu-id="50998-121">Удаление объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="50998-121">Delete managedAppOperation</span></span>](../api/intune-mam-managedappoperation-delete.md)|<span data-ttu-id="50998-122">Нет</span><span class="sxs-lookup"><span data-stu-id="50998-122">None</span></span>|<span data-ttu-id="50998-123">Удаляет объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="50998-123">Deletes a [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>|
|[<span data-ttu-id="50998-124">Обновление объекта managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="50998-124">Update managedAppOperation</span></span>](../api/intune-mam-managedappoperation-update.md)|[<span data-ttu-id="50998-125">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="50998-125">managedAppOperation</span></span>](../resources/intune-mam-managedappoperation.md)|<span data-ttu-id="50998-126">Обновление свойств объекта [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span><span class="sxs-lookup"><span data-stu-id="50998-126">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="50998-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="50998-127">Properties</span></span>
|<span data-ttu-id="50998-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="50998-128">Property</span></span>|<span data-ttu-id="50998-129">Тип</span><span class="sxs-lookup"><span data-stu-id="50998-129">Type</span></span>|<span data-ttu-id="50998-130">Описание</span><span class="sxs-lookup"><span data-stu-id="50998-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50998-131">displayName</span><span class="sxs-lookup"><span data-stu-id="50998-131">displayName</span></span>|<span data-ttu-id="50998-132">String</span><span class="sxs-lookup"><span data-stu-id="50998-132">String</span></span>|<span data-ttu-id="50998-133">Имя операции.</span><span class="sxs-lookup"><span data-stu-id="50998-133">The operation name.</span></span>|
|<span data-ttu-id="50998-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50998-134">lastModifiedDateTime</span></span>|<span data-ttu-id="50998-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50998-135">DateTimeOffset</span></span>|<span data-ttu-id="50998-136">Время последнего изменения операции для приложения.</span><span class="sxs-lookup"><span data-stu-id="50998-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="50998-137">state</span><span class="sxs-lookup"><span data-stu-id="50998-137">state</span></span>|<span data-ttu-id="50998-138">String</span><span class="sxs-lookup"><span data-stu-id="50998-138">String</span></span>|<span data-ttu-id="50998-139">Текущее состояние операции</span><span class="sxs-lookup"><span data-stu-id="50998-139">The current state of the operation</span></span>|
|<span data-ttu-id="50998-140">id</span><span class="sxs-lookup"><span data-stu-id="50998-140">id</span></span>|<span data-ttu-id="50998-141">Строка</span><span class="sxs-lookup"><span data-stu-id="50998-141">String</span></span>|<span data-ttu-id="50998-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="50998-142">Key of the entity.</span></span>|
|<span data-ttu-id="50998-143">version</span><span class="sxs-lookup"><span data-stu-id="50998-143">version</span></span>|<span data-ttu-id="50998-144">Строка</span><span class="sxs-lookup"><span data-stu-id="50998-144">String</span></span>|<span data-ttu-id="50998-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="50998-145">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50998-146">Связи</span><span class="sxs-lookup"><span data-stu-id="50998-146">Relationships</span></span>
<span data-ttu-id="50998-147">Нет</span><span class="sxs-lookup"><span data-stu-id="50998-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="50998-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50998-148">JSON Representation</span></span>
<span data-ttu-id="50998-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50998-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```





