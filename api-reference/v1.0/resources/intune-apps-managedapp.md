---
title: Тип ресурса managedApp
description: Абстрактный класс содержит свойства, в том числе унаследованные, для приложений, которыми вы можете управлять с помощью политики защиты приложений Intune.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 36e3da414e20ebf419b7e917536617778670a5b5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43354470"
---
# <a name="managedapp-resource-type"></a><span data-ttu-id="c5b2d-103">Тип ресурса managedApp</span><span class="sxs-lookup"><span data-stu-id="c5b2d-103">managedApp resource type</span></span>

<span data-ttu-id="c5b2d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5b2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5b2d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5b2d-106">Абстрактный класс содержит свойства, в том числе унаследованные, для приложений, которыми вы можете управлять с помощью политики защиты приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-106">Abstract class that contains properties and inherited properties for apps that you can manage with an Intune app protection policy.</span></span>


<span data-ttu-id="c5b2d-107">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c5b2d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c5b2d-108">Methods</span></span>
|<span data-ttu-id="c5b2d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c5b2d-109">Method</span></span>|<span data-ttu-id="c5b2d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c5b2d-110">Return Type</span></span>|<span data-ttu-id="c5b2d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c5b2d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c5b2d-112">Перечисление managedApps</span><span class="sxs-lookup"><span data-stu-id="c5b2d-112">List managedApps</span></span>](../api/intune-apps-managedapp-list.md)|<span data-ttu-id="c5b2d-113">Коллекция [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c5b2d-113">[managedApp](../resources/intune-apps-managedapp.md) collection</span></span>|<span data-ttu-id="c5b2d-114">Список свойств и связей объектов [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-114">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>|
|[<span data-ttu-id="c5b2d-115">Получение managedApp</span><span class="sxs-lookup"><span data-stu-id="c5b2d-115">Get managedApp</span></span>](../api/intune-apps-managedapp-get.md)|[<span data-ttu-id="c5b2d-116">managedApp</span><span class="sxs-lookup"><span data-stu-id="c5b2d-116">managedApp</span></span>](../resources/intune-apps-managedapp.md)|<span data-ttu-id="c5b2d-117">Считывание свойств и связей объекта [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-117">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5b2d-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5b2d-118">Properties</span></span>
|<span data-ttu-id="c5b2d-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5b2d-119">Property</span></span>|<span data-ttu-id="c5b2d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c5b2d-120">Type</span></span>|<span data-ttu-id="c5b2d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c5b2d-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5b2d-122">id</span><span class="sxs-lookup"><span data-stu-id="c5b2d-122">id</span></span>|<span data-ttu-id="c5b2d-123">Строка</span><span class="sxs-lookup"><span data-stu-id="c5b2d-123">String</span></span>|<span data-ttu-id="c5b2d-124">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-124">Key of the entity.</span></span> <span data-ttu-id="c5b2d-125">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-126">displayName</span><span class="sxs-lookup"><span data-stu-id="c5b2d-126">displayName</span></span>|<span data-ttu-id="c5b2d-127">Строка</span><span class="sxs-lookup"><span data-stu-id="c5b2d-127">String</span></span>|<span data-ttu-id="c5b2d-128">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c5b2d-129">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-130">description</span><span class="sxs-lookup"><span data-stu-id="c5b2d-130">description</span></span>|<span data-ttu-id="c5b2d-131">String</span><span class="sxs-lookup"><span data-stu-id="c5b2d-131">String</span></span>|<span data-ttu-id="c5b2d-132">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-132">The description of the app.</span></span> <span data-ttu-id="c5b2d-133">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-134">publisher</span><span class="sxs-lookup"><span data-stu-id="c5b2d-134">publisher</span></span>|<span data-ttu-id="c5b2d-135">String</span><span class="sxs-lookup"><span data-stu-id="c5b2d-135">String</span></span>|<span data-ttu-id="c5b2d-136">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-136">The publisher of the app.</span></span> <span data-ttu-id="c5b2d-137">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c5b2d-138">largeIcon</span></span>|[<span data-ttu-id="c5b2d-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c5b2d-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c5b2d-140">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c5b2d-141">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5b2d-142">createdDateTime</span></span>|<span data-ttu-id="c5b2d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5b2d-143">DateTimeOffset</span></span>|<span data-ttu-id="c5b2d-144">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-144">The date and time the app was created.</span></span> <span data-ttu-id="c5b2d-145">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5b2d-146">lastModifiedDateTime</span></span>|<span data-ttu-id="c5b2d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5b2d-147">DateTimeOffset</span></span>|<span data-ttu-id="c5b2d-148">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-148">The date and time the app was last modified.</span></span> <span data-ttu-id="c5b2d-149">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c5b2d-150">isFeatured</span></span>|<span data-ttu-id="c5b2d-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5b2d-151">Boolean</span></span>|<span data-ttu-id="c5b2d-152">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c5b2d-153">privacyInformationUrl</span></span>|<span data-ttu-id="c5b2d-154">String</span><span class="sxs-lookup"><span data-stu-id="c5b2d-154">String</span></span>|<span data-ttu-id="c5b2d-155">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-155">The privacy statement Url.</span></span> <span data-ttu-id="c5b2d-156">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c5b2d-157">informationUrl</span></span>|<span data-ttu-id="c5b2d-158">String</span><span class="sxs-lookup"><span data-stu-id="c5b2d-158">String</span></span>|<span data-ttu-id="c5b2d-159">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-159">The more information Url.</span></span> <span data-ttu-id="c5b2d-160">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-161">owner</span><span class="sxs-lookup"><span data-stu-id="c5b2d-161">owner</span></span>|<span data-ttu-id="c5b2d-162">String</span><span class="sxs-lookup"><span data-stu-id="c5b2d-162">String</span></span>|<span data-ttu-id="c5b2d-163">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-163">The owner of the app.</span></span> <span data-ttu-id="c5b2d-164">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-165">developer</span><span class="sxs-lookup"><span data-stu-id="c5b2d-165">developer</span></span>|<span data-ttu-id="c5b2d-166">String</span><span class="sxs-lookup"><span data-stu-id="c5b2d-166">String</span></span>|<span data-ttu-id="c5b2d-167">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-167">The developer of the app.</span></span> <span data-ttu-id="c5b2d-168">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-169">notes</span><span class="sxs-lookup"><span data-stu-id="c5b2d-169">notes</span></span>|<span data-ttu-id="c5b2d-170">String</span><span class="sxs-lookup"><span data-stu-id="c5b2d-170">String</span></span>|<span data-ttu-id="c5b2d-171">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-171">Notes for the app.</span></span> <span data-ttu-id="c5b2d-172">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c5b2d-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="c5b2d-173">publishingState</span></span>|[<span data-ttu-id="c5b2d-174">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="c5b2d-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c5b2d-175">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-175">The publishing state for the app.</span></span> <span data-ttu-id="c5b2d-176">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c5b2d-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c5b2d-178">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c5b2d-179">appAvailability</span><span class="sxs-lookup"><span data-stu-id="c5b2d-179">appAvailability</span></span>|[<span data-ttu-id="c5b2d-180">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="c5b2d-180">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="c5b2d-181">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-181">The Application's availability.</span></span> <span data-ttu-id="c5b2d-182">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-182">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="c5b2d-183">version</span><span class="sxs-lookup"><span data-stu-id="c5b2d-183">version</span></span>|<span data-ttu-id="c5b2d-184">String</span><span class="sxs-lookup"><span data-stu-id="c5b2d-184">String</span></span>|<span data-ttu-id="c5b2d-185">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-185">The Application's version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5b2d-186">Отношения</span><span class="sxs-lookup"><span data-stu-id="c5b2d-186">Relationships</span></span>
|<span data-ttu-id="c5b2d-187">Связь</span><span class="sxs-lookup"><span data-stu-id="c5b2d-187">Relationship</span></span>|<span data-ttu-id="c5b2d-188">Тип</span><span class="sxs-lookup"><span data-stu-id="c5b2d-188">Type</span></span>|<span data-ttu-id="c5b2d-189">Описание</span><span class="sxs-lookup"><span data-stu-id="c5b2d-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5b2d-190">categories</span><span class="sxs-lookup"><span data-stu-id="c5b2d-190">categories</span></span>|<span data-ttu-id="c5b2d-191">Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="c5b2d-191">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="c5b2d-192">Список категорий для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-192">The list of categories for this app.</span></span> <span data-ttu-id="c5b2d-193">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-193">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5b2d-194">assignments</span><span class="sxs-lookup"><span data-stu-id="c5b2d-194">assignments</span></span>|<span data-ttu-id="c5b2d-195">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c5b2d-195">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="c5b2d-196">Список назначений группы для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-196">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="c5b2d-197">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5b2d-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5b2d-198">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5b2d-198">JSON Representation</span></span>
<span data-ttu-id="c5b2d-199">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5b2d-199">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedApp",
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
  "publishingState": "String",
  "appAvailability": "String",
  "version": "String"
}
```







