---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: tfitzmac
ms.openlocfilehash: 584464b95eaa242ddae6653af65f16d9d2eeab3b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336766"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="fcc73-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="fcc73-103">managedEBook resource type</span></span>

> <span data-ttu-id="fcc73-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fcc73-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcc73-105">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fcc73-105">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="fcc73-106">Методы</span><span class="sxs-lookup"><span data-stu-id="fcc73-106">Methods</span></span>
|<span data-ttu-id="fcc73-107">Метод</span><span class="sxs-lookup"><span data-stu-id="fcc73-107">Method</span></span>|<span data-ttu-id="fcc73-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fcc73-108">Return Type</span></span>|<span data-ttu-id="fcc73-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fcc73-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fcc73-110">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="fcc73-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="fcc73-111">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="fcc73-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="fcc73-112">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fcc73-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="fcc73-113">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="fcc73-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="fcc73-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="fcc73-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="fcc73-115">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="fcc73-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="fcc73-116">действие назначения</span><span class="sxs-lookup"><span data-stu-id="fcc73-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="fcc73-117">Нет</span><span class="sxs-lookup"><span data-stu-id="fcc73-117">None</span></span>|<span data-ttu-id="fcc73-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fcc73-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fcc73-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcc73-119">Properties</span></span>
|<span data-ttu-id="fcc73-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcc73-120">Property</span></span>|<span data-ttu-id="fcc73-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fcc73-121">Type</span></span>|<span data-ttu-id="fcc73-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fcc73-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcc73-123">id</span><span class="sxs-lookup"><span data-stu-id="fcc73-123">id</span></span>|<span data-ttu-id="fcc73-124">Строка</span><span class="sxs-lookup"><span data-stu-id="fcc73-124">String</span></span>|<span data-ttu-id="fcc73-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fcc73-125">Key of the entity.</span></span>|
|<span data-ttu-id="fcc73-126">displayName</span><span class="sxs-lookup"><span data-stu-id="fcc73-126">displayName</span></span>|<span data-ttu-id="fcc73-127">String</span><span class="sxs-lookup"><span data-stu-id="fcc73-127">String</span></span>|<span data-ttu-id="fcc73-128">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fcc73-128">Name of the eBook.</span></span>|
|<span data-ttu-id="fcc73-129">описание</span><span class="sxs-lookup"><span data-stu-id="fcc73-129">description</span></span>|<span data-ttu-id="fcc73-130">Строка</span><span class="sxs-lookup"><span data-stu-id="fcc73-130">String</span></span>|<span data-ttu-id="fcc73-131">Описание.</span><span class="sxs-lookup"><span data-stu-id="fcc73-131">Description.</span></span>|
|<span data-ttu-id="fcc73-132">publisher</span><span class="sxs-lookup"><span data-stu-id="fcc73-132">publisher</span></span>|<span data-ttu-id="fcc73-133">String</span><span class="sxs-lookup"><span data-stu-id="fcc73-133">String</span></span>|<span data-ttu-id="fcc73-134">Издатель.</span><span class="sxs-lookup"><span data-stu-id="fcc73-134">Publisher.</span></span>|
|<span data-ttu-id="fcc73-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcc73-135">publishedDateTime</span></span>|<span data-ttu-id="fcc73-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcc73-136">DateTimeOffset</span></span>|<span data-ttu-id="fcc73-137">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fcc73-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="fcc73-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="fcc73-138">largeCover</span></span>|[<span data-ttu-id="fcc73-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fcc73-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fcc73-140">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="fcc73-140">Book cover.</span></span>|
|<span data-ttu-id="fcc73-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fcc73-141">createdDateTime</span></span>|<span data-ttu-id="fcc73-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcc73-142">DateTimeOffset</span></span>|<span data-ttu-id="fcc73-143">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fcc73-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="fcc73-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcc73-144">lastModifiedDateTime</span></span>|<span data-ttu-id="fcc73-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcc73-145">DateTimeOffset</span></span>|<span data-ttu-id="fcc73-146">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fcc73-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="fcc73-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fcc73-147">informationUrl</span></span>|<span data-ttu-id="fcc73-148">String</span><span class="sxs-lookup"><span data-stu-id="fcc73-148">String</span></span>|<span data-ttu-id="fcc73-149">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="fcc73-149">The more information Url.</span></span>|
|<span data-ttu-id="fcc73-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fcc73-150">privacyInformationUrl</span></span>|<span data-ttu-id="fcc73-151">String</span><span class="sxs-lookup"><span data-stu-id="fcc73-151">String</span></span>|<span data-ttu-id="fcc73-152">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="fcc73-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcc73-153">Связи</span><span class="sxs-lookup"><span data-stu-id="fcc73-153">Relationships</span></span>
|<span data-ttu-id="fcc73-154">Связь</span><span class="sxs-lookup"><span data-stu-id="fcc73-154">Relationship</span></span>|<span data-ttu-id="fcc73-155">Тип</span><span class="sxs-lookup"><span data-stu-id="fcc73-155">Type</span></span>|<span data-ttu-id="fcc73-156">Описание</span><span class="sxs-lookup"><span data-stu-id="fcc73-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcc73-157">assignments</span><span class="sxs-lookup"><span data-stu-id="fcc73-157">assignments</span></span>|<span data-ttu-id="fcc73-158">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fcc73-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="fcc73-159">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fcc73-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="fcc73-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="fcc73-160">installSummary</span></span>|[<span data-ttu-id="fcc73-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="fcc73-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="fcc73-162">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="fcc73-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="fcc73-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="fcc73-163">deviceStates</span></span>|<span data-ttu-id="fcc73-164">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="fcc73-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="fcc73-165">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fcc73-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="fcc73-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="fcc73-166">userStateSummary</span></span>|<span data-ttu-id="fcc73-167">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="fcc73-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="fcc73-168">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="fcc73-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fcc73-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcc73-169">JSON Representation</span></span>
<span data-ttu-id="fcc73-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcc73-170">Here is a JSON representation of the resource.</span></span>
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



