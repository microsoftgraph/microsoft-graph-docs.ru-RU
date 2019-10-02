---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3288b86ec735b4480577bb36a604107a51bb4f7f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360463"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="5e7f1-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="5e7f1-103">managedEBook resource type</span></span>

> <span data-ttu-id="5e7f1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e7f1-105">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-105">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="5e7f1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5e7f1-106">Methods</span></span>
|<span data-ttu-id="5e7f1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5e7f1-107">Method</span></span>|<span data-ttu-id="5e7f1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5e7f1-108">Return Type</span></span>|<span data-ttu-id="5e7f1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5e7f1-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e7f1-110">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="5e7f1-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="5e7f1-111">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="5e7f1-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="5e7f1-112">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e7f1-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="5e7f1-113">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="5e7f1-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="5e7f1-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="5e7f1-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="5e7f1-115">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e7f1-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="5e7f1-116">действие назначения</span><span class="sxs-lookup"><span data-stu-id="5e7f1-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="5e7f1-117">Нет</span><span class="sxs-lookup"><span data-stu-id="5e7f1-117">None</span></span>|<span data-ttu-id="5e7f1-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5e7f1-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5e7f1-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e7f1-119">Properties</span></span>
|<span data-ttu-id="5e7f1-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e7f1-120">Property</span></span>|<span data-ttu-id="5e7f1-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5e7f1-121">Type</span></span>|<span data-ttu-id="5e7f1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5e7f1-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e7f1-123">id</span><span class="sxs-lookup"><span data-stu-id="5e7f1-123">id</span></span>|<span data-ttu-id="5e7f1-124">Строка</span><span class="sxs-lookup"><span data-stu-id="5e7f1-124">String</span></span>|<span data-ttu-id="5e7f1-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-125">Key of the entity.</span></span>|
|<span data-ttu-id="5e7f1-126">displayName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-126">displayName</span></span>|<span data-ttu-id="5e7f1-127">Строка</span><span class="sxs-lookup"><span data-stu-id="5e7f1-127">String</span></span>|<span data-ttu-id="5e7f1-128">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-128">Name of the eBook.</span></span>|
|<span data-ttu-id="5e7f1-129">description</span><span class="sxs-lookup"><span data-stu-id="5e7f1-129">description</span></span>|<span data-ttu-id="5e7f1-130">String</span><span class="sxs-lookup"><span data-stu-id="5e7f1-130">String</span></span>|<span data-ttu-id="5e7f1-131">Описание.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-131">Description.</span></span>|
|<span data-ttu-id="5e7f1-132">publisher</span><span class="sxs-lookup"><span data-stu-id="5e7f1-132">publisher</span></span>|<span data-ttu-id="5e7f1-133">String</span><span class="sxs-lookup"><span data-stu-id="5e7f1-133">String</span></span>|<span data-ttu-id="5e7f1-134">Издатель.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-134">Publisher.</span></span>|
|<span data-ttu-id="5e7f1-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e7f1-135">publishedDateTime</span></span>|<span data-ttu-id="5e7f1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e7f1-136">DateTimeOffset</span></span>|<span data-ttu-id="5e7f1-137">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="5e7f1-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="5e7f1-138">largeCover</span></span>|[<span data-ttu-id="5e7f1-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5e7f1-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5e7f1-140">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-140">Book cover.</span></span>|
|<span data-ttu-id="5e7f1-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e7f1-141">createdDateTime</span></span>|<span data-ttu-id="5e7f1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e7f1-142">DateTimeOffset</span></span>|<span data-ttu-id="5e7f1-143">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="5e7f1-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e7f1-144">lastModifiedDateTime</span></span>|<span data-ttu-id="5e7f1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e7f1-145">DateTimeOffset</span></span>|<span data-ttu-id="5e7f1-146">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="5e7f1-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5e7f1-147">informationUrl</span></span>|<span data-ttu-id="5e7f1-148">String</span><span class="sxs-lookup"><span data-stu-id="5e7f1-148">String</span></span>|<span data-ttu-id="5e7f1-149">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-149">The more information Url.</span></span>|
|<span data-ttu-id="5e7f1-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5e7f1-150">privacyInformationUrl</span></span>|<span data-ttu-id="5e7f1-151">String</span><span class="sxs-lookup"><span data-stu-id="5e7f1-151">String</span></span>|<span data-ttu-id="5e7f1-152">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e7f1-153">Связи</span><span class="sxs-lookup"><span data-stu-id="5e7f1-153">Relationships</span></span>
|<span data-ttu-id="5e7f1-154">Связь</span><span class="sxs-lookup"><span data-stu-id="5e7f1-154">Relationship</span></span>|<span data-ttu-id="5e7f1-155">Тип</span><span class="sxs-lookup"><span data-stu-id="5e7f1-155">Type</span></span>|<span data-ttu-id="5e7f1-156">Описание</span><span class="sxs-lookup"><span data-stu-id="5e7f1-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e7f1-157">assignments</span><span class="sxs-lookup"><span data-stu-id="5e7f1-157">assignments</span></span>|<span data-ttu-id="5e7f1-158">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5e7f1-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="5e7f1-159">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="5e7f1-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="5e7f1-160">installSummary</span></span>|[<span data-ttu-id="5e7f1-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5e7f1-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="5e7f1-162">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="5e7f1-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="5e7f1-163">deviceStates</span></span>|<span data-ttu-id="5e7f1-164">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="5e7f1-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="5e7f1-165">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="5e7f1-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="5e7f1-166">userStateSummary</span></span>|<span data-ttu-id="5e7f1-167">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="5e7f1-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="5e7f1-168">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e7f1-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e7f1-169">JSON Representation</span></span>
<span data-ttu-id="5e7f1-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e7f1-170">Here is a JSON representation of the resource.</span></span>
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




