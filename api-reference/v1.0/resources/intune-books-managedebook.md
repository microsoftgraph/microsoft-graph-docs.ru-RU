---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 66d0efae21a68bd14286af45c4c021dbf7ba96fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531009"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="5d998-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="5d998-103">managedEBook resource type</span></span>

<span data-ttu-id="5d998-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d998-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d998-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d998-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d998-106">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5d998-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="5d998-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5d998-107">Methods</span></span>
|<span data-ttu-id="5d998-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5d998-108">Method</span></span>|<span data-ttu-id="5d998-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5d998-109">Return Type</span></span>|<span data-ttu-id="5d998-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5d998-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5d998-111">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="5d998-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="5d998-112">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="5d998-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="5d998-113">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5d998-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="5d998-114">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="5d998-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="5d998-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="5d998-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="5d998-116">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5d998-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="5d998-117">действие назначения</span><span class="sxs-lookup"><span data-stu-id="5d998-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="5d998-118">Нет</span><span class="sxs-lookup"><span data-stu-id="5d998-118">None</span></span>|<span data-ttu-id="5d998-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5d998-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5d998-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d998-120">Properties</span></span>
|<span data-ttu-id="5d998-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d998-121">Property</span></span>|<span data-ttu-id="5d998-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5d998-122">Type</span></span>|<span data-ttu-id="5d998-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5d998-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d998-124">id</span><span class="sxs-lookup"><span data-stu-id="5d998-124">id</span></span>|<span data-ttu-id="5d998-125">Строка</span><span class="sxs-lookup"><span data-stu-id="5d998-125">String</span></span>|<span data-ttu-id="5d998-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5d998-126">Key of the entity.</span></span>|
|<span data-ttu-id="5d998-127">displayName</span><span class="sxs-lookup"><span data-stu-id="5d998-127">displayName</span></span>|<span data-ttu-id="5d998-128">Строка</span><span class="sxs-lookup"><span data-stu-id="5d998-128">String</span></span>|<span data-ttu-id="5d998-129">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5d998-129">Name of the eBook.</span></span>|
|<span data-ttu-id="5d998-130">description</span><span class="sxs-lookup"><span data-stu-id="5d998-130">description</span></span>|<span data-ttu-id="5d998-131">String</span><span class="sxs-lookup"><span data-stu-id="5d998-131">String</span></span>|<span data-ttu-id="5d998-132">Описание.</span><span class="sxs-lookup"><span data-stu-id="5d998-132">Description.</span></span>|
|<span data-ttu-id="5d998-133">publisher</span><span class="sxs-lookup"><span data-stu-id="5d998-133">publisher</span></span>|<span data-ttu-id="5d998-134">String</span><span class="sxs-lookup"><span data-stu-id="5d998-134">String</span></span>|<span data-ttu-id="5d998-135">Издатель.</span><span class="sxs-lookup"><span data-stu-id="5d998-135">Publisher.</span></span>|
|<span data-ttu-id="5d998-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d998-136">publishedDateTime</span></span>|<span data-ttu-id="5d998-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d998-137">DateTimeOffset</span></span>|<span data-ttu-id="5d998-138">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5d998-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="5d998-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="5d998-139">largeCover</span></span>|[<span data-ttu-id="5d998-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5d998-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5d998-141">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="5d998-141">Book cover.</span></span>|
|<span data-ttu-id="5d998-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d998-142">createdDateTime</span></span>|<span data-ttu-id="5d998-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d998-143">DateTimeOffset</span></span>|<span data-ttu-id="5d998-144">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5d998-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="5d998-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d998-145">lastModifiedDateTime</span></span>|<span data-ttu-id="5d998-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d998-146">DateTimeOffset</span></span>|<span data-ttu-id="5d998-147">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5d998-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="5d998-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5d998-148">informationUrl</span></span>|<span data-ttu-id="5d998-149">String</span><span class="sxs-lookup"><span data-stu-id="5d998-149">String</span></span>|<span data-ttu-id="5d998-150">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5d998-150">The more information Url.</span></span>|
|<span data-ttu-id="5d998-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5d998-151">privacyInformationUrl</span></span>|<span data-ttu-id="5d998-152">Строка</span><span class="sxs-lookup"><span data-stu-id="5d998-152">String</span></span>|<span data-ttu-id="5d998-153">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5d998-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d998-154">Связи</span><span class="sxs-lookup"><span data-stu-id="5d998-154">Relationships</span></span>
|<span data-ttu-id="5d998-155">Связь</span><span class="sxs-lookup"><span data-stu-id="5d998-155">Relationship</span></span>|<span data-ttu-id="5d998-156">Тип</span><span class="sxs-lookup"><span data-stu-id="5d998-156">Type</span></span>|<span data-ttu-id="5d998-157">Описание</span><span class="sxs-lookup"><span data-stu-id="5d998-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d998-158">assignments</span><span class="sxs-lookup"><span data-stu-id="5d998-158">assignments</span></span>|<span data-ttu-id="5d998-159">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5d998-159">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="5d998-160">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5d998-160">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="5d998-161">installSummary</span><span class="sxs-lookup"><span data-stu-id="5d998-161">installSummary</span></span>|[<span data-ttu-id="5d998-162">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5d998-162">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="5d998-163">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="5d998-163">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="5d998-164">deviceStates</span><span class="sxs-lookup"><span data-stu-id="5d998-164">deviceStates</span></span>|<span data-ttu-id="5d998-165">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="5d998-165">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="5d998-166">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5d998-166">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="5d998-167">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="5d998-167">userStateSummary</span></span>|<span data-ttu-id="5d998-168">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="5d998-168">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="5d998-169">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5d998-169">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5d998-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d998-170">JSON Representation</span></span>
<span data-ttu-id="5d998-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d998-171">Here is a JSON representation of the resource.</span></span>
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




