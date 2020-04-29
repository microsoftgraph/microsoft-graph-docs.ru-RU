---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a73da0f3f9fc6eb86f158ece8f9a8f8eecb663d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468669"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="18d39-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="18d39-103">managedEBook resource type</span></span>

<span data-ttu-id="18d39-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18d39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18d39-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18d39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18d39-106">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="18d39-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="18d39-107">Методы</span><span class="sxs-lookup"><span data-stu-id="18d39-107">Methods</span></span>
|<span data-ttu-id="18d39-108">Метод</span><span class="sxs-lookup"><span data-stu-id="18d39-108">Method</span></span>|<span data-ttu-id="18d39-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="18d39-109">Return Type</span></span>|<span data-ttu-id="18d39-110">Описание</span><span class="sxs-lookup"><span data-stu-id="18d39-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="18d39-111">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="18d39-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="18d39-112">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="18d39-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="18d39-113">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="18d39-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="18d39-114">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="18d39-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="18d39-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="18d39-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="18d39-116">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="18d39-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="18d39-117">действие назначения</span><span class="sxs-lookup"><span data-stu-id="18d39-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="18d39-118">Нет</span><span class="sxs-lookup"><span data-stu-id="18d39-118">None</span></span>|<span data-ttu-id="18d39-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="18d39-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="18d39-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="18d39-120">Properties</span></span>
|<span data-ttu-id="18d39-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="18d39-121">Property</span></span>|<span data-ttu-id="18d39-122">Тип</span><span class="sxs-lookup"><span data-stu-id="18d39-122">Type</span></span>|<span data-ttu-id="18d39-123">Описание</span><span class="sxs-lookup"><span data-stu-id="18d39-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18d39-124">id</span><span class="sxs-lookup"><span data-stu-id="18d39-124">id</span></span>|<span data-ttu-id="18d39-125">Строка</span><span class="sxs-lookup"><span data-stu-id="18d39-125">String</span></span>|<span data-ttu-id="18d39-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="18d39-126">Key of the entity.</span></span>|
|<span data-ttu-id="18d39-127">displayName</span><span class="sxs-lookup"><span data-stu-id="18d39-127">displayName</span></span>|<span data-ttu-id="18d39-128">Строка</span><span class="sxs-lookup"><span data-stu-id="18d39-128">String</span></span>|<span data-ttu-id="18d39-129">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="18d39-129">Name of the eBook.</span></span>|
|<span data-ttu-id="18d39-130">description</span><span class="sxs-lookup"><span data-stu-id="18d39-130">description</span></span>|<span data-ttu-id="18d39-131">String</span><span class="sxs-lookup"><span data-stu-id="18d39-131">String</span></span>|<span data-ttu-id="18d39-132">Описание.</span><span class="sxs-lookup"><span data-stu-id="18d39-132">Description.</span></span>|
|<span data-ttu-id="18d39-133">publisher</span><span class="sxs-lookup"><span data-stu-id="18d39-133">publisher</span></span>|<span data-ttu-id="18d39-134">String</span><span class="sxs-lookup"><span data-stu-id="18d39-134">String</span></span>|<span data-ttu-id="18d39-135">Издатель.</span><span class="sxs-lookup"><span data-stu-id="18d39-135">Publisher.</span></span>|
|<span data-ttu-id="18d39-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="18d39-136">publishedDateTime</span></span>|<span data-ttu-id="18d39-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18d39-137">DateTimeOffset</span></span>|<span data-ttu-id="18d39-138">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="18d39-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="18d39-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="18d39-139">largeCover</span></span>|[<span data-ttu-id="18d39-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="18d39-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="18d39-141">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="18d39-141">Book cover.</span></span>|
|<span data-ttu-id="18d39-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18d39-142">createdDateTime</span></span>|<span data-ttu-id="18d39-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18d39-143">DateTimeOffset</span></span>|<span data-ttu-id="18d39-144">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="18d39-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="18d39-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18d39-145">lastModifiedDateTime</span></span>|<span data-ttu-id="18d39-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18d39-146">DateTimeOffset</span></span>|<span data-ttu-id="18d39-147">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="18d39-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="18d39-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="18d39-148">informationUrl</span></span>|<span data-ttu-id="18d39-149">String</span><span class="sxs-lookup"><span data-stu-id="18d39-149">String</span></span>|<span data-ttu-id="18d39-150">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="18d39-150">The more information Url.</span></span>|
|<span data-ttu-id="18d39-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="18d39-151">privacyInformationUrl</span></span>|<span data-ttu-id="18d39-152">String</span><span class="sxs-lookup"><span data-stu-id="18d39-152">String</span></span>|<span data-ttu-id="18d39-153">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="18d39-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18d39-154">Связи</span><span class="sxs-lookup"><span data-stu-id="18d39-154">Relationships</span></span>
|<span data-ttu-id="18d39-155">Связь</span><span class="sxs-lookup"><span data-stu-id="18d39-155">Relationship</span></span>|<span data-ttu-id="18d39-156">Тип</span><span class="sxs-lookup"><span data-stu-id="18d39-156">Type</span></span>|<span data-ttu-id="18d39-157">Описание</span><span class="sxs-lookup"><span data-stu-id="18d39-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18d39-158">assignments</span><span class="sxs-lookup"><span data-stu-id="18d39-158">assignments</span></span>|<span data-ttu-id="18d39-159">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="18d39-159">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="18d39-160">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="18d39-160">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="18d39-161">installSummary</span><span class="sxs-lookup"><span data-stu-id="18d39-161">installSummary</span></span>|[<span data-ttu-id="18d39-162">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="18d39-162">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="18d39-163">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="18d39-163">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="18d39-164">deviceStates</span><span class="sxs-lookup"><span data-stu-id="18d39-164">deviceStates</span></span>|<span data-ttu-id="18d39-165">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="18d39-165">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="18d39-166">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="18d39-166">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="18d39-167">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="18d39-167">userStateSummary</span></span>|<span data-ttu-id="18d39-168">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="18d39-168">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="18d39-169">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="18d39-169">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18d39-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18d39-170">JSON Representation</span></span>
<span data-ttu-id="18d39-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18d39-171">Here is a JSON representation of the resource.</span></span>
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







