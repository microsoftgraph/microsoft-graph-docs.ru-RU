---
title: Тип ресурса managedEBook
description: Абстрактный класс, содержащий базовые свойства управляемой электронной книги.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d303932765976cc8828fef5b256a7f7cf8e26482
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691486"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="9ac5f-103">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="9ac5f-103">managedEBook resource type</span></span>

<span data-ttu-id="9ac5f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ac5f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ac5f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ac5f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ac5f-107">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="9ac5f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9ac5f-108">Methods</span></span>
|<span data-ttu-id="9ac5f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9ac5f-109">Method</span></span>|<span data-ttu-id="9ac5f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9ac5f-110">Return Type</span></span>|<span data-ttu-id="9ac5f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9ac5f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ac5f-112">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="9ac5f-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="9ac5f-113">Коллекция [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="9ac5f-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="9ac5f-114">Список свойств и связей объектов [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="9ac5f-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="9ac5f-115">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="9ac5f-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="9ac5f-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="9ac5f-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="9ac5f-117">Чтение свойств и связей объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="9ac5f-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="9ac5f-118">действие назначения</span><span class="sxs-lookup"><span data-stu-id="9ac5f-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="9ac5f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="9ac5f-119">None</span></span>|<span data-ttu-id="9ac5f-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9ac5f-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9ac5f-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ac5f-121">Properties</span></span>
|<span data-ttu-id="9ac5f-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ac5f-122">Property</span></span>|<span data-ttu-id="9ac5f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9ac5f-123">Type</span></span>|<span data-ttu-id="9ac5f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9ac5f-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ac5f-125">id</span><span class="sxs-lookup"><span data-stu-id="9ac5f-125">id</span></span>|<span data-ttu-id="9ac5f-126">Строка</span><span class="sxs-lookup"><span data-stu-id="9ac5f-126">String</span></span>|<span data-ttu-id="9ac5f-127">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-127">Key of the entity.</span></span>|
|<span data-ttu-id="9ac5f-128">displayName</span><span class="sxs-lookup"><span data-stu-id="9ac5f-128">displayName</span></span>|<span data-ttu-id="9ac5f-129">Строка</span><span class="sxs-lookup"><span data-stu-id="9ac5f-129">String</span></span>|<span data-ttu-id="9ac5f-130">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-130">Name of the eBook.</span></span>|
|<span data-ttu-id="9ac5f-131">description</span><span class="sxs-lookup"><span data-stu-id="9ac5f-131">description</span></span>|<span data-ttu-id="9ac5f-132">Строка</span><span class="sxs-lookup"><span data-stu-id="9ac5f-132">String</span></span>|<span data-ttu-id="9ac5f-133">Описание.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-133">Description.</span></span>|
|<span data-ttu-id="9ac5f-134">publisher</span><span class="sxs-lookup"><span data-stu-id="9ac5f-134">publisher</span></span>|<span data-ttu-id="9ac5f-135">String</span><span class="sxs-lookup"><span data-stu-id="9ac5f-135">String</span></span>|<span data-ttu-id="9ac5f-136">Издатель.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-136">Publisher.</span></span>|
|<span data-ttu-id="9ac5f-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac5f-137">publishedDateTime</span></span>|<span data-ttu-id="9ac5f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac5f-138">DateTimeOffset</span></span>|<span data-ttu-id="9ac5f-139">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="9ac5f-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="9ac5f-140">largeCover</span></span>|[<span data-ttu-id="9ac5f-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ac5f-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9ac5f-142">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-142">Book cover.</span></span>|
|<span data-ttu-id="9ac5f-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac5f-143">createdDateTime</span></span>|<span data-ttu-id="9ac5f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac5f-144">DateTimeOffset</span></span>|<span data-ttu-id="9ac5f-145">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="9ac5f-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac5f-146">lastModifiedDateTime</span></span>|<span data-ttu-id="9ac5f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac5f-147">DateTimeOffset</span></span>|<span data-ttu-id="9ac5f-148">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="9ac5f-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9ac5f-149">informationUrl</span></span>|<span data-ttu-id="9ac5f-150">String</span><span class="sxs-lookup"><span data-stu-id="9ac5f-150">String</span></span>|<span data-ttu-id="9ac5f-151">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-151">The more information Url.</span></span>|
|<span data-ttu-id="9ac5f-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9ac5f-152">privacyInformationUrl</span></span>|<span data-ttu-id="9ac5f-153">String</span><span class="sxs-lookup"><span data-stu-id="9ac5f-153">String</span></span>|<span data-ttu-id="9ac5f-154">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ac5f-155">Связи</span><span class="sxs-lookup"><span data-stu-id="9ac5f-155">Relationships</span></span>
|<span data-ttu-id="9ac5f-156">Связь</span><span class="sxs-lookup"><span data-stu-id="9ac5f-156">Relationship</span></span>|<span data-ttu-id="9ac5f-157">Тип</span><span class="sxs-lookup"><span data-stu-id="9ac5f-157">Type</span></span>|<span data-ttu-id="9ac5f-158">Описание</span><span class="sxs-lookup"><span data-stu-id="9ac5f-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ac5f-159">categories</span><span class="sxs-lookup"><span data-stu-id="9ac5f-159">categories</span></span>|<span data-ttu-id="9ac5f-160">Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)</span><span class="sxs-lookup"><span data-stu-id="9ac5f-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="9ac5f-161">Список категорий для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="9ac5f-162">assignments</span><span class="sxs-lookup"><span data-stu-id="9ac5f-162">assignments</span></span>|<span data-ttu-id="9ac5f-163">Коллекция [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9ac5f-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="9ac5f-164">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="9ac5f-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="9ac5f-165">installSummary</span></span>|[<span data-ttu-id="9ac5f-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9ac5f-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="9ac5f-167">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="9ac5f-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="9ac5f-168">deviceStates</span></span>|<span data-ttu-id="9ac5f-169">Коллекция [deviceInstallState](../resources/intune-books-deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="9ac5f-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="9ac5f-170">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="9ac5f-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="9ac5f-171">userStateSummary</span></span>|<span data-ttu-id="9ac5f-172">Коллекция [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="9ac5f-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="9ac5f-173">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ac5f-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ac5f-174">JSON Representation</span></span>
<span data-ttu-id="9ac5f-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ac5f-175">Here is a JSON representation of the resource.</span></span>
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





