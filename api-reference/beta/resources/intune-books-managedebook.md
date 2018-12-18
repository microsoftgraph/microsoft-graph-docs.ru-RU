---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: tfitzmac
ms.openlocfilehash: 7b826d7b0a11ce957a87154f276abc0e8168f45d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347147"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="5e991-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="5e991-103">managedEBook resource type</span></span>

> <span data-ttu-id="5e991-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e991-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e991-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e991-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e991-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5e991-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e991-107">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e991-107">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="5e991-108">Методы</span><span class="sxs-lookup"><span data-stu-id="5e991-108">Methods</span></span>
|<span data-ttu-id="5e991-109">Метод</span><span class="sxs-lookup"><span data-stu-id="5e991-109">Method</span></span>|<span data-ttu-id="5e991-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5e991-110">Return Type</span></span>|<span data-ttu-id="5e991-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5e991-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e991-112">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="5e991-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="5e991-113">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="5e991-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="5e991-114">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e991-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="5e991-115">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="5e991-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="5e991-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="5e991-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="5e991-117">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e991-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="5e991-118">действие назначения</span><span class="sxs-lookup"><span data-stu-id="5e991-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="5e991-119">Нет</span><span class="sxs-lookup"><span data-stu-id="5e991-119">None</span></span>|<span data-ttu-id="5e991-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5e991-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5e991-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e991-121">Properties</span></span>
|<span data-ttu-id="5e991-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e991-122">Property</span></span>|<span data-ttu-id="5e991-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5e991-123">Type</span></span>|<span data-ttu-id="5e991-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5e991-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e991-125">id</span><span class="sxs-lookup"><span data-stu-id="5e991-125">id</span></span>|<span data-ttu-id="5e991-126">Строка</span><span class="sxs-lookup"><span data-stu-id="5e991-126">String</span></span>|<span data-ttu-id="5e991-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5e991-127">Key of the entity.</span></span>|
|<span data-ttu-id="5e991-128">displayName</span><span class="sxs-lookup"><span data-stu-id="5e991-128">displayName</span></span>|<span data-ttu-id="5e991-129">String</span><span class="sxs-lookup"><span data-stu-id="5e991-129">String</span></span>|<span data-ttu-id="5e991-130">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e991-130">Name of the eBook.</span></span>|
|<span data-ttu-id="5e991-131">описание</span><span class="sxs-lookup"><span data-stu-id="5e991-131">description</span></span>|<span data-ttu-id="5e991-132">Строка</span><span class="sxs-lookup"><span data-stu-id="5e991-132">String</span></span>|<span data-ttu-id="5e991-133">Описание.</span><span class="sxs-lookup"><span data-stu-id="5e991-133">Description.</span></span>|
|<span data-ttu-id="5e991-134">publisher</span><span class="sxs-lookup"><span data-stu-id="5e991-134">publisher</span></span>|<span data-ttu-id="5e991-135">String</span><span class="sxs-lookup"><span data-stu-id="5e991-135">String</span></span>|<span data-ttu-id="5e991-136">Издатель.</span><span class="sxs-lookup"><span data-stu-id="5e991-136">Publisher.</span></span>|
|<span data-ttu-id="5e991-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e991-137">publishedDateTime</span></span>|<span data-ttu-id="5e991-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e991-138">DateTimeOffset</span></span>|<span data-ttu-id="5e991-139">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e991-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="5e991-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="5e991-140">largeCover</span></span>|[<span data-ttu-id="5e991-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5e991-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5e991-142">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="5e991-142">Book cover.</span></span>|
|<span data-ttu-id="5e991-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e991-143">createdDateTime</span></span>|<span data-ttu-id="5e991-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e991-144">DateTimeOffset</span></span>|<span data-ttu-id="5e991-145">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e991-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="5e991-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e991-146">lastModifiedDateTime</span></span>|<span data-ttu-id="5e991-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e991-147">DateTimeOffset</span></span>|<span data-ttu-id="5e991-148">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e991-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="5e991-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5e991-149">informationUrl</span></span>|<span data-ttu-id="5e991-150">String</span><span class="sxs-lookup"><span data-stu-id="5e991-150">String</span></span>|<span data-ttu-id="5e991-151">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5e991-151">The more information Url.</span></span>|
|<span data-ttu-id="5e991-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5e991-152">privacyInformationUrl</span></span>|<span data-ttu-id="5e991-153">String</span><span class="sxs-lookup"><span data-stu-id="5e991-153">String</span></span>|<span data-ttu-id="5e991-154">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5e991-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e991-155">Связи</span><span class="sxs-lookup"><span data-stu-id="5e991-155">Relationships</span></span>
|<span data-ttu-id="5e991-156">Связь</span><span class="sxs-lookup"><span data-stu-id="5e991-156">Relationship</span></span>|<span data-ttu-id="5e991-157">Тип</span><span class="sxs-lookup"><span data-stu-id="5e991-157">Type</span></span>|<span data-ttu-id="5e991-158">Описание</span><span class="sxs-lookup"><span data-stu-id="5e991-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e991-159">categories</span><span class="sxs-lookup"><span data-stu-id="5e991-159">categories</span></span>|<span data-ttu-id="5e991-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5e991-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="5e991-161">Список категорий для этой книги.</span><span class="sxs-lookup"><span data-stu-id="5e991-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="5e991-162">assignments</span><span class="sxs-lookup"><span data-stu-id="5e991-162">assignments</span></span>|<span data-ttu-id="5e991-163">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5e991-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="5e991-164">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e991-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="5e991-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="5e991-165">installSummary</span></span>|[<span data-ttu-id="5e991-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5e991-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="5e991-167">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="5e991-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="5e991-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="5e991-168">deviceStates</span></span>|<span data-ttu-id="5e991-169">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="5e991-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="5e991-170">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e991-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="5e991-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="5e991-171">userStateSummary</span></span>|<span data-ttu-id="5e991-172">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="5e991-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="5e991-173">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e991-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e991-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e991-174">JSON Representation</span></span>
<span data-ttu-id="5e991-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e991-175">Here is a JSON representation of the resource.</span></span>
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





