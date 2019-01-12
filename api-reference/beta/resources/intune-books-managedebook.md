---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6fd4fd3caef3aab90257805a48e53bee9c6b8764
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962599"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="f5459-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="f5459-103">managedEBook resource type</span></span>

> <span data-ttu-id="f5459-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f5459-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5459-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5459-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5459-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f5459-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5459-107">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f5459-107">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="f5459-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f5459-108">Methods</span></span>
|<span data-ttu-id="f5459-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f5459-109">Method</span></span>|<span data-ttu-id="f5459-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f5459-110">Return Type</span></span>|<span data-ttu-id="f5459-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f5459-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f5459-112">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="f5459-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="f5459-113">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="f5459-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="f5459-114">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f5459-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="f5459-115">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="f5459-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="f5459-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="f5459-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="f5459-117">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="f5459-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="f5459-118">действие назначения</span><span class="sxs-lookup"><span data-stu-id="f5459-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="f5459-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f5459-119">None</span></span>|<span data-ttu-id="f5459-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f5459-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f5459-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5459-121">Properties</span></span>
|<span data-ttu-id="f5459-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5459-122">Property</span></span>|<span data-ttu-id="f5459-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f5459-123">Type</span></span>|<span data-ttu-id="f5459-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f5459-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5459-125">id</span><span class="sxs-lookup"><span data-stu-id="f5459-125">id</span></span>|<span data-ttu-id="f5459-126">String</span><span class="sxs-lookup"><span data-stu-id="f5459-126">String</span></span>|<span data-ttu-id="f5459-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f5459-127">Key of the entity.</span></span>|
|<span data-ttu-id="f5459-128">displayName</span><span class="sxs-lookup"><span data-stu-id="f5459-128">displayName</span></span>|<span data-ttu-id="f5459-129">String</span><span class="sxs-lookup"><span data-stu-id="f5459-129">String</span></span>|<span data-ttu-id="f5459-130">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f5459-130">Name of the eBook.</span></span>|
|<span data-ttu-id="f5459-131">описание</span><span class="sxs-lookup"><span data-stu-id="f5459-131">description</span></span>|<span data-ttu-id="f5459-132">String</span><span class="sxs-lookup"><span data-stu-id="f5459-132">String</span></span>|<span data-ttu-id="f5459-133">Описание.</span><span class="sxs-lookup"><span data-stu-id="f5459-133">Description.</span></span>|
|<span data-ttu-id="f5459-134">publisher</span><span class="sxs-lookup"><span data-stu-id="f5459-134">publisher</span></span>|<span data-ttu-id="f5459-135">String</span><span class="sxs-lookup"><span data-stu-id="f5459-135">String</span></span>|<span data-ttu-id="f5459-136">Издатель.</span><span class="sxs-lookup"><span data-stu-id="f5459-136">Publisher.</span></span>|
|<span data-ttu-id="f5459-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5459-137">publishedDateTime</span></span>|<span data-ttu-id="f5459-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5459-138">DateTimeOffset</span></span>|<span data-ttu-id="f5459-139">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f5459-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="f5459-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="f5459-140">largeCover</span></span>|[<span data-ttu-id="f5459-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f5459-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f5459-142">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="f5459-142">Book cover.</span></span>|
|<span data-ttu-id="f5459-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5459-143">createdDateTime</span></span>|<span data-ttu-id="f5459-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5459-144">DateTimeOffset</span></span>|<span data-ttu-id="f5459-145">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f5459-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="f5459-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5459-146">lastModifiedDateTime</span></span>|<span data-ttu-id="f5459-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5459-147">DateTimeOffset</span></span>|<span data-ttu-id="f5459-148">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f5459-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="f5459-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f5459-149">informationUrl</span></span>|<span data-ttu-id="f5459-150">String</span><span class="sxs-lookup"><span data-stu-id="f5459-150">String</span></span>|<span data-ttu-id="f5459-151">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f5459-151">The more information Url.</span></span>|
|<span data-ttu-id="f5459-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f5459-152">privacyInformationUrl</span></span>|<span data-ttu-id="f5459-153">String</span><span class="sxs-lookup"><span data-stu-id="f5459-153">String</span></span>|<span data-ttu-id="f5459-154">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f5459-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5459-155">Связи</span><span class="sxs-lookup"><span data-stu-id="f5459-155">Relationships</span></span>
|<span data-ttu-id="f5459-156">Связь</span><span class="sxs-lookup"><span data-stu-id="f5459-156">Relationship</span></span>|<span data-ttu-id="f5459-157">Тип</span><span class="sxs-lookup"><span data-stu-id="f5459-157">Type</span></span>|<span data-ttu-id="f5459-158">Описание</span><span class="sxs-lookup"><span data-stu-id="f5459-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5459-159">categories</span><span class="sxs-lookup"><span data-stu-id="f5459-159">categories</span></span>|<span data-ttu-id="f5459-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f5459-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="f5459-161">Список категорий для этой книги.</span><span class="sxs-lookup"><span data-stu-id="f5459-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="f5459-162">assignments</span><span class="sxs-lookup"><span data-stu-id="f5459-162">assignments</span></span>|<span data-ttu-id="f5459-163">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f5459-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="f5459-164">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f5459-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="f5459-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="f5459-165">installSummary</span></span>|[<span data-ttu-id="f5459-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f5459-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="f5459-167">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f5459-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="f5459-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="f5459-168">deviceStates</span></span>|<span data-ttu-id="f5459-169">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="f5459-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="f5459-170">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f5459-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="f5459-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="f5459-171">userStateSummary</span></span>|<span data-ttu-id="f5459-172">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="f5459-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="f5459-173">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="f5459-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5459-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5459-174">JSON Representation</span></span>
<span data-ttu-id="f5459-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5459-175">Here is a JSON representation of the resource.</span></span>
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





