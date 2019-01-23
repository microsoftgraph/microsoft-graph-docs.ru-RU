---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08bd5cc6f5630aca0ff5b35c5590875d259ad294
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422049"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="b6010-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="b6010-103">managedEBook resource type</span></span>

> <span data-ttu-id="b6010-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6010-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b6010-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6010-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6010-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6010-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6010-107">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b6010-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="b6010-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b6010-108">Methods</span></span>
|<span data-ttu-id="b6010-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b6010-109">Method</span></span>|<span data-ttu-id="b6010-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b6010-110">Return Type</span></span>|<span data-ttu-id="b6010-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b6010-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b6010-112">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="b6010-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="b6010-113">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="b6010-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="b6010-114">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b6010-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="b6010-115">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="b6010-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="b6010-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="b6010-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="b6010-117">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b6010-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="b6010-118">действие назначения</span><span class="sxs-lookup"><span data-stu-id="b6010-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="b6010-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b6010-119">None</span></span>|<span data-ttu-id="b6010-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b6010-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b6010-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6010-121">Properties</span></span>
|<span data-ttu-id="b6010-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6010-122">Property</span></span>|<span data-ttu-id="b6010-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b6010-123">Type</span></span>|<span data-ttu-id="b6010-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b6010-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6010-125">id</span><span class="sxs-lookup"><span data-stu-id="b6010-125">id</span></span>|<span data-ttu-id="b6010-126">String</span><span class="sxs-lookup"><span data-stu-id="b6010-126">String</span></span>|<span data-ttu-id="b6010-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b6010-127">Key of the entity.</span></span>|
|<span data-ttu-id="b6010-128">displayName</span><span class="sxs-lookup"><span data-stu-id="b6010-128">displayName</span></span>|<span data-ttu-id="b6010-129">String</span><span class="sxs-lookup"><span data-stu-id="b6010-129">String</span></span>|<span data-ttu-id="b6010-130">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b6010-130">Name of the eBook.</span></span>|
|<span data-ttu-id="b6010-131">description</span><span class="sxs-lookup"><span data-stu-id="b6010-131">description</span></span>|<span data-ttu-id="b6010-132">String</span><span class="sxs-lookup"><span data-stu-id="b6010-132">String</span></span>|<span data-ttu-id="b6010-133">Описание.</span><span class="sxs-lookup"><span data-stu-id="b6010-133">Description.</span></span>|
|<span data-ttu-id="b6010-134">publisher</span><span class="sxs-lookup"><span data-stu-id="b6010-134">publisher</span></span>|<span data-ttu-id="b6010-135">String</span><span class="sxs-lookup"><span data-stu-id="b6010-135">String</span></span>|<span data-ttu-id="b6010-136">Издатель.</span><span class="sxs-lookup"><span data-stu-id="b6010-136">Publisher.</span></span>|
|<span data-ttu-id="b6010-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6010-137">publishedDateTime</span></span>|<span data-ttu-id="b6010-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6010-138">DateTimeOffset</span></span>|<span data-ttu-id="b6010-139">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b6010-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="b6010-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="b6010-140">largeCover</span></span>|[<span data-ttu-id="b6010-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b6010-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b6010-142">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="b6010-142">Book cover.</span></span>|
|<span data-ttu-id="b6010-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6010-143">createdDateTime</span></span>|<span data-ttu-id="b6010-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6010-144">DateTimeOffset</span></span>|<span data-ttu-id="b6010-145">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b6010-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="b6010-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6010-146">lastModifiedDateTime</span></span>|<span data-ttu-id="b6010-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6010-147">DateTimeOffset</span></span>|<span data-ttu-id="b6010-148">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b6010-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="b6010-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b6010-149">informationUrl</span></span>|<span data-ttu-id="b6010-150">String</span><span class="sxs-lookup"><span data-stu-id="b6010-150">String</span></span>|<span data-ttu-id="b6010-151">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b6010-151">The more information Url.</span></span>|
|<span data-ttu-id="b6010-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b6010-152">privacyInformationUrl</span></span>|<span data-ttu-id="b6010-153">String</span><span class="sxs-lookup"><span data-stu-id="b6010-153">String</span></span>|<span data-ttu-id="b6010-154">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b6010-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6010-155">Связи</span><span class="sxs-lookup"><span data-stu-id="b6010-155">Relationships</span></span>
|<span data-ttu-id="b6010-156">Связь</span><span class="sxs-lookup"><span data-stu-id="b6010-156">Relationship</span></span>|<span data-ttu-id="b6010-157">Тип</span><span class="sxs-lookup"><span data-stu-id="b6010-157">Type</span></span>|<span data-ttu-id="b6010-158">Описание</span><span class="sxs-lookup"><span data-stu-id="b6010-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6010-159">categories</span><span class="sxs-lookup"><span data-stu-id="b6010-159">categories</span></span>|<span data-ttu-id="b6010-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b6010-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="b6010-161">Список категорий для этой книги.</span><span class="sxs-lookup"><span data-stu-id="b6010-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="b6010-162">assignments</span><span class="sxs-lookup"><span data-stu-id="b6010-162">assignments</span></span>|<span data-ttu-id="b6010-163">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b6010-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="b6010-164">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b6010-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="b6010-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="b6010-165">installSummary</span></span>|[<span data-ttu-id="b6010-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b6010-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="b6010-167">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b6010-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="b6010-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="b6010-168">deviceStates</span></span>|<span data-ttu-id="b6010-169">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="b6010-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="b6010-170">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b6010-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="b6010-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="b6010-171">userStateSummary</span></span>|<span data-ttu-id="b6010-172">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="b6010-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="b6010-173">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b6010-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6010-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6010-174">JSON Representation</span></span>
<span data-ttu-id="b6010-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6010-175">Here is a JSON representation of the resource.</span></span>
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




