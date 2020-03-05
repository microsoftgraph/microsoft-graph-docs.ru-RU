---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 040da9c471d42ff77423dc035cce8b255ab9299a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42488728"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="f34cd-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="f34cd-103">managedEBook resource type</span></span>

<span data-ttu-id="f34cd-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f34cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f34cd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f34cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f34cd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f34cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f34cd-107">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f34cd-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="f34cd-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f34cd-108">Methods</span></span>
|<span data-ttu-id="f34cd-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f34cd-109">Method</span></span>|<span data-ttu-id="f34cd-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f34cd-110">Return Type</span></span>|<span data-ttu-id="f34cd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f34cd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f34cd-112">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="f34cd-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="f34cd-113">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f34cd-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="f34cd-114">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f34cd-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="f34cd-115">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="f34cd-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="f34cd-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="f34cd-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="f34cd-117">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f34cd-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="f34cd-118">действие назначения</span><span class="sxs-lookup"><span data-stu-id="f34cd-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="f34cd-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f34cd-119">None</span></span>|<span data-ttu-id="f34cd-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f34cd-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f34cd-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="f34cd-121">Properties</span></span>
|<span data-ttu-id="f34cd-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="f34cd-122">Property</span></span>|<span data-ttu-id="f34cd-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f34cd-123">Type</span></span>|<span data-ttu-id="f34cd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f34cd-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f34cd-125">id</span><span class="sxs-lookup"><span data-stu-id="f34cd-125">id</span></span>|<span data-ttu-id="f34cd-126">Строка</span><span class="sxs-lookup"><span data-stu-id="f34cd-126">String</span></span>|<span data-ttu-id="f34cd-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f34cd-127">Key of the entity.</span></span>|
|<span data-ttu-id="f34cd-128">displayName</span><span class="sxs-lookup"><span data-stu-id="f34cd-128">displayName</span></span>|<span data-ttu-id="f34cd-129">Строка</span><span class="sxs-lookup"><span data-stu-id="f34cd-129">String</span></span>|<span data-ttu-id="f34cd-130">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f34cd-130">Name of the eBook.</span></span>|
|<span data-ttu-id="f34cd-131">description</span><span class="sxs-lookup"><span data-stu-id="f34cd-131">description</span></span>|<span data-ttu-id="f34cd-132">String</span><span class="sxs-lookup"><span data-stu-id="f34cd-132">String</span></span>|<span data-ttu-id="f34cd-133">Описание.</span><span class="sxs-lookup"><span data-stu-id="f34cd-133">Description.</span></span>|
|<span data-ttu-id="f34cd-134">publisher</span><span class="sxs-lookup"><span data-stu-id="f34cd-134">publisher</span></span>|<span data-ttu-id="f34cd-135">String</span><span class="sxs-lookup"><span data-stu-id="f34cd-135">String</span></span>|<span data-ttu-id="f34cd-136">Издатель.</span><span class="sxs-lookup"><span data-stu-id="f34cd-136">Publisher.</span></span>|
|<span data-ttu-id="f34cd-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="f34cd-137">publishedDateTime</span></span>|<span data-ttu-id="f34cd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f34cd-138">DateTimeOffset</span></span>|<span data-ttu-id="f34cd-139">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f34cd-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="f34cd-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="f34cd-140">largeCover</span></span>|[<span data-ttu-id="f34cd-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f34cd-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f34cd-142">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="f34cd-142">Book cover.</span></span>|
|<span data-ttu-id="f34cd-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f34cd-143">createdDateTime</span></span>|<span data-ttu-id="f34cd-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f34cd-144">DateTimeOffset</span></span>|<span data-ttu-id="f34cd-145">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f34cd-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="f34cd-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f34cd-146">lastModifiedDateTime</span></span>|<span data-ttu-id="f34cd-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f34cd-147">DateTimeOffset</span></span>|<span data-ttu-id="f34cd-148">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f34cd-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="f34cd-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f34cd-149">informationUrl</span></span>|<span data-ttu-id="f34cd-150">String</span><span class="sxs-lookup"><span data-stu-id="f34cd-150">String</span></span>|<span data-ttu-id="f34cd-151">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f34cd-151">The more information Url.</span></span>|
|<span data-ttu-id="f34cd-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f34cd-152">privacyInformationUrl</span></span>|<span data-ttu-id="f34cd-153">String</span><span class="sxs-lookup"><span data-stu-id="f34cd-153">String</span></span>|<span data-ttu-id="f34cd-154">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f34cd-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f34cd-155">Связи</span><span class="sxs-lookup"><span data-stu-id="f34cd-155">Relationships</span></span>
|<span data-ttu-id="f34cd-156">Связь</span><span class="sxs-lookup"><span data-stu-id="f34cd-156">Relationship</span></span>|<span data-ttu-id="f34cd-157">Тип</span><span class="sxs-lookup"><span data-stu-id="f34cd-157">Type</span></span>|<span data-ttu-id="f34cd-158">Описание</span><span class="sxs-lookup"><span data-stu-id="f34cd-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f34cd-159">categories</span><span class="sxs-lookup"><span data-stu-id="f34cd-159">categories</span></span>|<span data-ttu-id="f34cd-160">Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="f34cd-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="f34cd-161">Список категорий для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f34cd-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="f34cd-162">assignments</span><span class="sxs-lookup"><span data-stu-id="f34cd-162">assignments</span></span>|<span data-ttu-id="f34cd-163">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f34cd-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="f34cd-164">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f34cd-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="f34cd-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="f34cd-165">installSummary</span></span>|[<span data-ttu-id="f34cd-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f34cd-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="f34cd-167">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f34cd-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="f34cd-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="f34cd-168">deviceStates</span></span>|<span data-ttu-id="f34cd-169">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="f34cd-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="f34cd-170">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f34cd-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="f34cd-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="f34cd-171">userStateSummary</span></span>|<span data-ttu-id="f34cd-172">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="f34cd-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="f34cd-173">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f34cd-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f34cd-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f34cd-174">JSON Representation</span></span>
<span data-ttu-id="f34cd-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f34cd-175">Here is a JSON representation of the resource.</span></span>
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



