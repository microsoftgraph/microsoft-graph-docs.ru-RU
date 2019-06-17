---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8bf13e2c0a5c8e55a397516c21fe91d65aa413a5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991655"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="eea19-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="eea19-103">managedEBook resource type</span></span>

> <span data-ttu-id="eea19-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eea19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eea19-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eea19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eea19-106">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="eea19-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="eea19-107">Методы</span><span class="sxs-lookup"><span data-stu-id="eea19-107">Methods</span></span>
|<span data-ttu-id="eea19-108">Метод</span><span class="sxs-lookup"><span data-stu-id="eea19-108">Method</span></span>|<span data-ttu-id="eea19-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eea19-109">Return Type</span></span>|<span data-ttu-id="eea19-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eea19-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eea19-111">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="eea19-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="eea19-112">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="eea19-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="eea19-113">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="eea19-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="eea19-114">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="eea19-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="eea19-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="eea19-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="eea19-116">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="eea19-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="eea19-117">действие назначения</span><span class="sxs-lookup"><span data-stu-id="eea19-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="eea19-118">Нет</span><span class="sxs-lookup"><span data-stu-id="eea19-118">None</span></span>|<span data-ttu-id="eea19-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="eea19-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="eea19-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="eea19-120">Properties</span></span>
|<span data-ttu-id="eea19-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="eea19-121">Property</span></span>|<span data-ttu-id="eea19-122">Тип</span><span class="sxs-lookup"><span data-stu-id="eea19-122">Type</span></span>|<span data-ttu-id="eea19-123">Описание</span><span class="sxs-lookup"><span data-stu-id="eea19-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eea19-124">id</span><span class="sxs-lookup"><span data-stu-id="eea19-124">id</span></span>|<span data-ttu-id="eea19-125">Строка</span><span class="sxs-lookup"><span data-stu-id="eea19-125">String</span></span>|<span data-ttu-id="eea19-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eea19-126">Key of the entity.</span></span>|
|<span data-ttu-id="eea19-127">displayName</span><span class="sxs-lookup"><span data-stu-id="eea19-127">displayName</span></span>|<span data-ttu-id="eea19-128">Строка</span><span class="sxs-lookup"><span data-stu-id="eea19-128">String</span></span>|<span data-ttu-id="eea19-129">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="eea19-129">Name of the eBook.</span></span>|
|<span data-ttu-id="eea19-130">description</span><span class="sxs-lookup"><span data-stu-id="eea19-130">description</span></span>|<span data-ttu-id="eea19-131">String</span><span class="sxs-lookup"><span data-stu-id="eea19-131">String</span></span>|<span data-ttu-id="eea19-132">Описание.</span><span class="sxs-lookup"><span data-stu-id="eea19-132">Description.</span></span>|
|<span data-ttu-id="eea19-133">publisher</span><span class="sxs-lookup"><span data-stu-id="eea19-133">publisher</span></span>|<span data-ttu-id="eea19-134">String</span><span class="sxs-lookup"><span data-stu-id="eea19-134">String</span></span>|<span data-ttu-id="eea19-135">Издатель.</span><span class="sxs-lookup"><span data-stu-id="eea19-135">Publisher.</span></span>|
|<span data-ttu-id="eea19-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="eea19-136">publishedDateTime</span></span>|<span data-ttu-id="eea19-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eea19-137">DateTimeOffset</span></span>|<span data-ttu-id="eea19-138">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="eea19-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="eea19-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="eea19-139">largeCover</span></span>|[<span data-ttu-id="eea19-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eea19-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eea19-141">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="eea19-141">Book cover.</span></span>|
|<span data-ttu-id="eea19-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eea19-142">createdDateTime</span></span>|<span data-ttu-id="eea19-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eea19-143">DateTimeOffset</span></span>|<span data-ttu-id="eea19-144">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="eea19-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="eea19-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eea19-145">lastModifiedDateTime</span></span>|<span data-ttu-id="eea19-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eea19-146">DateTimeOffset</span></span>|<span data-ttu-id="eea19-147">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="eea19-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="eea19-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eea19-148">informationUrl</span></span>|<span data-ttu-id="eea19-149">String</span><span class="sxs-lookup"><span data-stu-id="eea19-149">String</span></span>|<span data-ttu-id="eea19-150">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="eea19-150">The more information Url.</span></span>|
|<span data-ttu-id="eea19-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eea19-151">privacyInformationUrl</span></span>|<span data-ttu-id="eea19-152">String</span><span class="sxs-lookup"><span data-stu-id="eea19-152">String</span></span>|<span data-ttu-id="eea19-153">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="eea19-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eea19-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="eea19-154">Relationships</span></span>
|<span data-ttu-id="eea19-155">Отношение</span><span class="sxs-lookup"><span data-stu-id="eea19-155">Relationship</span></span>|<span data-ttu-id="eea19-156">Тип</span><span class="sxs-lookup"><span data-stu-id="eea19-156">Type</span></span>|<span data-ttu-id="eea19-157">Описание</span><span class="sxs-lookup"><span data-stu-id="eea19-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eea19-158">categories</span><span class="sxs-lookup"><span data-stu-id="eea19-158">categories</span></span>|<span data-ttu-id="eea19-159">Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="eea19-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="eea19-160">Список категорий для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="eea19-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="eea19-161">assignments</span><span class="sxs-lookup"><span data-stu-id="eea19-161">assignments</span></span>|<span data-ttu-id="eea19-162">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eea19-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="eea19-163">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="eea19-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="eea19-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="eea19-164">installSummary</span></span>|[<span data-ttu-id="eea19-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="eea19-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="eea19-166">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="eea19-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="eea19-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="eea19-167">deviceStates</span></span>|<span data-ttu-id="eea19-168">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="eea19-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="eea19-169">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="eea19-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="eea19-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="eea19-170">userStateSummary</span></span>|<span data-ttu-id="eea19-171">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="eea19-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="eea19-172">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="eea19-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eea19-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eea19-173">JSON Representation</span></span>
<span data-ttu-id="eea19-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eea19-174">Here is a JSON representation of the resource.</span></span>
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





