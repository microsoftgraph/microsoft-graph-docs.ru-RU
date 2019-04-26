---
title: Тип ресурса mobileApp
description: Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91167967a543ea4556c1704a2bba4ec9a10a4c3d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557896"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="f0ed6-103">Тип ресурса mobileApp</span><span class="sxs-lookup"><span data-stu-id="f0ed6-103">mobileApp resource type</span></span>

> <span data-ttu-id="f0ed6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0ed6-105">Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-105">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="f0ed6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f0ed6-106">Methods</span></span>
|<span data-ttu-id="f0ed6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f0ed6-107">Method</span></span>|<span data-ttu-id="f0ed6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f0ed6-108">Return Type</span></span>|<span data-ttu-id="f0ed6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f0ed6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f0ed6-110">Список mobileApps</span><span class="sxs-lookup"><span data-stu-id="f0ed6-110">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="f0ed6-111">Коллекция [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0ed6-111">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="f0ed6-112">Список свойств и связей объектов [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0ed6-112">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="f0ed6-113">Получение объекта mobileApp</span><span class="sxs-lookup"><span data-stu-id="f0ed6-113">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="f0ed6-114">mobileApp</span><span class="sxs-lookup"><span data-stu-id="f0ed6-114">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="f0ed6-115">Чтение свойств и связей объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0ed6-115">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="f0ed6-116">assign action</span><span class="sxs-lookup"><span data-stu-id="f0ed6-116">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="f0ed6-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f0ed6-117">None</span></span>|<span data-ttu-id="f0ed6-118">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f0ed6-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f0ed6-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0ed6-119">Properties</span></span>
|<span data-ttu-id="f0ed6-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0ed6-120">Property</span></span>|<span data-ttu-id="f0ed6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f0ed6-121">Type</span></span>|<span data-ttu-id="f0ed6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f0ed6-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0ed6-123">id</span><span class="sxs-lookup"><span data-stu-id="f0ed6-123">id</span></span>|<span data-ttu-id="f0ed6-124">Строка</span><span class="sxs-lookup"><span data-stu-id="f0ed6-124">String</span></span>|<span data-ttu-id="f0ed6-125">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-125">Key of the entity.</span></span>|
|<span data-ttu-id="f0ed6-126">displayName</span><span class="sxs-lookup"><span data-stu-id="f0ed6-126">displayName</span></span>|<span data-ttu-id="f0ed6-127">Строка</span><span class="sxs-lookup"><span data-stu-id="f0ed6-127">String</span></span>|<span data-ttu-id="f0ed6-128">Администратор предоставил или импортировал название приложения.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-128">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="f0ed6-129">description</span><span class="sxs-lookup"><span data-stu-id="f0ed6-129">description</span></span>|<span data-ttu-id="f0ed6-130">String</span><span class="sxs-lookup"><span data-stu-id="f0ed6-130">String</span></span>|<span data-ttu-id="f0ed6-131">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-131">The description of the app.</span></span>|
|<span data-ttu-id="f0ed6-132">publisher</span><span class="sxs-lookup"><span data-stu-id="f0ed6-132">publisher</span></span>|<span data-ttu-id="f0ed6-133">String</span><span class="sxs-lookup"><span data-stu-id="f0ed6-133">String</span></span>|<span data-ttu-id="f0ed6-134">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-134">The publisher of the app.</span></span>|
|<span data-ttu-id="f0ed6-135">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f0ed6-135">largeIcon</span></span>|[<span data-ttu-id="f0ed6-136">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f0ed6-136">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f0ed6-137">Большой значок, отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-137">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="f0ed6-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0ed6-138">createdDateTime</span></span>|<span data-ttu-id="f0ed6-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0ed6-139">DateTimeOffset</span></span>|<span data-ttu-id="f0ed6-140">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-140">The date and time the app was created.</span></span>|
|<span data-ttu-id="f0ed6-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0ed6-141">lastModifiedDateTime</span></span>|<span data-ttu-id="f0ed6-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0ed6-142">DateTimeOffset</span></span>|<span data-ttu-id="f0ed6-143">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-143">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="f0ed6-144">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f0ed6-144">isFeatured</span></span>|<span data-ttu-id="f0ed6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0ed6-145">Boolean</span></span>|<span data-ttu-id="f0ed6-146">Значение, которое показывает, отмечено ли приложение как подобранное администратором.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-146">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="f0ed6-147">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f0ed6-147">privacyInformationUrl</span></span>|<span data-ttu-id="f0ed6-148">String</span><span class="sxs-lookup"><span data-stu-id="f0ed6-148">String</span></span>|<span data-ttu-id="f0ed6-149">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-149">The privacy statement Url.</span></span>|
|<span data-ttu-id="f0ed6-150">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f0ed6-150">informationUrl</span></span>|<span data-ttu-id="f0ed6-151">String</span><span class="sxs-lookup"><span data-stu-id="f0ed6-151">String</span></span>|<span data-ttu-id="f0ed6-152">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-152">The more information Url.</span></span>|
|<span data-ttu-id="f0ed6-153">owner</span><span class="sxs-lookup"><span data-stu-id="f0ed6-153">owner</span></span>|<span data-ttu-id="f0ed6-154">String</span><span class="sxs-lookup"><span data-stu-id="f0ed6-154">String</span></span>|<span data-ttu-id="f0ed6-155">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-155">The owner of the app.</span></span>|
|<span data-ttu-id="f0ed6-156">developer</span><span class="sxs-lookup"><span data-stu-id="f0ed6-156">developer</span></span>|<span data-ttu-id="f0ed6-157">String</span><span class="sxs-lookup"><span data-stu-id="f0ed6-157">String</span></span>|<span data-ttu-id="f0ed6-158">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-158">The developer of the app.</span></span>|
|<span data-ttu-id="f0ed6-159">notes</span><span class="sxs-lookup"><span data-stu-id="f0ed6-159">notes</span></span>|<span data-ttu-id="f0ed6-160">String</span><span class="sxs-lookup"><span data-stu-id="f0ed6-160">String</span></span>|<span data-ttu-id="f0ed6-161">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-161">Notes for the app.</span></span>|
|<span data-ttu-id="f0ed6-162">publishingState</span><span class="sxs-lookup"><span data-stu-id="f0ed6-162">publishingState</span></span>|[<span data-ttu-id="f0ed6-163">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="f0ed6-163">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f0ed6-164">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-164">The publishing state for the app.</span></span> <span data-ttu-id="f0ed6-165">Приложение не может быть назначено, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-165">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f0ed6-166">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-166">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0ed6-167">Связи</span><span class="sxs-lookup"><span data-stu-id="f0ed6-167">Relationships</span></span>
|<span data-ttu-id="f0ed6-168">Отношение</span><span class="sxs-lookup"><span data-stu-id="f0ed6-168">Relationship</span></span>|<span data-ttu-id="f0ed6-169">Тип</span><span class="sxs-lookup"><span data-stu-id="f0ed6-169">Type</span></span>|<span data-ttu-id="f0ed6-170">Описание</span><span class="sxs-lookup"><span data-stu-id="f0ed6-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0ed6-171">categories</span><span class="sxs-lookup"><span data-stu-id="f0ed6-171">categories</span></span>|<span data-ttu-id="f0ed6-172">Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="f0ed6-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="f0ed6-173">Список категорий для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-173">The list of categories for this app.</span></span>|
|<span data-ttu-id="f0ed6-174">assignments</span><span class="sxs-lookup"><span data-stu-id="f0ed6-174">assignments</span></span>|<span data-ttu-id="f0ed6-175">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f0ed6-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="f0ed6-176">Список назначений группы для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-176">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0ed6-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0ed6-177">JSON Representation</span></span>
<span data-ttu-id="f0ed6-178">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0ed6-178">Here is a JSON representation of the resource.</span></span>
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



