---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f3bcbd777c87150103fe21495370adddf3afe90
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43403016"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="6b22b-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="6b22b-103">managedEBook resource type</span></span>

<span data-ttu-id="6b22b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b22b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b22b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b22b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b22b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b22b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b22b-107">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="6b22b-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="6b22b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6b22b-108">Methods</span></span>
|<span data-ttu-id="6b22b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6b22b-109">Method</span></span>|<span data-ttu-id="6b22b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6b22b-110">Return Type</span></span>|<span data-ttu-id="6b22b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6b22b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6b22b-112">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="6b22b-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="6b22b-113">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="6b22b-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="6b22b-114">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="6b22b-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="6b22b-115">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="6b22b-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="6b22b-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="6b22b-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="6b22b-117">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="6b22b-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="6b22b-118">действие назначения</span><span class="sxs-lookup"><span data-stu-id="6b22b-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="6b22b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6b22b-119">None</span></span>|<span data-ttu-id="6b22b-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6b22b-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6b22b-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b22b-121">Properties</span></span>
|<span data-ttu-id="6b22b-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b22b-122">Property</span></span>|<span data-ttu-id="6b22b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6b22b-123">Type</span></span>|<span data-ttu-id="6b22b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6b22b-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b22b-125">id</span><span class="sxs-lookup"><span data-stu-id="6b22b-125">id</span></span>|<span data-ttu-id="6b22b-126">Строка</span><span class="sxs-lookup"><span data-stu-id="6b22b-126">String</span></span>|<span data-ttu-id="6b22b-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6b22b-127">Key of the entity.</span></span>|
|<span data-ttu-id="6b22b-128">displayName</span><span class="sxs-lookup"><span data-stu-id="6b22b-128">displayName</span></span>|<span data-ttu-id="6b22b-129">Строка</span><span class="sxs-lookup"><span data-stu-id="6b22b-129">String</span></span>|<span data-ttu-id="6b22b-130">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="6b22b-130">Name of the eBook.</span></span>|
|<span data-ttu-id="6b22b-131">description</span><span class="sxs-lookup"><span data-stu-id="6b22b-131">description</span></span>|<span data-ttu-id="6b22b-132">String</span><span class="sxs-lookup"><span data-stu-id="6b22b-132">String</span></span>|<span data-ttu-id="6b22b-133">Описание.</span><span class="sxs-lookup"><span data-stu-id="6b22b-133">Description.</span></span>|
|<span data-ttu-id="6b22b-134">publisher</span><span class="sxs-lookup"><span data-stu-id="6b22b-134">publisher</span></span>|<span data-ttu-id="6b22b-135">String</span><span class="sxs-lookup"><span data-stu-id="6b22b-135">String</span></span>|<span data-ttu-id="6b22b-136">Издатель.</span><span class="sxs-lookup"><span data-stu-id="6b22b-136">Publisher.</span></span>|
|<span data-ttu-id="6b22b-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b22b-137">publishedDateTime</span></span>|<span data-ttu-id="6b22b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b22b-138">DateTimeOffset</span></span>|<span data-ttu-id="6b22b-139">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="6b22b-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="6b22b-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="6b22b-140">largeCover</span></span>|[<span data-ttu-id="6b22b-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6b22b-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6b22b-142">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="6b22b-142">Book cover.</span></span>|
|<span data-ttu-id="6b22b-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b22b-143">createdDateTime</span></span>|<span data-ttu-id="6b22b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b22b-144">DateTimeOffset</span></span>|<span data-ttu-id="6b22b-145">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="6b22b-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="6b22b-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b22b-146">lastModifiedDateTime</span></span>|<span data-ttu-id="6b22b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b22b-147">DateTimeOffset</span></span>|<span data-ttu-id="6b22b-148">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="6b22b-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="6b22b-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6b22b-149">informationUrl</span></span>|<span data-ttu-id="6b22b-150">String</span><span class="sxs-lookup"><span data-stu-id="6b22b-150">String</span></span>|<span data-ttu-id="6b22b-151">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="6b22b-151">The more information Url.</span></span>|
|<span data-ttu-id="6b22b-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6b22b-152">privacyInformationUrl</span></span>|<span data-ttu-id="6b22b-153">String</span><span class="sxs-lookup"><span data-stu-id="6b22b-153">String</span></span>|<span data-ttu-id="6b22b-154">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="6b22b-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b22b-155">Связи</span><span class="sxs-lookup"><span data-stu-id="6b22b-155">Relationships</span></span>
|<span data-ttu-id="6b22b-156">Связь</span><span class="sxs-lookup"><span data-stu-id="6b22b-156">Relationship</span></span>|<span data-ttu-id="6b22b-157">Тип</span><span class="sxs-lookup"><span data-stu-id="6b22b-157">Type</span></span>|<span data-ttu-id="6b22b-158">Описание</span><span class="sxs-lookup"><span data-stu-id="6b22b-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b22b-159">categories</span><span class="sxs-lookup"><span data-stu-id="6b22b-159">categories</span></span>|<span data-ttu-id="6b22b-160">Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="6b22b-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="6b22b-161">Список категорий для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="6b22b-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="6b22b-162">assignments</span><span class="sxs-lookup"><span data-stu-id="6b22b-162">assignments</span></span>|<span data-ttu-id="6b22b-163">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6b22b-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="6b22b-164">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="6b22b-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="6b22b-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="6b22b-165">installSummary</span></span>|[<span data-ttu-id="6b22b-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6b22b-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="6b22b-167">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="6b22b-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="6b22b-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="6b22b-168">deviceStates</span></span>|<span data-ttu-id="6b22b-169">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="6b22b-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="6b22b-170">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="6b22b-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="6b22b-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="6b22b-171">userStateSummary</span></span>|<span data-ttu-id="6b22b-172">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="6b22b-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="6b22b-173">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="6b22b-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b22b-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b22b-174">JSON Representation</span></span>
<span data-ttu-id="6b22b-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b22b-175">Here is a JSON representation of the resource.</span></span>
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



