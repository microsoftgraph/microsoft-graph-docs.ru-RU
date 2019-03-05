---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24a8619d92eee6c666b7126a84895b14e0404755
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156037"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="ed524-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="ed524-103">managedEBook resource type</span></span>

> <span data-ttu-id="ed524-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed524-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed524-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed524-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed524-106">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ed524-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="ed524-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ed524-107">Methods</span></span>
|<span data-ttu-id="ed524-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ed524-108">Method</span></span>|<span data-ttu-id="ed524-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ed524-109">Return Type</span></span>|<span data-ttu-id="ed524-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ed524-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed524-111">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="ed524-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="ed524-112">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="ed524-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="ed524-113">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="ed524-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="ed524-114">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="ed524-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="ed524-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="ed524-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="ed524-116">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="ed524-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="ed524-117">действие назначения</span><span class="sxs-lookup"><span data-stu-id="ed524-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="ed524-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ed524-118">None</span></span>|<span data-ttu-id="ed524-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ed524-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ed524-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed524-120">Properties</span></span>
|<span data-ttu-id="ed524-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed524-121">Property</span></span>|<span data-ttu-id="ed524-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ed524-122">Type</span></span>|<span data-ttu-id="ed524-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ed524-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed524-124">id</span><span class="sxs-lookup"><span data-stu-id="ed524-124">id</span></span>|<span data-ttu-id="ed524-125">Строка</span><span class="sxs-lookup"><span data-stu-id="ed524-125">String</span></span>|<span data-ttu-id="ed524-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ed524-126">Key of the entity.</span></span>|
|<span data-ttu-id="ed524-127">displayName</span><span class="sxs-lookup"><span data-stu-id="ed524-127">displayName</span></span>|<span data-ttu-id="ed524-128">String</span><span class="sxs-lookup"><span data-stu-id="ed524-128">String</span></span>|<span data-ttu-id="ed524-129">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ed524-129">Name of the eBook.</span></span>|
|<span data-ttu-id="ed524-130">description</span><span class="sxs-lookup"><span data-stu-id="ed524-130">description</span></span>|<span data-ttu-id="ed524-131">String</span><span class="sxs-lookup"><span data-stu-id="ed524-131">String</span></span>|<span data-ttu-id="ed524-132">Описание.</span><span class="sxs-lookup"><span data-stu-id="ed524-132">Description.</span></span>|
|<span data-ttu-id="ed524-133">publisher</span><span class="sxs-lookup"><span data-stu-id="ed524-133">publisher</span></span>|<span data-ttu-id="ed524-134">String</span><span class="sxs-lookup"><span data-stu-id="ed524-134">String</span></span>|<span data-ttu-id="ed524-135">Издатель.</span><span class="sxs-lookup"><span data-stu-id="ed524-135">Publisher.</span></span>|
|<span data-ttu-id="ed524-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed524-136">publishedDateTime</span></span>|<span data-ttu-id="ed524-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed524-137">DateTimeOffset</span></span>|<span data-ttu-id="ed524-138">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ed524-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="ed524-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="ed524-139">largeCover</span></span>|[<span data-ttu-id="ed524-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ed524-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ed524-141">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="ed524-141">Book cover.</span></span>|
|<span data-ttu-id="ed524-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed524-142">createdDateTime</span></span>|<span data-ttu-id="ed524-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed524-143">DateTimeOffset</span></span>|<span data-ttu-id="ed524-144">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ed524-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="ed524-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed524-145">lastModifiedDateTime</span></span>|<span data-ttu-id="ed524-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed524-146">DateTimeOffset</span></span>|<span data-ttu-id="ed524-147">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ed524-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="ed524-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ed524-148">informationUrl</span></span>|<span data-ttu-id="ed524-149">String</span><span class="sxs-lookup"><span data-stu-id="ed524-149">String</span></span>|<span data-ttu-id="ed524-150">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ed524-150">The more information Url.</span></span>|
|<span data-ttu-id="ed524-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ed524-151">privacyInformationUrl</span></span>|<span data-ttu-id="ed524-152">String</span><span class="sxs-lookup"><span data-stu-id="ed524-152">String</span></span>|<span data-ttu-id="ed524-153">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ed524-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed524-154">Связи</span><span class="sxs-lookup"><span data-stu-id="ed524-154">Relationships</span></span>
|<span data-ttu-id="ed524-155">Отношение</span><span class="sxs-lookup"><span data-stu-id="ed524-155">Relationship</span></span>|<span data-ttu-id="ed524-156">Тип</span><span class="sxs-lookup"><span data-stu-id="ed524-156">Type</span></span>|<span data-ttu-id="ed524-157">Описание</span><span class="sxs-lookup"><span data-stu-id="ed524-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed524-158">categories</span><span class="sxs-lookup"><span data-stu-id="ed524-158">categories</span></span>|<span data-ttu-id="ed524-159">Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="ed524-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="ed524-160">Список категорий для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ed524-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="ed524-161">assignments</span><span class="sxs-lookup"><span data-stu-id="ed524-161">assignments</span></span>|<span data-ttu-id="ed524-162">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ed524-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="ed524-163">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ed524-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="ed524-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="ed524-164">installSummary</span></span>|[<span data-ttu-id="ed524-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ed524-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="ed524-166">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ed524-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="ed524-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="ed524-167">deviceStates</span></span>|<span data-ttu-id="ed524-168">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="ed524-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="ed524-169">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ed524-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="ed524-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="ed524-170">userStateSummary</span></span>|<span data-ttu-id="ed524-171">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="ed524-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="ed524-172">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ed524-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed524-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed524-173">JSON Representation</span></span>
<span data-ttu-id="ed524-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed524-174">Here is a JSON representation of the resource.</span></span>
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




