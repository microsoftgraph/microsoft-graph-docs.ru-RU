---
title: Тип ресурса mobileApp
description: Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8287895e66c016f92cdee7c4da8e3d9881b239b8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457878"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="89354-103">Тип ресурса mobileApp</span><span class="sxs-lookup"><span data-stu-id="89354-103">mobileApp resource type</span></span>

<span data-ttu-id="89354-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89354-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89354-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89354-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89354-106">Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="89354-106">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="89354-107">Методы</span><span class="sxs-lookup"><span data-stu-id="89354-107">Methods</span></span>
|<span data-ttu-id="89354-108">Метод</span><span class="sxs-lookup"><span data-stu-id="89354-108">Method</span></span>|<span data-ttu-id="89354-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="89354-109">Return Type</span></span>|<span data-ttu-id="89354-110">Описание</span><span class="sxs-lookup"><span data-stu-id="89354-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="89354-111">Список mobileApps</span><span class="sxs-lookup"><span data-stu-id="89354-111">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="89354-112">Коллекция [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="89354-112">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="89354-113">Список свойств и связей объектов [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="89354-113">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="89354-114">Получение объекта mobileApp</span><span class="sxs-lookup"><span data-stu-id="89354-114">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="89354-115">mobileApp</span><span class="sxs-lookup"><span data-stu-id="89354-115">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="89354-116">Чтение свойств и связей объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="89354-116">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="89354-117">assign action</span><span class="sxs-lookup"><span data-stu-id="89354-117">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="89354-118">Нет</span><span class="sxs-lookup"><span data-stu-id="89354-118">None</span></span>|<span data-ttu-id="89354-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="89354-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="89354-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="89354-120">Properties</span></span>
|<span data-ttu-id="89354-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="89354-121">Property</span></span>|<span data-ttu-id="89354-122">Тип</span><span class="sxs-lookup"><span data-stu-id="89354-122">Type</span></span>|<span data-ttu-id="89354-123">Описание</span><span class="sxs-lookup"><span data-stu-id="89354-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89354-124">id</span><span class="sxs-lookup"><span data-stu-id="89354-124">id</span></span>|<span data-ttu-id="89354-125">Строка</span><span class="sxs-lookup"><span data-stu-id="89354-125">String</span></span>|<span data-ttu-id="89354-126">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="89354-126">Key of the entity.</span></span>|
|<span data-ttu-id="89354-127">displayName</span><span class="sxs-lookup"><span data-stu-id="89354-127">displayName</span></span>|<span data-ttu-id="89354-128">Строка</span><span class="sxs-lookup"><span data-stu-id="89354-128">String</span></span>|<span data-ttu-id="89354-129">Администратор предоставил или импортировал название приложения.</span><span class="sxs-lookup"><span data-stu-id="89354-129">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="89354-130">description</span><span class="sxs-lookup"><span data-stu-id="89354-130">description</span></span>|<span data-ttu-id="89354-131">Строка</span><span class="sxs-lookup"><span data-stu-id="89354-131">String</span></span>|<span data-ttu-id="89354-132">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="89354-132">The description of the app.</span></span>|
|<span data-ttu-id="89354-133">publisher</span><span class="sxs-lookup"><span data-stu-id="89354-133">publisher</span></span>|<span data-ttu-id="89354-134">String</span><span class="sxs-lookup"><span data-stu-id="89354-134">String</span></span>|<span data-ttu-id="89354-135">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="89354-135">The publisher of the app.</span></span>|
|<span data-ttu-id="89354-136">largeIcon</span><span class="sxs-lookup"><span data-stu-id="89354-136">largeIcon</span></span>|[<span data-ttu-id="89354-137">mimeContent</span><span class="sxs-lookup"><span data-stu-id="89354-137">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="89354-138">Большой значок, отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="89354-138">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="89354-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89354-139">createdDateTime</span></span>|<span data-ttu-id="89354-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89354-140">DateTimeOffset</span></span>|<span data-ttu-id="89354-141">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="89354-141">The date and time the app was created.</span></span>|
|<span data-ttu-id="89354-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89354-142">lastModifiedDateTime</span></span>|<span data-ttu-id="89354-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89354-143">DateTimeOffset</span></span>|<span data-ttu-id="89354-144">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="89354-144">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="89354-145">isFeatured</span><span class="sxs-lookup"><span data-stu-id="89354-145">isFeatured</span></span>|<span data-ttu-id="89354-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="89354-146">Boolean</span></span>|<span data-ttu-id="89354-147">Значение, которое показывает, отмечено ли приложение как подобранное администратором.</span><span class="sxs-lookup"><span data-stu-id="89354-147">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="89354-148">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="89354-148">privacyInformationUrl</span></span>|<span data-ttu-id="89354-149">String</span><span class="sxs-lookup"><span data-stu-id="89354-149">String</span></span>|<span data-ttu-id="89354-150">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="89354-150">The privacy statement Url.</span></span>|
|<span data-ttu-id="89354-151">informationUrl</span><span class="sxs-lookup"><span data-stu-id="89354-151">informationUrl</span></span>|<span data-ttu-id="89354-152">String</span><span class="sxs-lookup"><span data-stu-id="89354-152">String</span></span>|<span data-ttu-id="89354-153">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="89354-153">The more information Url.</span></span>|
|<span data-ttu-id="89354-154">owner</span><span class="sxs-lookup"><span data-stu-id="89354-154">owner</span></span>|<span data-ttu-id="89354-155">String</span><span class="sxs-lookup"><span data-stu-id="89354-155">String</span></span>|<span data-ttu-id="89354-156">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="89354-156">The owner of the app.</span></span>|
|<span data-ttu-id="89354-157">developer</span><span class="sxs-lookup"><span data-stu-id="89354-157">developer</span></span>|<span data-ttu-id="89354-158">String</span><span class="sxs-lookup"><span data-stu-id="89354-158">String</span></span>|<span data-ttu-id="89354-159">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="89354-159">The developer of the app.</span></span>|
|<span data-ttu-id="89354-160">notes</span><span class="sxs-lookup"><span data-stu-id="89354-160">notes</span></span>|<span data-ttu-id="89354-161">String</span><span class="sxs-lookup"><span data-stu-id="89354-161">String</span></span>|<span data-ttu-id="89354-162">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="89354-162">Notes for the app.</span></span>|
|<span data-ttu-id="89354-163">publishingState</span><span class="sxs-lookup"><span data-stu-id="89354-163">publishingState</span></span>|[<span data-ttu-id="89354-164">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="89354-164">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="89354-165">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="89354-165">The publishing state for the app.</span></span> <span data-ttu-id="89354-166">Приложение не может быть назначено, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="89354-166">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="89354-167">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="89354-167">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89354-168">Связи</span><span class="sxs-lookup"><span data-stu-id="89354-168">Relationships</span></span>
|<span data-ttu-id="89354-169">Связь</span><span class="sxs-lookup"><span data-stu-id="89354-169">Relationship</span></span>|<span data-ttu-id="89354-170">Тип</span><span class="sxs-lookup"><span data-stu-id="89354-170">Type</span></span>|<span data-ttu-id="89354-171">Описание</span><span class="sxs-lookup"><span data-stu-id="89354-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89354-172">categories</span><span class="sxs-lookup"><span data-stu-id="89354-172">categories</span></span>|<span data-ttu-id="89354-173">Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="89354-173">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="89354-174">Список категорий для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="89354-174">The list of categories for this app.</span></span>|
|<span data-ttu-id="89354-175">assignments</span><span class="sxs-lookup"><span data-stu-id="89354-175">assignments</span></span>|<span data-ttu-id="89354-176">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="89354-176">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="89354-177">Список назначений группы для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="89354-177">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89354-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89354-178">JSON Representation</span></span>
<span data-ttu-id="89354-179">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89354-179">Here is a JSON representation of the resource.</span></span>
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







