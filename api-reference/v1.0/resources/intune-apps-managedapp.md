---
title: Тип ресурса managedApp
description: Абстрактный класс содержит свойства, в том числе унаследованные, для приложений, которыми вы можете управлять с помощью политики защиты приложений Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4fbb934f3bb52c1980908c1595c2252800c465e3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756052"
---
# <a name="managedapp-resource-type"></a><span data-ttu-id="915b9-103">Тип ресурса managedApp</span><span class="sxs-lookup"><span data-stu-id="915b9-103">managedApp resource type</span></span>

<span data-ttu-id="915b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="915b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="915b9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="915b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="915b9-106">Абстрактный класс содержит свойства, в том числе унаследованные, для приложений, которыми вы можете управлять с помощью политики защиты приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="915b9-106">Abstract class that contains properties and inherited properties for apps that you can manage with an Intune app protection policy.</span></span>


<span data-ttu-id="915b9-107">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="915b9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="915b9-108">Methods</span></span>
|<span data-ttu-id="915b9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="915b9-109">Method</span></span>|<span data-ttu-id="915b9-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="915b9-110">Return Type</span></span>|<span data-ttu-id="915b9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="915b9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="915b9-112">Перечисление managedApps</span><span class="sxs-lookup"><span data-stu-id="915b9-112">List managedApps</span></span>](../api/intune-apps-managedapp-list.md)|<span data-ttu-id="915b9-113">Коллекция [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="915b9-113">[managedApp](../resources/intune-apps-managedapp.md) collection</span></span>|<span data-ttu-id="915b9-114">Список свойств и связей объектов [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-114">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>|
|[<span data-ttu-id="915b9-115">Получение managedApp</span><span class="sxs-lookup"><span data-stu-id="915b9-115">Get managedApp</span></span>](../api/intune-apps-managedapp-get.md)|[<span data-ttu-id="915b9-116">managedApp</span><span class="sxs-lookup"><span data-stu-id="915b9-116">managedApp</span></span>](../resources/intune-apps-managedapp.md)|<span data-ttu-id="915b9-117">Считывание свойств и связей объекта [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-117">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="915b9-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="915b9-118">Properties</span></span>
|<span data-ttu-id="915b9-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="915b9-119">Property</span></span>|<span data-ttu-id="915b9-120">Тип</span><span class="sxs-lookup"><span data-stu-id="915b9-120">Type</span></span>|<span data-ttu-id="915b9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="915b9-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="915b9-122">id</span><span class="sxs-lookup"><span data-stu-id="915b9-122">id</span></span>|<span data-ttu-id="915b9-123">String</span><span class="sxs-lookup"><span data-stu-id="915b9-123">String</span></span>|<span data-ttu-id="915b9-124">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="915b9-124">Key of the entity.</span></span> <span data-ttu-id="915b9-125">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-126">displayName</span><span class="sxs-lookup"><span data-stu-id="915b9-126">displayName</span></span>|<span data-ttu-id="915b9-127">String</span><span class="sxs-lookup"><span data-stu-id="915b9-127">String</span></span>|<span data-ttu-id="915b9-128">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="915b9-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="915b9-129">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-130">description</span><span class="sxs-lookup"><span data-stu-id="915b9-130">description</span></span>|<span data-ttu-id="915b9-131">String</span><span class="sxs-lookup"><span data-stu-id="915b9-131">String</span></span>|<span data-ttu-id="915b9-132">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="915b9-132">The description of the app.</span></span> <span data-ttu-id="915b9-133">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-134">publisher</span><span class="sxs-lookup"><span data-stu-id="915b9-134">publisher</span></span>|<span data-ttu-id="915b9-135">String</span><span class="sxs-lookup"><span data-stu-id="915b9-135">String</span></span>|<span data-ttu-id="915b9-136">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="915b9-136">The publisher of the app.</span></span> <span data-ttu-id="915b9-137">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="915b9-138">largeIcon</span></span>|[<span data-ttu-id="915b9-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="915b9-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="915b9-140">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="915b9-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="915b9-141">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="915b9-142">createdDateTime</span></span>|<span data-ttu-id="915b9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="915b9-143">DateTimeOffset</span></span>|<span data-ttu-id="915b9-144">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="915b9-144">The date and time the app was created.</span></span> <span data-ttu-id="915b9-145">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="915b9-146">lastModifiedDateTime</span></span>|<span data-ttu-id="915b9-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="915b9-147">DateTimeOffset</span></span>|<span data-ttu-id="915b9-148">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="915b9-148">The date and time the app was last modified.</span></span> <span data-ttu-id="915b9-149">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="915b9-150">isFeatured</span></span>|<span data-ttu-id="915b9-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="915b9-151">Boolean</span></span>|<span data-ttu-id="915b9-152">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="915b9-153">privacyInformationUrl</span></span>|<span data-ttu-id="915b9-154">String</span><span class="sxs-lookup"><span data-stu-id="915b9-154">String</span></span>|<span data-ttu-id="915b9-155">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="915b9-155">The privacy statement Url.</span></span> <span data-ttu-id="915b9-156">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="915b9-157">informationUrl</span></span>|<span data-ttu-id="915b9-158">String</span><span class="sxs-lookup"><span data-stu-id="915b9-158">String</span></span>|<span data-ttu-id="915b9-159">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="915b9-159">The more information Url.</span></span> <span data-ttu-id="915b9-160">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-161">owner</span><span class="sxs-lookup"><span data-stu-id="915b9-161">owner</span></span>|<span data-ttu-id="915b9-162">String</span><span class="sxs-lookup"><span data-stu-id="915b9-162">String</span></span>|<span data-ttu-id="915b9-163">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="915b9-163">The owner of the app.</span></span> <span data-ttu-id="915b9-164">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-165">developer</span><span class="sxs-lookup"><span data-stu-id="915b9-165">developer</span></span>|<span data-ttu-id="915b9-166">String</span><span class="sxs-lookup"><span data-stu-id="915b9-166">String</span></span>|<span data-ttu-id="915b9-167">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="915b9-167">The developer of the app.</span></span> <span data-ttu-id="915b9-168">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-169">notes</span><span class="sxs-lookup"><span data-stu-id="915b9-169">notes</span></span>|<span data-ttu-id="915b9-170">String</span><span class="sxs-lookup"><span data-stu-id="915b9-170">String</span></span>|<span data-ttu-id="915b9-171">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="915b9-171">Notes for the app.</span></span> <span data-ttu-id="915b9-172">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="915b9-173">publishingState</span></span>|[<span data-ttu-id="915b9-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="915b9-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="915b9-175">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="915b9-175">The publishing state for the app.</span></span> <span data-ttu-id="915b9-176">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="915b9-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="915b9-177">Унаследованный от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="915b9-178">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="915b9-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="915b9-179">appAvailability</span><span class="sxs-lookup"><span data-stu-id="915b9-179">appAvailability</span></span>|[<span data-ttu-id="915b9-180">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="915b9-180">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="915b9-181">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="915b9-181">The Application's availability.</span></span> <span data-ttu-id="915b9-182">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="915b9-182">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="915b9-183">version</span><span class="sxs-lookup"><span data-stu-id="915b9-183">version</span></span>|<span data-ttu-id="915b9-184">String</span><span class="sxs-lookup"><span data-stu-id="915b9-184">String</span></span>|<span data-ttu-id="915b9-185">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="915b9-185">The Application's version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="915b9-186">Отношения</span><span class="sxs-lookup"><span data-stu-id="915b9-186">Relationships</span></span>
|<span data-ttu-id="915b9-187">Связь</span><span class="sxs-lookup"><span data-stu-id="915b9-187">Relationship</span></span>|<span data-ttu-id="915b9-188">Тип</span><span class="sxs-lookup"><span data-stu-id="915b9-188">Type</span></span>|<span data-ttu-id="915b9-189">Описание</span><span class="sxs-lookup"><span data-stu-id="915b9-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="915b9-190">categories</span><span class="sxs-lookup"><span data-stu-id="915b9-190">categories</span></span>|<span data-ttu-id="915b9-191">Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="915b9-191">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="915b9-192">Список категорий для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="915b9-192">The list of categories for this app.</span></span> <span data-ttu-id="915b9-193">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-193">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="915b9-194">assignments</span><span class="sxs-lookup"><span data-stu-id="915b9-194">assignments</span></span>|<span data-ttu-id="915b9-195">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="915b9-195">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="915b9-196">Список назначений группы для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="915b9-196">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="915b9-197">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="915b9-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="915b9-198">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="915b9-198">JSON Representation</span></span>
<span data-ttu-id="915b9-199">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="915b9-199">Here is a JSON representation of the resource.</span></span>
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




