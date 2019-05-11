---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a9248a2bca56188deb913159d9ff664ce8d9b48
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949299"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="9d37b-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="9d37b-103">managedEBook resource type</span></span>

> <span data-ttu-id="9d37b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d37b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d37b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d37b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d37b-106">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9d37b-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="9d37b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9d37b-107">Methods</span></span>
|<span data-ttu-id="9d37b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9d37b-108">Method</span></span>|<span data-ttu-id="9d37b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9d37b-109">Return Type</span></span>|<span data-ttu-id="9d37b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9d37b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9d37b-111">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="9d37b-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="9d37b-112">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="9d37b-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="9d37b-113">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="9d37b-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="9d37b-114">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="9d37b-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="9d37b-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="9d37b-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="9d37b-116">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="9d37b-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="9d37b-117">действие назначения</span><span class="sxs-lookup"><span data-stu-id="9d37b-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="9d37b-118">Нет</span><span class="sxs-lookup"><span data-stu-id="9d37b-118">None</span></span>|<span data-ttu-id="9d37b-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9d37b-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9d37b-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d37b-120">Properties</span></span>
|<span data-ttu-id="9d37b-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d37b-121">Property</span></span>|<span data-ttu-id="9d37b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="9d37b-122">Type</span></span>|<span data-ttu-id="9d37b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9d37b-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d37b-124">id</span><span class="sxs-lookup"><span data-stu-id="9d37b-124">id</span></span>|<span data-ttu-id="9d37b-125">Строка</span><span class="sxs-lookup"><span data-stu-id="9d37b-125">String</span></span>|<span data-ttu-id="9d37b-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9d37b-126">Key of the entity.</span></span>|
|<span data-ttu-id="9d37b-127">displayName</span><span class="sxs-lookup"><span data-stu-id="9d37b-127">displayName</span></span>|<span data-ttu-id="9d37b-128">Строка</span><span class="sxs-lookup"><span data-stu-id="9d37b-128">String</span></span>|<span data-ttu-id="9d37b-129">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9d37b-129">Name of the eBook.</span></span>|
|<span data-ttu-id="9d37b-130">description</span><span class="sxs-lookup"><span data-stu-id="9d37b-130">description</span></span>|<span data-ttu-id="9d37b-131">String</span><span class="sxs-lookup"><span data-stu-id="9d37b-131">String</span></span>|<span data-ttu-id="9d37b-132">Описание.</span><span class="sxs-lookup"><span data-stu-id="9d37b-132">Description.</span></span>|
|<span data-ttu-id="9d37b-133">publisher</span><span class="sxs-lookup"><span data-stu-id="9d37b-133">publisher</span></span>|<span data-ttu-id="9d37b-134">String</span><span class="sxs-lookup"><span data-stu-id="9d37b-134">String</span></span>|<span data-ttu-id="9d37b-135">Издатель.</span><span class="sxs-lookup"><span data-stu-id="9d37b-135">Publisher.</span></span>|
|<span data-ttu-id="9d37b-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d37b-136">publishedDateTime</span></span>|<span data-ttu-id="9d37b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d37b-137">DateTimeOffset</span></span>|<span data-ttu-id="9d37b-138">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9d37b-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="9d37b-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="9d37b-139">largeCover</span></span>|[<span data-ttu-id="9d37b-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9d37b-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9d37b-141">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="9d37b-141">Book cover.</span></span>|
|<span data-ttu-id="9d37b-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d37b-142">createdDateTime</span></span>|<span data-ttu-id="9d37b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d37b-143">DateTimeOffset</span></span>|<span data-ttu-id="9d37b-144">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9d37b-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="9d37b-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d37b-145">lastModifiedDateTime</span></span>|<span data-ttu-id="9d37b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d37b-146">DateTimeOffset</span></span>|<span data-ttu-id="9d37b-147">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9d37b-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="9d37b-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9d37b-148">informationUrl</span></span>|<span data-ttu-id="9d37b-149">String</span><span class="sxs-lookup"><span data-stu-id="9d37b-149">String</span></span>|<span data-ttu-id="9d37b-150">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9d37b-150">The more information Url.</span></span>|
|<span data-ttu-id="9d37b-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9d37b-151">privacyInformationUrl</span></span>|<span data-ttu-id="9d37b-152">Строка</span><span class="sxs-lookup"><span data-stu-id="9d37b-152">String</span></span>|<span data-ttu-id="9d37b-153">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9d37b-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d37b-154">Связи</span><span class="sxs-lookup"><span data-stu-id="9d37b-154">Relationships</span></span>
|<span data-ttu-id="9d37b-155">Отношение</span><span class="sxs-lookup"><span data-stu-id="9d37b-155">Relationship</span></span>|<span data-ttu-id="9d37b-156">Тип</span><span class="sxs-lookup"><span data-stu-id="9d37b-156">Type</span></span>|<span data-ttu-id="9d37b-157">Описание</span><span class="sxs-lookup"><span data-stu-id="9d37b-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d37b-158">categories</span><span class="sxs-lookup"><span data-stu-id="9d37b-158">categories</span></span>|<span data-ttu-id="9d37b-159">Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="9d37b-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="9d37b-160">Список категорий для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9d37b-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="9d37b-161">assignments</span><span class="sxs-lookup"><span data-stu-id="9d37b-161">assignments</span></span>|<span data-ttu-id="9d37b-162">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9d37b-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="9d37b-163">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9d37b-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="9d37b-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="9d37b-164">installSummary</span></span>|[<span data-ttu-id="9d37b-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9d37b-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="9d37b-166">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9d37b-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="9d37b-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="9d37b-167">deviceStates</span></span>|<span data-ttu-id="9d37b-168">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="9d37b-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="9d37b-169">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9d37b-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="9d37b-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="9d37b-170">userStateSummary</span></span>|<span data-ttu-id="9d37b-171">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9d37b-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="9d37b-172">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9d37b-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d37b-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d37b-173">JSON Representation</span></span>
<span data-ttu-id="9d37b-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d37b-174">Here is a JSON representation of the resource.</span></span>
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




