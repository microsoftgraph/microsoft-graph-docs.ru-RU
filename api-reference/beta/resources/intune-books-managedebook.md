---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c6d39e1a965713054304e7faaf127ab8a735758c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004836"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="64585-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="64585-103">managedEBook resource type</span></span>

> <span data-ttu-id="64585-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64585-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64585-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64585-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64585-106">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="64585-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="64585-107">Методы</span><span class="sxs-lookup"><span data-stu-id="64585-107">Methods</span></span>
|<span data-ttu-id="64585-108">Метод</span><span class="sxs-lookup"><span data-stu-id="64585-108">Method</span></span>|<span data-ttu-id="64585-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="64585-109">Return Type</span></span>|<span data-ttu-id="64585-110">Описание</span><span class="sxs-lookup"><span data-stu-id="64585-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="64585-111">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="64585-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="64585-112">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="64585-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="64585-113">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="64585-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="64585-114">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="64585-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="64585-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="64585-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="64585-116">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="64585-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="64585-117">действие назначения</span><span class="sxs-lookup"><span data-stu-id="64585-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="64585-118">Нет</span><span class="sxs-lookup"><span data-stu-id="64585-118">None</span></span>|<span data-ttu-id="64585-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="64585-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="64585-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="64585-120">Properties</span></span>
|<span data-ttu-id="64585-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="64585-121">Property</span></span>|<span data-ttu-id="64585-122">Тип</span><span class="sxs-lookup"><span data-stu-id="64585-122">Type</span></span>|<span data-ttu-id="64585-123">Описание</span><span class="sxs-lookup"><span data-stu-id="64585-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64585-124">id</span><span class="sxs-lookup"><span data-stu-id="64585-124">id</span></span>|<span data-ttu-id="64585-125">Строка</span><span class="sxs-lookup"><span data-stu-id="64585-125">String</span></span>|<span data-ttu-id="64585-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="64585-126">Key of the entity.</span></span>|
|<span data-ttu-id="64585-127">displayName</span><span class="sxs-lookup"><span data-stu-id="64585-127">displayName</span></span>|<span data-ttu-id="64585-128">Строка</span><span class="sxs-lookup"><span data-stu-id="64585-128">String</span></span>|<span data-ttu-id="64585-129">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="64585-129">Name of the eBook.</span></span>|
|<span data-ttu-id="64585-130">description</span><span class="sxs-lookup"><span data-stu-id="64585-130">description</span></span>|<span data-ttu-id="64585-131">String</span><span class="sxs-lookup"><span data-stu-id="64585-131">String</span></span>|<span data-ttu-id="64585-132">Описание.</span><span class="sxs-lookup"><span data-stu-id="64585-132">Description.</span></span>|
|<span data-ttu-id="64585-133">publisher</span><span class="sxs-lookup"><span data-stu-id="64585-133">publisher</span></span>|<span data-ttu-id="64585-134">String</span><span class="sxs-lookup"><span data-stu-id="64585-134">String</span></span>|<span data-ttu-id="64585-135">Издатель.</span><span class="sxs-lookup"><span data-stu-id="64585-135">Publisher.</span></span>|
|<span data-ttu-id="64585-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="64585-136">publishedDateTime</span></span>|<span data-ttu-id="64585-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64585-137">DateTimeOffset</span></span>|<span data-ttu-id="64585-138">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="64585-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="64585-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="64585-139">largeCover</span></span>|[<span data-ttu-id="64585-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="64585-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="64585-141">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="64585-141">Book cover.</span></span>|
|<span data-ttu-id="64585-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64585-142">createdDateTime</span></span>|<span data-ttu-id="64585-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64585-143">DateTimeOffset</span></span>|<span data-ttu-id="64585-144">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="64585-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="64585-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64585-145">lastModifiedDateTime</span></span>|<span data-ttu-id="64585-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64585-146">DateTimeOffset</span></span>|<span data-ttu-id="64585-147">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="64585-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="64585-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="64585-148">informationUrl</span></span>|<span data-ttu-id="64585-149">String</span><span class="sxs-lookup"><span data-stu-id="64585-149">String</span></span>|<span data-ttu-id="64585-150">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="64585-150">The more information Url.</span></span>|
|<span data-ttu-id="64585-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="64585-151">privacyInformationUrl</span></span>|<span data-ttu-id="64585-152">String</span><span class="sxs-lookup"><span data-stu-id="64585-152">String</span></span>|<span data-ttu-id="64585-153">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="64585-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64585-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="64585-154">Relationships</span></span>
|<span data-ttu-id="64585-155">Отношение</span><span class="sxs-lookup"><span data-stu-id="64585-155">Relationship</span></span>|<span data-ttu-id="64585-156">Тип</span><span class="sxs-lookup"><span data-stu-id="64585-156">Type</span></span>|<span data-ttu-id="64585-157">Описание</span><span class="sxs-lookup"><span data-stu-id="64585-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64585-158">categories</span><span class="sxs-lookup"><span data-stu-id="64585-158">categories</span></span>|<span data-ttu-id="64585-159">Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="64585-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="64585-160">Список категорий для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="64585-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="64585-161">assignments</span><span class="sxs-lookup"><span data-stu-id="64585-161">assignments</span></span>|<span data-ttu-id="64585-162">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="64585-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="64585-163">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="64585-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="64585-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="64585-164">installSummary</span></span>|[<span data-ttu-id="64585-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="64585-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="64585-166">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="64585-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="64585-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="64585-167">deviceStates</span></span>|<span data-ttu-id="64585-168">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="64585-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="64585-169">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="64585-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="64585-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="64585-170">userStateSummary</span></span>|<span data-ttu-id="64585-171">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="64585-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="64585-172">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="64585-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64585-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64585-173">JSON Representation</span></span>
<span data-ttu-id="64585-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64585-174">Here is a JSON representation of the resource.</span></span>
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





