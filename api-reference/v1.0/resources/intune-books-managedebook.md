---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae6151c23bf05b076ade441f908a2810c80f45ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534362"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="cd61c-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="cd61c-103">managedEBook resource type</span></span>

> <span data-ttu-id="cd61c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd61c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd61c-105">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cd61c-105">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="cd61c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cd61c-106">Methods</span></span>
|<span data-ttu-id="cd61c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cd61c-107">Method</span></span>|<span data-ttu-id="cd61c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cd61c-108">Return Type</span></span>|<span data-ttu-id="cd61c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cd61c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cd61c-110">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="cd61c-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="cd61c-111">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="cd61c-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="cd61c-112">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cd61c-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="cd61c-113">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="cd61c-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="cd61c-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="cd61c-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="cd61c-115">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="cd61c-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="cd61c-116">действие назначения</span><span class="sxs-lookup"><span data-stu-id="cd61c-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="cd61c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="cd61c-117">None</span></span>|<span data-ttu-id="cd61c-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cd61c-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cd61c-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd61c-119">Properties</span></span>
|<span data-ttu-id="cd61c-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd61c-120">Property</span></span>|<span data-ttu-id="cd61c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="cd61c-121">Type</span></span>|<span data-ttu-id="cd61c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cd61c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd61c-123">id</span><span class="sxs-lookup"><span data-stu-id="cd61c-123">id</span></span>|<span data-ttu-id="cd61c-124">Строка</span><span class="sxs-lookup"><span data-stu-id="cd61c-124">String</span></span>|<span data-ttu-id="cd61c-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cd61c-125">Key of the entity.</span></span>|
|<span data-ttu-id="cd61c-126">displayName</span><span class="sxs-lookup"><span data-stu-id="cd61c-126">displayName</span></span>|<span data-ttu-id="cd61c-127">Строка</span><span class="sxs-lookup"><span data-stu-id="cd61c-127">String</span></span>|<span data-ttu-id="cd61c-128">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cd61c-128">Name of the eBook.</span></span>|
|<span data-ttu-id="cd61c-129">description</span><span class="sxs-lookup"><span data-stu-id="cd61c-129">description</span></span>|<span data-ttu-id="cd61c-130">String</span><span class="sxs-lookup"><span data-stu-id="cd61c-130">String</span></span>|<span data-ttu-id="cd61c-131">Описание.</span><span class="sxs-lookup"><span data-stu-id="cd61c-131">Description.</span></span>|
|<span data-ttu-id="cd61c-132">publisher</span><span class="sxs-lookup"><span data-stu-id="cd61c-132">publisher</span></span>|<span data-ttu-id="cd61c-133">String</span><span class="sxs-lookup"><span data-stu-id="cd61c-133">String</span></span>|<span data-ttu-id="cd61c-134">Издатель.</span><span class="sxs-lookup"><span data-stu-id="cd61c-134">Publisher.</span></span>|
|<span data-ttu-id="cd61c-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd61c-135">publishedDateTime</span></span>|<span data-ttu-id="cd61c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd61c-136">DateTimeOffset</span></span>|<span data-ttu-id="cd61c-137">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cd61c-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="cd61c-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="cd61c-138">largeCover</span></span>|[<span data-ttu-id="cd61c-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cd61c-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cd61c-140">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="cd61c-140">Book cover.</span></span>|
|<span data-ttu-id="cd61c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd61c-141">createdDateTime</span></span>|<span data-ttu-id="cd61c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd61c-142">DateTimeOffset</span></span>|<span data-ttu-id="cd61c-143">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cd61c-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="cd61c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd61c-144">lastModifiedDateTime</span></span>|<span data-ttu-id="cd61c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd61c-145">DateTimeOffset</span></span>|<span data-ttu-id="cd61c-146">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cd61c-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="cd61c-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cd61c-147">informationUrl</span></span>|<span data-ttu-id="cd61c-148">String</span><span class="sxs-lookup"><span data-stu-id="cd61c-148">String</span></span>|<span data-ttu-id="cd61c-149">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="cd61c-149">The more information Url.</span></span>|
|<span data-ttu-id="cd61c-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cd61c-150">privacyInformationUrl</span></span>|<span data-ttu-id="cd61c-151">String</span><span class="sxs-lookup"><span data-stu-id="cd61c-151">String</span></span>|<span data-ttu-id="cd61c-152">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cd61c-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd61c-153">Связи</span><span class="sxs-lookup"><span data-stu-id="cd61c-153">Relationships</span></span>
|<span data-ttu-id="cd61c-154">Отношение</span><span class="sxs-lookup"><span data-stu-id="cd61c-154">Relationship</span></span>|<span data-ttu-id="cd61c-155">Тип</span><span class="sxs-lookup"><span data-stu-id="cd61c-155">Type</span></span>|<span data-ttu-id="cd61c-156">Описание</span><span class="sxs-lookup"><span data-stu-id="cd61c-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd61c-157">assignments</span><span class="sxs-lookup"><span data-stu-id="cd61c-157">assignments</span></span>|<span data-ttu-id="cd61c-158">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cd61c-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="cd61c-159">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cd61c-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="cd61c-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="cd61c-160">installSummary</span></span>|[<span data-ttu-id="cd61c-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="cd61c-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="cd61c-162">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="cd61c-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="cd61c-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="cd61c-163">deviceStates</span></span>|<span data-ttu-id="cd61c-164">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="cd61c-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="cd61c-165">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cd61c-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="cd61c-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="cd61c-166">userStateSummary</span></span>|<span data-ttu-id="cd61c-167">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="cd61c-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="cd61c-168">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="cd61c-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd61c-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd61c-169">JSON Representation</span></span>
<span data-ttu-id="cd61c-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd61c-170">Here is a JSON representation of the resource.</span></span>
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



