---
title: Тип ресурса mobileApp
description: Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1682c08e4fb15de6e5fc9d66d86d83c832e4c27
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752422"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="e6732-103">Тип ресурса mobileApp</span><span class="sxs-lookup"><span data-stu-id="e6732-103">mobileApp resource type</span></span>

<span data-ttu-id="e6732-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6732-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6732-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6732-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6732-106">Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="e6732-106">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="e6732-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e6732-107">Methods</span></span>
|<span data-ttu-id="e6732-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e6732-108">Method</span></span>|<span data-ttu-id="e6732-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e6732-109">Return Type</span></span>|<span data-ttu-id="e6732-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e6732-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6732-111">Список mobileApps</span><span class="sxs-lookup"><span data-stu-id="e6732-111">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="e6732-112">Коллекция [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e6732-112">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="e6732-113">Список свойств и связей объектов [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e6732-113">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="e6732-114">Получение объекта mobileApp</span><span class="sxs-lookup"><span data-stu-id="e6732-114">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="e6732-115">mobileApp</span><span class="sxs-lookup"><span data-stu-id="e6732-115">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="e6732-116">Чтение свойств и связей объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e6732-116">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="e6732-117">assign action</span><span class="sxs-lookup"><span data-stu-id="e6732-117">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="e6732-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e6732-118">None</span></span>|<span data-ttu-id="e6732-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e6732-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e6732-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6732-120">Properties</span></span>
|<span data-ttu-id="e6732-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6732-121">Property</span></span>|<span data-ttu-id="e6732-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e6732-122">Type</span></span>|<span data-ttu-id="e6732-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e6732-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6732-124">id</span><span class="sxs-lookup"><span data-stu-id="e6732-124">id</span></span>|<span data-ttu-id="e6732-125">String</span><span class="sxs-lookup"><span data-stu-id="e6732-125">String</span></span>|<span data-ttu-id="e6732-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e6732-126">Key of the entity.</span></span>|
|<span data-ttu-id="e6732-127">displayName</span><span class="sxs-lookup"><span data-stu-id="e6732-127">displayName</span></span>|<span data-ttu-id="e6732-128">String</span><span class="sxs-lookup"><span data-stu-id="e6732-128">String</span></span>|<span data-ttu-id="e6732-129">Администратор предоставил или импортировал название приложения.</span><span class="sxs-lookup"><span data-stu-id="e6732-129">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="e6732-130">description</span><span class="sxs-lookup"><span data-stu-id="e6732-130">description</span></span>|<span data-ttu-id="e6732-131">String</span><span class="sxs-lookup"><span data-stu-id="e6732-131">String</span></span>|<span data-ttu-id="e6732-132">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e6732-132">The description of the app.</span></span>|
|<span data-ttu-id="e6732-133">publisher</span><span class="sxs-lookup"><span data-stu-id="e6732-133">publisher</span></span>|<span data-ttu-id="e6732-134">String</span><span class="sxs-lookup"><span data-stu-id="e6732-134">String</span></span>|<span data-ttu-id="e6732-135">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e6732-135">The publisher of the app.</span></span>|
|<span data-ttu-id="e6732-136">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e6732-136">largeIcon</span></span>|[<span data-ttu-id="e6732-137">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e6732-137">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e6732-138">Большой значок, отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e6732-138">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="e6732-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6732-139">createdDateTime</span></span>|<span data-ttu-id="e6732-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6732-140">DateTimeOffset</span></span>|<span data-ttu-id="e6732-141">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e6732-141">The date and time the app was created.</span></span>|
|<span data-ttu-id="e6732-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6732-142">lastModifiedDateTime</span></span>|<span data-ttu-id="e6732-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6732-143">DateTimeOffset</span></span>|<span data-ttu-id="e6732-144">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e6732-144">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="e6732-145">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e6732-145">isFeatured</span></span>|<span data-ttu-id="e6732-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6732-146">Boolean</span></span>|<span data-ttu-id="e6732-147">Значение, которое показывает, отмечено ли приложение как подобранное администратором.</span><span class="sxs-lookup"><span data-stu-id="e6732-147">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="e6732-148">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e6732-148">privacyInformationUrl</span></span>|<span data-ttu-id="e6732-149">String</span><span class="sxs-lookup"><span data-stu-id="e6732-149">String</span></span>|<span data-ttu-id="e6732-150">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e6732-150">The privacy statement Url.</span></span>|
|<span data-ttu-id="e6732-151">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e6732-151">informationUrl</span></span>|<span data-ttu-id="e6732-152">String</span><span class="sxs-lookup"><span data-stu-id="e6732-152">String</span></span>|<span data-ttu-id="e6732-153">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e6732-153">The more information Url.</span></span>|
|<span data-ttu-id="e6732-154">owner</span><span class="sxs-lookup"><span data-stu-id="e6732-154">owner</span></span>|<span data-ttu-id="e6732-155">String</span><span class="sxs-lookup"><span data-stu-id="e6732-155">String</span></span>|<span data-ttu-id="e6732-156">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e6732-156">The owner of the app.</span></span>|
|<span data-ttu-id="e6732-157">developer</span><span class="sxs-lookup"><span data-stu-id="e6732-157">developer</span></span>|<span data-ttu-id="e6732-158">String</span><span class="sxs-lookup"><span data-stu-id="e6732-158">String</span></span>|<span data-ttu-id="e6732-159">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e6732-159">The developer of the app.</span></span>|
|<span data-ttu-id="e6732-160">notes</span><span class="sxs-lookup"><span data-stu-id="e6732-160">notes</span></span>|<span data-ttu-id="e6732-161">String</span><span class="sxs-lookup"><span data-stu-id="e6732-161">String</span></span>|<span data-ttu-id="e6732-162">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="e6732-162">Notes for the app.</span></span>|
|<span data-ttu-id="e6732-163">publishingState</span><span class="sxs-lookup"><span data-stu-id="e6732-163">publishingState</span></span>|[<span data-ttu-id="e6732-164">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e6732-164">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e6732-165">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="e6732-165">The publishing state for the app.</span></span> <span data-ttu-id="e6732-166">Приложение не может быть назначено, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e6732-166">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e6732-167">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e6732-167">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6732-168">Отношения</span><span class="sxs-lookup"><span data-stu-id="e6732-168">Relationships</span></span>
|<span data-ttu-id="e6732-169">Связь</span><span class="sxs-lookup"><span data-stu-id="e6732-169">Relationship</span></span>|<span data-ttu-id="e6732-170">Тип</span><span class="sxs-lookup"><span data-stu-id="e6732-170">Type</span></span>|<span data-ttu-id="e6732-171">Описание</span><span class="sxs-lookup"><span data-stu-id="e6732-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6732-172">categories</span><span class="sxs-lookup"><span data-stu-id="e6732-172">categories</span></span>|<span data-ttu-id="e6732-173">Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="e6732-173">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="e6732-174">Список категорий для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="e6732-174">The list of categories for this app.</span></span>|
|<span data-ttu-id="e6732-175">assignments</span><span class="sxs-lookup"><span data-stu-id="e6732-175">assignments</span></span>|<span data-ttu-id="e6732-176">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e6732-176">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="e6732-177">Список назначений группы для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e6732-177">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6732-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6732-178">JSON Representation</span></span>
<span data-ttu-id="e6732-179">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6732-179">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String"
}
```




