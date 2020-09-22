---
title: Тип ресурса mobileApp
description: Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4124a114a60f20f6540cdef7ba97787f980afdb0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094450"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="1261b-103">Тип ресурса mobileApp</span><span class="sxs-lookup"><span data-stu-id="1261b-103">mobileApp resource type</span></span>

<span data-ttu-id="1261b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1261b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1261b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1261b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1261b-106">Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="1261b-106">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="1261b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1261b-107">Methods</span></span>
|<span data-ttu-id="1261b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1261b-108">Method</span></span>|<span data-ttu-id="1261b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1261b-109">Return Type</span></span>|<span data-ttu-id="1261b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1261b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1261b-111">Список mobileApps</span><span class="sxs-lookup"><span data-stu-id="1261b-111">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="1261b-112">Коллекция [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1261b-112">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="1261b-113">Список свойств и связей объектов [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1261b-113">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="1261b-114">Получение объекта mobileApp</span><span class="sxs-lookup"><span data-stu-id="1261b-114">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="1261b-115">mobileApp</span><span class="sxs-lookup"><span data-stu-id="1261b-115">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="1261b-116">Чтение свойств и связей объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1261b-116">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="1261b-117">assign action</span><span class="sxs-lookup"><span data-stu-id="1261b-117">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="1261b-118">Нет</span><span class="sxs-lookup"><span data-stu-id="1261b-118">None</span></span>|<span data-ttu-id="1261b-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1261b-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1261b-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="1261b-120">Properties</span></span>
|<span data-ttu-id="1261b-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="1261b-121">Property</span></span>|<span data-ttu-id="1261b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1261b-122">Type</span></span>|<span data-ttu-id="1261b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1261b-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1261b-124">id</span><span class="sxs-lookup"><span data-stu-id="1261b-124">id</span></span>|<span data-ttu-id="1261b-125">Строка</span><span class="sxs-lookup"><span data-stu-id="1261b-125">String</span></span>|<span data-ttu-id="1261b-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1261b-126">Key of the entity.</span></span>|
|<span data-ttu-id="1261b-127">displayName</span><span class="sxs-lookup"><span data-stu-id="1261b-127">displayName</span></span>|<span data-ttu-id="1261b-128">Строка</span><span class="sxs-lookup"><span data-stu-id="1261b-128">String</span></span>|<span data-ttu-id="1261b-129">Администратор предоставил или импортировал название приложения.</span><span class="sxs-lookup"><span data-stu-id="1261b-129">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="1261b-130">description</span><span class="sxs-lookup"><span data-stu-id="1261b-130">description</span></span>|<span data-ttu-id="1261b-131">Строка</span><span class="sxs-lookup"><span data-stu-id="1261b-131">String</span></span>|<span data-ttu-id="1261b-132">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="1261b-132">The description of the app.</span></span>|
|<span data-ttu-id="1261b-133">publisher</span><span class="sxs-lookup"><span data-stu-id="1261b-133">publisher</span></span>|<span data-ttu-id="1261b-134">String</span><span class="sxs-lookup"><span data-stu-id="1261b-134">String</span></span>|<span data-ttu-id="1261b-135">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="1261b-135">The publisher of the app.</span></span>|
|<span data-ttu-id="1261b-136">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1261b-136">largeIcon</span></span>|[<span data-ttu-id="1261b-137">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1261b-137">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1261b-138">Большой значок, отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="1261b-138">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="1261b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1261b-139">createdDateTime</span></span>|<span data-ttu-id="1261b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1261b-140">DateTimeOffset</span></span>|<span data-ttu-id="1261b-141">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="1261b-141">The date and time the app was created.</span></span>|
|<span data-ttu-id="1261b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1261b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="1261b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1261b-143">DateTimeOffset</span></span>|<span data-ttu-id="1261b-144">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="1261b-144">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="1261b-145">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1261b-145">isFeatured</span></span>|<span data-ttu-id="1261b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1261b-146">Boolean</span></span>|<span data-ttu-id="1261b-147">Значение, которое показывает, отмечено ли приложение как подобранное администратором.</span><span class="sxs-lookup"><span data-stu-id="1261b-147">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="1261b-148">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1261b-148">privacyInformationUrl</span></span>|<span data-ttu-id="1261b-149">String</span><span class="sxs-lookup"><span data-stu-id="1261b-149">String</span></span>|<span data-ttu-id="1261b-150">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="1261b-150">The privacy statement Url.</span></span>|
|<span data-ttu-id="1261b-151">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1261b-151">informationUrl</span></span>|<span data-ttu-id="1261b-152">String</span><span class="sxs-lookup"><span data-stu-id="1261b-152">String</span></span>|<span data-ttu-id="1261b-153">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="1261b-153">The more information Url.</span></span>|
|<span data-ttu-id="1261b-154">owner</span><span class="sxs-lookup"><span data-stu-id="1261b-154">owner</span></span>|<span data-ttu-id="1261b-155">String</span><span class="sxs-lookup"><span data-stu-id="1261b-155">String</span></span>|<span data-ttu-id="1261b-156">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="1261b-156">The owner of the app.</span></span>|
|<span data-ttu-id="1261b-157">developer</span><span class="sxs-lookup"><span data-stu-id="1261b-157">developer</span></span>|<span data-ttu-id="1261b-158">String</span><span class="sxs-lookup"><span data-stu-id="1261b-158">String</span></span>|<span data-ttu-id="1261b-159">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="1261b-159">The developer of the app.</span></span>|
|<span data-ttu-id="1261b-160">notes</span><span class="sxs-lookup"><span data-stu-id="1261b-160">notes</span></span>|<span data-ttu-id="1261b-161">String</span><span class="sxs-lookup"><span data-stu-id="1261b-161">String</span></span>|<span data-ttu-id="1261b-162">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="1261b-162">Notes for the app.</span></span>|
|<span data-ttu-id="1261b-163">publishingState</span><span class="sxs-lookup"><span data-stu-id="1261b-163">publishingState</span></span>|[<span data-ttu-id="1261b-164">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="1261b-164">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1261b-165">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="1261b-165">The publishing state for the app.</span></span> <span data-ttu-id="1261b-166">Приложение не может быть назначено, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="1261b-166">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1261b-167">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1261b-167">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1261b-168">Связи</span><span class="sxs-lookup"><span data-stu-id="1261b-168">Relationships</span></span>
|<span data-ttu-id="1261b-169">Связь</span><span class="sxs-lookup"><span data-stu-id="1261b-169">Relationship</span></span>|<span data-ttu-id="1261b-170">Тип</span><span class="sxs-lookup"><span data-stu-id="1261b-170">Type</span></span>|<span data-ttu-id="1261b-171">Описание</span><span class="sxs-lookup"><span data-stu-id="1261b-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1261b-172">categories</span><span class="sxs-lookup"><span data-stu-id="1261b-172">categories</span></span>|<span data-ttu-id="1261b-173">Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1261b-173">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="1261b-174">Список категорий для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="1261b-174">The list of categories for this app.</span></span>|
|<span data-ttu-id="1261b-175">assignments</span><span class="sxs-lookup"><span data-stu-id="1261b-175">assignments</span></span>|<span data-ttu-id="1261b-176">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1261b-176">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="1261b-177">Список назначений группы для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="1261b-177">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1261b-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1261b-178">JSON Representation</span></span>
<span data-ttu-id="1261b-179">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1261b-179">Here is a JSON representation of the resource.</span></span>
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









