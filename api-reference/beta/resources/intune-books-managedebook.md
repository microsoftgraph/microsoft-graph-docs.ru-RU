---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
ms.openlocfilehash: 7370b685b40902552a44b5c041742f6d6a884e72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081340"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="241cf-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="241cf-103">managedEBook resource type</span></span>

> <span data-ttu-id="241cf-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="241cf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="241cf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="241cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="241cf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="241cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="241cf-107">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="241cf-107">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="241cf-108">Методы</span><span class="sxs-lookup"><span data-stu-id="241cf-108">Methods</span></span>
|<span data-ttu-id="241cf-109">Метод</span><span class="sxs-lookup"><span data-stu-id="241cf-109">Method</span></span>|<span data-ttu-id="241cf-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="241cf-110">Return Type</span></span>|<span data-ttu-id="241cf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="241cf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="241cf-112">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="241cf-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="241cf-113">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="241cf-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="241cf-114">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="241cf-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="241cf-115">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="241cf-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="241cf-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="241cf-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="241cf-117">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="241cf-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="241cf-118">действие назначения</span><span class="sxs-lookup"><span data-stu-id="241cf-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="241cf-119">Нет</span><span class="sxs-lookup"><span data-stu-id="241cf-119">None</span></span>|<span data-ttu-id="241cf-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="241cf-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="241cf-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="241cf-121">Properties</span></span>
|<span data-ttu-id="241cf-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="241cf-122">Property</span></span>|<span data-ttu-id="241cf-123">Тип</span><span class="sxs-lookup"><span data-stu-id="241cf-123">Type</span></span>|<span data-ttu-id="241cf-124">Описание</span><span class="sxs-lookup"><span data-stu-id="241cf-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="241cf-125">id</span><span class="sxs-lookup"><span data-stu-id="241cf-125">id</span></span>|<span data-ttu-id="241cf-126">String</span><span class="sxs-lookup"><span data-stu-id="241cf-126">String</span></span>|<span data-ttu-id="241cf-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="241cf-127">Key of the entity.</span></span>|
|<span data-ttu-id="241cf-128">displayName</span><span class="sxs-lookup"><span data-stu-id="241cf-128">displayName</span></span>|<span data-ttu-id="241cf-129">String</span><span class="sxs-lookup"><span data-stu-id="241cf-129">String</span></span>|<span data-ttu-id="241cf-130">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="241cf-130">Name of the eBook.</span></span>|
|<span data-ttu-id="241cf-131">описание</span><span class="sxs-lookup"><span data-stu-id="241cf-131">description</span></span>|<span data-ttu-id="241cf-132">String</span><span class="sxs-lookup"><span data-stu-id="241cf-132">String</span></span>|<span data-ttu-id="241cf-133">Описание.</span><span class="sxs-lookup"><span data-stu-id="241cf-133">Description.</span></span>|
|<span data-ttu-id="241cf-134">publisher</span><span class="sxs-lookup"><span data-stu-id="241cf-134">publisher</span></span>|<span data-ttu-id="241cf-135">String</span><span class="sxs-lookup"><span data-stu-id="241cf-135">String</span></span>|<span data-ttu-id="241cf-136">Издатель.</span><span class="sxs-lookup"><span data-stu-id="241cf-136">Publisher.</span></span>|
|<span data-ttu-id="241cf-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="241cf-137">publishedDateTime</span></span>|<span data-ttu-id="241cf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="241cf-138">DateTimeOffset</span></span>|<span data-ttu-id="241cf-139">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="241cf-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="241cf-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="241cf-140">largeCover</span></span>|[<span data-ttu-id="241cf-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="241cf-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="241cf-142">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="241cf-142">Book cover.</span></span>|
|<span data-ttu-id="241cf-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="241cf-143">createdDateTime</span></span>|<span data-ttu-id="241cf-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="241cf-144">DateTimeOffset</span></span>|<span data-ttu-id="241cf-145">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="241cf-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="241cf-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="241cf-146">lastModifiedDateTime</span></span>|<span data-ttu-id="241cf-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="241cf-147">DateTimeOffset</span></span>|<span data-ttu-id="241cf-148">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="241cf-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="241cf-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="241cf-149">informationUrl</span></span>|<span data-ttu-id="241cf-150">String</span><span class="sxs-lookup"><span data-stu-id="241cf-150">String</span></span>|<span data-ttu-id="241cf-151">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="241cf-151">The more information Url.</span></span>|
|<span data-ttu-id="241cf-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="241cf-152">privacyInformationUrl</span></span>|<span data-ttu-id="241cf-153">String</span><span class="sxs-lookup"><span data-stu-id="241cf-153">String</span></span>|<span data-ttu-id="241cf-154">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="241cf-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="241cf-155">Связи</span><span class="sxs-lookup"><span data-stu-id="241cf-155">Relationships</span></span>
|<span data-ttu-id="241cf-156">Связь</span><span class="sxs-lookup"><span data-stu-id="241cf-156">Relationship</span></span>|<span data-ttu-id="241cf-157">Тип</span><span class="sxs-lookup"><span data-stu-id="241cf-157">Type</span></span>|<span data-ttu-id="241cf-158">Описание</span><span class="sxs-lookup"><span data-stu-id="241cf-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="241cf-159">categories</span><span class="sxs-lookup"><span data-stu-id="241cf-159">categories</span></span>|<span data-ttu-id="241cf-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="241cf-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="241cf-161">Список категорий для этой книги.</span><span class="sxs-lookup"><span data-stu-id="241cf-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="241cf-162">assignments</span><span class="sxs-lookup"><span data-stu-id="241cf-162">assignments</span></span>|<span data-ttu-id="241cf-163">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="241cf-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="241cf-164">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="241cf-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="241cf-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="241cf-165">installSummary</span></span>|[<span data-ttu-id="241cf-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="241cf-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="241cf-167">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="241cf-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="241cf-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="241cf-168">deviceStates</span></span>|<span data-ttu-id="241cf-169">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="241cf-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="241cf-170">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="241cf-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="241cf-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="241cf-171">userStateSummary</span></span>|<span data-ttu-id="241cf-172">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="241cf-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="241cf-173">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="241cf-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="241cf-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="241cf-174">JSON Representation</span></span>
<span data-ttu-id="241cf-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="241cf-175">Here is a JSON representation of the resource.</span></span>
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





