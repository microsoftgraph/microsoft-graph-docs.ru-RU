---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fcec7c8dfaa0461e6b88d67a5a0f73373a1af7b0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797369"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="19285-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="19285-103">managedEBook resource type</span></span>

> <span data-ttu-id="19285-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19285-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19285-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19285-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19285-106">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="19285-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="19285-107">Методы</span><span class="sxs-lookup"><span data-stu-id="19285-107">Methods</span></span>
|<span data-ttu-id="19285-108">Метод</span><span class="sxs-lookup"><span data-stu-id="19285-108">Method</span></span>|<span data-ttu-id="19285-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="19285-109">Return Type</span></span>|<span data-ttu-id="19285-110">Описание</span><span class="sxs-lookup"><span data-stu-id="19285-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="19285-111">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="19285-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="19285-112">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="19285-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="19285-113">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="19285-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="19285-114">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="19285-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="19285-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="19285-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="19285-116">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="19285-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="19285-117">действие назначения</span><span class="sxs-lookup"><span data-stu-id="19285-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="19285-118">Нет</span><span class="sxs-lookup"><span data-stu-id="19285-118">None</span></span>|<span data-ttu-id="19285-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="19285-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="19285-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="19285-120">Properties</span></span>
|<span data-ttu-id="19285-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="19285-121">Property</span></span>|<span data-ttu-id="19285-122">Тип</span><span class="sxs-lookup"><span data-stu-id="19285-122">Type</span></span>|<span data-ttu-id="19285-123">Описание</span><span class="sxs-lookup"><span data-stu-id="19285-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19285-124">id</span><span class="sxs-lookup"><span data-stu-id="19285-124">id</span></span>|<span data-ttu-id="19285-125">Строка</span><span class="sxs-lookup"><span data-stu-id="19285-125">String</span></span>|<span data-ttu-id="19285-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="19285-126">Key of the entity.</span></span>|
|<span data-ttu-id="19285-127">displayName</span><span class="sxs-lookup"><span data-stu-id="19285-127">displayName</span></span>|<span data-ttu-id="19285-128">Строка</span><span class="sxs-lookup"><span data-stu-id="19285-128">String</span></span>|<span data-ttu-id="19285-129">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="19285-129">Name of the eBook.</span></span>|
|<span data-ttu-id="19285-130">description</span><span class="sxs-lookup"><span data-stu-id="19285-130">description</span></span>|<span data-ttu-id="19285-131">String</span><span class="sxs-lookup"><span data-stu-id="19285-131">String</span></span>|<span data-ttu-id="19285-132">Описание.</span><span class="sxs-lookup"><span data-stu-id="19285-132">Description.</span></span>|
|<span data-ttu-id="19285-133">publisher</span><span class="sxs-lookup"><span data-stu-id="19285-133">publisher</span></span>|<span data-ttu-id="19285-134">String</span><span class="sxs-lookup"><span data-stu-id="19285-134">String</span></span>|<span data-ttu-id="19285-135">Издатель.</span><span class="sxs-lookup"><span data-stu-id="19285-135">Publisher.</span></span>|
|<span data-ttu-id="19285-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="19285-136">publishedDateTime</span></span>|<span data-ttu-id="19285-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19285-137">DateTimeOffset</span></span>|<span data-ttu-id="19285-138">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="19285-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="19285-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="19285-139">largeCover</span></span>|[<span data-ttu-id="19285-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="19285-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="19285-141">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="19285-141">Book cover.</span></span>|
|<span data-ttu-id="19285-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19285-142">createdDateTime</span></span>|<span data-ttu-id="19285-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19285-143">DateTimeOffset</span></span>|<span data-ttu-id="19285-144">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="19285-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="19285-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19285-145">lastModifiedDateTime</span></span>|<span data-ttu-id="19285-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19285-146">DateTimeOffset</span></span>|<span data-ttu-id="19285-147">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="19285-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="19285-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="19285-148">informationUrl</span></span>|<span data-ttu-id="19285-149">String</span><span class="sxs-lookup"><span data-stu-id="19285-149">String</span></span>|<span data-ttu-id="19285-150">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="19285-150">The more information Url.</span></span>|
|<span data-ttu-id="19285-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="19285-151">privacyInformationUrl</span></span>|<span data-ttu-id="19285-152">String</span><span class="sxs-lookup"><span data-stu-id="19285-152">String</span></span>|<span data-ttu-id="19285-153">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="19285-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19285-154">Связи</span><span class="sxs-lookup"><span data-stu-id="19285-154">Relationships</span></span>
|<span data-ttu-id="19285-155">Связь</span><span class="sxs-lookup"><span data-stu-id="19285-155">Relationship</span></span>|<span data-ttu-id="19285-156">Тип</span><span class="sxs-lookup"><span data-stu-id="19285-156">Type</span></span>|<span data-ttu-id="19285-157">Описание</span><span class="sxs-lookup"><span data-stu-id="19285-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19285-158">categories</span><span class="sxs-lookup"><span data-stu-id="19285-158">categories</span></span>|<span data-ttu-id="19285-159">Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="19285-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="19285-160">Список категорий для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="19285-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="19285-161">assignments</span><span class="sxs-lookup"><span data-stu-id="19285-161">assignments</span></span>|<span data-ttu-id="19285-162">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="19285-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="19285-163">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="19285-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="19285-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="19285-164">installSummary</span></span>|[<span data-ttu-id="19285-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="19285-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="19285-166">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="19285-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="19285-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="19285-167">deviceStates</span></span>|<span data-ttu-id="19285-168">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="19285-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="19285-169">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="19285-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="19285-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="19285-170">userStateSummary</span></span>|<span data-ttu-id="19285-171">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="19285-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="19285-172">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="19285-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19285-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19285-173">JSON Representation</span></span>
<span data-ttu-id="19285-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19285-174">Here is a JSON representation of the resource.</span></span>
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



