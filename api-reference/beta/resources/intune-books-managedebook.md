---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01fd5b25e4fb7861ef2ea6e2ddd0c810f706b8f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021793"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="1e915-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="1e915-103">managedEBook resource type</span></span>

<span data-ttu-id="1e915-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e915-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e915-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e915-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e915-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e915-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e915-107">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="1e915-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="1e915-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1e915-108">Methods</span></span>
|<span data-ttu-id="1e915-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1e915-109">Method</span></span>|<span data-ttu-id="1e915-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1e915-110">Return Type</span></span>|<span data-ttu-id="1e915-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1e915-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1e915-112">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="1e915-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="1e915-113">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="1e915-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="1e915-114">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="1e915-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="1e915-115">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="1e915-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="1e915-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="1e915-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="1e915-117">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="1e915-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="1e915-118">действие назначения</span><span class="sxs-lookup"><span data-stu-id="1e915-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="1e915-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1e915-119">None</span></span>|<span data-ttu-id="1e915-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1e915-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1e915-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e915-121">Properties</span></span>
|<span data-ttu-id="1e915-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e915-122">Property</span></span>|<span data-ttu-id="1e915-123">Тип</span><span class="sxs-lookup"><span data-stu-id="1e915-123">Type</span></span>|<span data-ttu-id="1e915-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1e915-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e915-125">id</span><span class="sxs-lookup"><span data-stu-id="1e915-125">id</span></span>|<span data-ttu-id="1e915-126">String</span><span class="sxs-lookup"><span data-stu-id="1e915-126">String</span></span>|<span data-ttu-id="1e915-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1e915-127">Key of the entity.</span></span>|
|<span data-ttu-id="1e915-128">displayName</span><span class="sxs-lookup"><span data-stu-id="1e915-128">displayName</span></span>|<span data-ttu-id="1e915-129">String</span><span class="sxs-lookup"><span data-stu-id="1e915-129">String</span></span>|<span data-ttu-id="1e915-130">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="1e915-130">Name of the eBook.</span></span>|
|<span data-ttu-id="1e915-131">description</span><span class="sxs-lookup"><span data-stu-id="1e915-131">description</span></span>|<span data-ttu-id="1e915-132">String</span><span class="sxs-lookup"><span data-stu-id="1e915-132">String</span></span>|<span data-ttu-id="1e915-133">Описание.</span><span class="sxs-lookup"><span data-stu-id="1e915-133">Description.</span></span>|
|<span data-ttu-id="1e915-134">publisher</span><span class="sxs-lookup"><span data-stu-id="1e915-134">publisher</span></span>|<span data-ttu-id="1e915-135">String</span><span class="sxs-lookup"><span data-stu-id="1e915-135">String</span></span>|<span data-ttu-id="1e915-136">Издатель.</span><span class="sxs-lookup"><span data-stu-id="1e915-136">Publisher.</span></span>|
|<span data-ttu-id="1e915-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e915-137">publishedDateTime</span></span>|<span data-ttu-id="1e915-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e915-138">DateTimeOffset</span></span>|<span data-ttu-id="1e915-139">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="1e915-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="1e915-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="1e915-140">largeCover</span></span>|[<span data-ttu-id="1e915-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1e915-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1e915-142">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="1e915-142">Book cover.</span></span>|
|<span data-ttu-id="1e915-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e915-143">createdDateTime</span></span>|<span data-ttu-id="1e915-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e915-144">DateTimeOffset</span></span>|<span data-ttu-id="1e915-145">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="1e915-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="1e915-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e915-146">lastModifiedDateTime</span></span>|<span data-ttu-id="1e915-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e915-147">DateTimeOffset</span></span>|<span data-ttu-id="1e915-148">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="1e915-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="1e915-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1e915-149">informationUrl</span></span>|<span data-ttu-id="1e915-150">String</span><span class="sxs-lookup"><span data-stu-id="1e915-150">String</span></span>|<span data-ttu-id="1e915-151">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="1e915-151">The more information Url.</span></span>|
|<span data-ttu-id="1e915-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1e915-152">privacyInformationUrl</span></span>|<span data-ttu-id="1e915-153">String</span><span class="sxs-lookup"><span data-stu-id="1e915-153">String</span></span>|<span data-ttu-id="1e915-154">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="1e915-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e915-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="1e915-155">Relationships</span></span>
|<span data-ttu-id="1e915-156">Связь</span><span class="sxs-lookup"><span data-stu-id="1e915-156">Relationship</span></span>|<span data-ttu-id="1e915-157">Тип</span><span class="sxs-lookup"><span data-stu-id="1e915-157">Type</span></span>|<span data-ttu-id="1e915-158">Описание</span><span class="sxs-lookup"><span data-stu-id="1e915-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e915-159">categories</span><span class="sxs-lookup"><span data-stu-id="1e915-159">categories</span></span>|<span data-ttu-id="1e915-160">Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1e915-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="1e915-161">Список категорий для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="1e915-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="1e915-162">assignments</span><span class="sxs-lookup"><span data-stu-id="1e915-162">assignments</span></span>|<span data-ttu-id="1e915-163">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1e915-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="1e915-164">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="1e915-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="1e915-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="1e915-165">installSummary</span></span>|[<span data-ttu-id="1e915-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="1e915-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="1e915-167">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="1e915-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="1e915-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="1e915-168">deviceStates</span></span>|<span data-ttu-id="1e915-169">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="1e915-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="1e915-170">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="1e915-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="1e915-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="1e915-171">userStateSummary</span></span>|<span data-ttu-id="1e915-172">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="1e915-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="1e915-173">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="1e915-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e915-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e915-174">JSON Representation</span></span>
<span data-ttu-id="1e915-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e915-175">Here is a JSON representation of the resource.</span></span>
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






