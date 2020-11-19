---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b399e84a0f714242f7213596dc1aea20a3eba9d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295273"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="8a0d3-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="8a0d3-103">managedEBook resource type</span></span>

<span data-ttu-id="8a0d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a0d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a0d3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a0d3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a0d3-107">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="8a0d3-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8a0d3-108">Methods</span></span>
|<span data-ttu-id="8a0d3-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8a0d3-109">Method</span></span>|<span data-ttu-id="8a0d3-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a0d3-110">Return Type</span></span>|<span data-ttu-id="8a0d3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8a0d3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8a0d3-112">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="8a0d3-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="8a0d3-113">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="8a0d3-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="8a0d3-114">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="8a0d3-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="8a0d3-115">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="8a0d3-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="8a0d3-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="8a0d3-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="8a0d3-117">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="8a0d3-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="8a0d3-118">действие назначения</span><span class="sxs-lookup"><span data-stu-id="8a0d3-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="8a0d3-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8a0d3-119">None</span></span>|<span data-ttu-id="8a0d3-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8a0d3-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8a0d3-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a0d3-121">Properties</span></span>
|<span data-ttu-id="8a0d3-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a0d3-122">Property</span></span>|<span data-ttu-id="8a0d3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8a0d3-123">Type</span></span>|<span data-ttu-id="8a0d3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8a0d3-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a0d3-125">id</span><span class="sxs-lookup"><span data-stu-id="8a0d3-125">id</span></span>|<span data-ttu-id="8a0d3-126">String</span><span class="sxs-lookup"><span data-stu-id="8a0d3-126">String</span></span>|<span data-ttu-id="8a0d3-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-127">Key of the entity.</span></span>|
|<span data-ttu-id="8a0d3-128">displayName</span><span class="sxs-lookup"><span data-stu-id="8a0d3-128">displayName</span></span>|<span data-ttu-id="8a0d3-129">String</span><span class="sxs-lookup"><span data-stu-id="8a0d3-129">String</span></span>|<span data-ttu-id="8a0d3-130">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-130">Name of the eBook.</span></span>|
|<span data-ttu-id="8a0d3-131">description</span><span class="sxs-lookup"><span data-stu-id="8a0d3-131">description</span></span>|<span data-ttu-id="8a0d3-132">String</span><span class="sxs-lookup"><span data-stu-id="8a0d3-132">String</span></span>|<span data-ttu-id="8a0d3-133">Описание.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-133">Description.</span></span>|
|<span data-ttu-id="8a0d3-134">publisher</span><span class="sxs-lookup"><span data-stu-id="8a0d3-134">publisher</span></span>|<span data-ttu-id="8a0d3-135">String</span><span class="sxs-lookup"><span data-stu-id="8a0d3-135">String</span></span>|<span data-ttu-id="8a0d3-136">Издатель.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-136">Publisher.</span></span>|
|<span data-ttu-id="8a0d3-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a0d3-137">publishedDateTime</span></span>|<span data-ttu-id="8a0d3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a0d3-138">DateTimeOffset</span></span>|<span data-ttu-id="8a0d3-139">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="8a0d3-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="8a0d3-140">largeCover</span></span>|[<span data-ttu-id="8a0d3-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8a0d3-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8a0d3-142">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-142">Book cover.</span></span>|
|<span data-ttu-id="8a0d3-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a0d3-143">createdDateTime</span></span>|<span data-ttu-id="8a0d3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a0d3-144">DateTimeOffset</span></span>|<span data-ttu-id="8a0d3-145">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="8a0d3-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a0d3-146">lastModifiedDateTime</span></span>|<span data-ttu-id="8a0d3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a0d3-147">DateTimeOffset</span></span>|<span data-ttu-id="8a0d3-148">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="8a0d3-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8a0d3-149">informationUrl</span></span>|<span data-ttu-id="8a0d3-150">String</span><span class="sxs-lookup"><span data-stu-id="8a0d3-150">String</span></span>|<span data-ttu-id="8a0d3-151">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-151">The more information Url.</span></span>|
|<span data-ttu-id="8a0d3-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8a0d3-152">privacyInformationUrl</span></span>|<span data-ttu-id="8a0d3-153">String</span><span class="sxs-lookup"><span data-stu-id="8a0d3-153">String</span></span>|<span data-ttu-id="8a0d3-154">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a0d3-155">Связи</span><span class="sxs-lookup"><span data-stu-id="8a0d3-155">Relationships</span></span>
|<span data-ttu-id="8a0d3-156">Связь</span><span class="sxs-lookup"><span data-stu-id="8a0d3-156">Relationship</span></span>|<span data-ttu-id="8a0d3-157">Тип</span><span class="sxs-lookup"><span data-stu-id="8a0d3-157">Type</span></span>|<span data-ttu-id="8a0d3-158">Описание</span><span class="sxs-lookup"><span data-stu-id="8a0d3-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a0d3-159">categories</span><span class="sxs-lookup"><span data-stu-id="8a0d3-159">categories</span></span>|<span data-ttu-id="8a0d3-160">Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="8a0d3-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="8a0d3-161">Список категорий для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="8a0d3-162">assignments</span><span class="sxs-lookup"><span data-stu-id="8a0d3-162">assignments</span></span>|<span data-ttu-id="8a0d3-163">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8a0d3-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="8a0d3-164">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="8a0d3-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="8a0d3-165">installSummary</span></span>|[<span data-ttu-id="8a0d3-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="8a0d3-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="8a0d3-167">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="8a0d3-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="8a0d3-168">deviceStates</span></span>|<span data-ttu-id="8a0d3-169">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="8a0d3-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="8a0d3-170">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="8a0d3-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="8a0d3-171">userStateSummary</span></span>|<span data-ttu-id="8a0d3-172">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="8a0d3-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="8a0d3-173">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a0d3-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a0d3-174">JSON Representation</span></span>
<span data-ttu-id="8a0d3-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a0d3-175">Here is a JSON representation of the resource.</span></span>
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




