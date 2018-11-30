---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
ms.openlocfilehash: 427582977558254561b219dff2392f01ced4f53d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027680"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="3b213-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="3b213-103">managedEBook resource type</span></span>

> <span data-ttu-id="3b213-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3b213-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b213-105">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3b213-105">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="3b213-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3b213-106">Methods</span></span>
|<span data-ttu-id="3b213-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3b213-107">Method</span></span>|<span data-ttu-id="3b213-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3b213-108">Return Type</span></span>|<span data-ttu-id="3b213-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3b213-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3b213-110">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="3b213-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="3b213-111">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3b213-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="3b213-112">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3b213-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="3b213-113">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="3b213-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="3b213-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="3b213-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="3b213-115">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3b213-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="3b213-116">действие назначения</span><span class="sxs-lookup"><span data-stu-id="3b213-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="3b213-117">Нет</span><span class="sxs-lookup"><span data-stu-id="3b213-117">None</span></span>|<span data-ttu-id="3b213-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3b213-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3b213-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b213-119">Properties</span></span>
|<span data-ttu-id="3b213-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b213-120">Property</span></span>|<span data-ttu-id="3b213-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3b213-121">Type</span></span>|<span data-ttu-id="3b213-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3b213-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b213-123">id</span><span class="sxs-lookup"><span data-stu-id="3b213-123">id</span></span>|<span data-ttu-id="3b213-124">String</span><span class="sxs-lookup"><span data-stu-id="3b213-124">String</span></span>|<span data-ttu-id="3b213-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3b213-125">Key of the entity.</span></span>|
|<span data-ttu-id="3b213-126">displayName</span><span class="sxs-lookup"><span data-stu-id="3b213-126">displayName</span></span>|<span data-ttu-id="3b213-127">String</span><span class="sxs-lookup"><span data-stu-id="3b213-127">String</span></span>|<span data-ttu-id="3b213-128">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3b213-128">Name of the eBook.</span></span>|
|<span data-ttu-id="3b213-129">описание</span><span class="sxs-lookup"><span data-stu-id="3b213-129">description</span></span>|<span data-ttu-id="3b213-130">String</span><span class="sxs-lookup"><span data-stu-id="3b213-130">String</span></span>|<span data-ttu-id="3b213-131">Описание.</span><span class="sxs-lookup"><span data-stu-id="3b213-131">Description.</span></span>|
|<span data-ttu-id="3b213-132">publisher</span><span class="sxs-lookup"><span data-stu-id="3b213-132">publisher</span></span>|<span data-ttu-id="3b213-133">String</span><span class="sxs-lookup"><span data-stu-id="3b213-133">String</span></span>|<span data-ttu-id="3b213-134">Издатель.</span><span class="sxs-lookup"><span data-stu-id="3b213-134">Publisher.</span></span>|
|<span data-ttu-id="3b213-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b213-135">publishedDateTime</span></span>|<span data-ttu-id="3b213-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b213-136">DateTimeOffset</span></span>|<span data-ttu-id="3b213-137">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3b213-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="3b213-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="3b213-138">largeCover</span></span>|[<span data-ttu-id="3b213-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3b213-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3b213-140">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="3b213-140">Book cover.</span></span>|
|<span data-ttu-id="3b213-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b213-141">createdDateTime</span></span>|<span data-ttu-id="3b213-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b213-142">DateTimeOffset</span></span>|<span data-ttu-id="3b213-143">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3b213-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="3b213-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b213-144">lastModifiedDateTime</span></span>|<span data-ttu-id="3b213-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b213-145">DateTimeOffset</span></span>|<span data-ttu-id="3b213-146">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3b213-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="3b213-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3b213-147">informationUrl</span></span>|<span data-ttu-id="3b213-148">String</span><span class="sxs-lookup"><span data-stu-id="3b213-148">String</span></span>|<span data-ttu-id="3b213-149">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3b213-149">The more information Url.</span></span>|
|<span data-ttu-id="3b213-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3b213-150">privacyInformationUrl</span></span>|<span data-ttu-id="3b213-151">String</span><span class="sxs-lookup"><span data-stu-id="3b213-151">String</span></span>|<span data-ttu-id="3b213-152">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3b213-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b213-153">Связи</span><span class="sxs-lookup"><span data-stu-id="3b213-153">Relationships</span></span>
|<span data-ttu-id="3b213-154">Связь</span><span class="sxs-lookup"><span data-stu-id="3b213-154">Relationship</span></span>|<span data-ttu-id="3b213-155">Тип</span><span class="sxs-lookup"><span data-stu-id="3b213-155">Type</span></span>|<span data-ttu-id="3b213-156">Описание</span><span class="sxs-lookup"><span data-stu-id="3b213-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b213-157">assignments</span><span class="sxs-lookup"><span data-stu-id="3b213-157">assignments</span></span>|<span data-ttu-id="3b213-158">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3b213-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="3b213-159">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3b213-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="3b213-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="3b213-160">installSummary</span></span>|[<span data-ttu-id="3b213-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3b213-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="3b213-162">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="3b213-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="3b213-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="3b213-163">deviceStates</span></span>|<span data-ttu-id="3b213-164">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="3b213-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="3b213-165">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3b213-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="3b213-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="3b213-166">userStateSummary</span></span>|<span data-ttu-id="3b213-167">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="3b213-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="3b213-168">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3b213-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b213-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b213-169">JSON Representation</span></span>
<span data-ttu-id="3b213-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b213-170">Here is a JSON representation of the resource.</span></span>
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



