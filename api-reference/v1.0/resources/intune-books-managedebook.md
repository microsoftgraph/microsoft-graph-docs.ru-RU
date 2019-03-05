---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae6151c23bf05b076ade441f908a2810c80f45ed
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253465"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="5982e-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="5982e-103">managedEBook resource type</span></span>

> <span data-ttu-id="5982e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5982e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5982e-105">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5982e-105">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="5982e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5982e-106">Methods</span></span>
|<span data-ttu-id="5982e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5982e-107">Method</span></span>|<span data-ttu-id="5982e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5982e-108">Return Type</span></span>|<span data-ttu-id="5982e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5982e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5982e-110">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="5982e-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="5982e-111">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="5982e-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="5982e-112">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5982e-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="5982e-113">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="5982e-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="5982e-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="5982e-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="5982e-115">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5982e-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="5982e-116">действие назначения</span><span class="sxs-lookup"><span data-stu-id="5982e-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="5982e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="5982e-117">None</span></span>|<span data-ttu-id="5982e-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5982e-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5982e-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="5982e-119">Properties</span></span>
|<span data-ttu-id="5982e-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="5982e-120">Property</span></span>|<span data-ttu-id="5982e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5982e-121">Type</span></span>|<span data-ttu-id="5982e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5982e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5982e-123">id</span><span class="sxs-lookup"><span data-stu-id="5982e-123">id</span></span>|<span data-ttu-id="5982e-124">Строка</span><span class="sxs-lookup"><span data-stu-id="5982e-124">String</span></span>|<span data-ttu-id="5982e-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5982e-125">Key of the entity.</span></span>|
|<span data-ttu-id="5982e-126">displayName</span><span class="sxs-lookup"><span data-stu-id="5982e-126">displayName</span></span>|<span data-ttu-id="5982e-127">String</span><span class="sxs-lookup"><span data-stu-id="5982e-127">String</span></span>|<span data-ttu-id="5982e-128">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5982e-128">Name of the eBook.</span></span>|
|<span data-ttu-id="5982e-129">description</span><span class="sxs-lookup"><span data-stu-id="5982e-129">description</span></span>|<span data-ttu-id="5982e-130">String</span><span class="sxs-lookup"><span data-stu-id="5982e-130">String</span></span>|<span data-ttu-id="5982e-131">Описание.</span><span class="sxs-lookup"><span data-stu-id="5982e-131">Description.</span></span>|
|<span data-ttu-id="5982e-132">publisher</span><span class="sxs-lookup"><span data-stu-id="5982e-132">publisher</span></span>|<span data-ttu-id="5982e-133">String</span><span class="sxs-lookup"><span data-stu-id="5982e-133">String</span></span>|<span data-ttu-id="5982e-134">Издатель.</span><span class="sxs-lookup"><span data-stu-id="5982e-134">Publisher.</span></span>|
|<span data-ttu-id="5982e-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="5982e-135">publishedDateTime</span></span>|<span data-ttu-id="5982e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5982e-136">DateTimeOffset</span></span>|<span data-ttu-id="5982e-137">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5982e-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="5982e-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="5982e-138">largeCover</span></span>|[<span data-ttu-id="5982e-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5982e-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5982e-140">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="5982e-140">Book cover.</span></span>|
|<span data-ttu-id="5982e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5982e-141">createdDateTime</span></span>|<span data-ttu-id="5982e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5982e-142">DateTimeOffset</span></span>|<span data-ttu-id="5982e-143">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5982e-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="5982e-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5982e-144">lastModifiedDateTime</span></span>|<span data-ttu-id="5982e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5982e-145">DateTimeOffset</span></span>|<span data-ttu-id="5982e-146">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5982e-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="5982e-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5982e-147">informationUrl</span></span>|<span data-ttu-id="5982e-148">String</span><span class="sxs-lookup"><span data-stu-id="5982e-148">String</span></span>|<span data-ttu-id="5982e-149">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5982e-149">The more information Url.</span></span>|
|<span data-ttu-id="5982e-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5982e-150">privacyInformationUrl</span></span>|<span data-ttu-id="5982e-151">String</span><span class="sxs-lookup"><span data-stu-id="5982e-151">String</span></span>|<span data-ttu-id="5982e-152">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5982e-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5982e-153">Связи</span><span class="sxs-lookup"><span data-stu-id="5982e-153">Relationships</span></span>
|<span data-ttu-id="5982e-154">Отношение</span><span class="sxs-lookup"><span data-stu-id="5982e-154">Relationship</span></span>|<span data-ttu-id="5982e-155">Тип</span><span class="sxs-lookup"><span data-stu-id="5982e-155">Type</span></span>|<span data-ttu-id="5982e-156">Описание</span><span class="sxs-lookup"><span data-stu-id="5982e-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5982e-157">assignments</span><span class="sxs-lookup"><span data-stu-id="5982e-157">assignments</span></span>|<span data-ttu-id="5982e-158">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5982e-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="5982e-159">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5982e-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="5982e-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="5982e-160">installSummary</span></span>|[<span data-ttu-id="5982e-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5982e-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="5982e-162">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="5982e-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="5982e-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="5982e-163">deviceStates</span></span>|<span data-ttu-id="5982e-164">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="5982e-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="5982e-165">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5982e-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="5982e-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="5982e-166">userStateSummary</span></span>|<span data-ttu-id="5982e-167">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="5982e-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="5982e-168">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5982e-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5982e-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5982e-169">JSON Representation</span></span>
<span data-ttu-id="5982e-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5982e-170">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



