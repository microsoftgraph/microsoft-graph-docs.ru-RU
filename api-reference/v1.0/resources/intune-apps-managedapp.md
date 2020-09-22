---
title: Тип ресурса managedApp
description: Абстрактный класс содержит свойства, в том числе унаследованные, для приложений, которыми вы можете управлять с помощью политики защиты приложений Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 72cb905c266dba33c635dded929b32bc333705f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015428"
---
# <a name="managedapp-resource-type"></a><span data-ttu-id="37de5-103">Тип ресурса managedApp</span><span class="sxs-lookup"><span data-stu-id="37de5-103">managedApp resource type</span></span>

<span data-ttu-id="37de5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37de5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37de5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37de5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37de5-106">Абстрактный класс содержит свойства, в том числе унаследованные, для приложений, которыми вы можете управлять с помощью политики защиты приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="37de5-106">Abstract class that contains properties and inherited properties for apps that you can manage with an Intune app protection policy.</span></span>


<span data-ttu-id="37de5-107">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="37de5-108">Методы</span><span class="sxs-lookup"><span data-stu-id="37de5-108">Methods</span></span>
|<span data-ttu-id="37de5-109">Метод</span><span class="sxs-lookup"><span data-stu-id="37de5-109">Method</span></span>|<span data-ttu-id="37de5-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="37de5-110">Return Type</span></span>|<span data-ttu-id="37de5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="37de5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="37de5-112">Перечисление managedApps</span><span class="sxs-lookup"><span data-stu-id="37de5-112">List managedApps</span></span>](../api/intune-apps-managedapp-list.md)|<span data-ttu-id="37de5-113">Коллекция [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="37de5-113">[managedApp](../resources/intune-apps-managedapp.md) collection</span></span>|<span data-ttu-id="37de5-114">Список свойств и связей объектов [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-114">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>|
|[<span data-ttu-id="37de5-115">Получение managedApp</span><span class="sxs-lookup"><span data-stu-id="37de5-115">Get managedApp</span></span>](../api/intune-apps-managedapp-get.md)|[<span data-ttu-id="37de5-116">managedApp</span><span class="sxs-lookup"><span data-stu-id="37de5-116">managedApp</span></span>](../resources/intune-apps-managedapp.md)|<span data-ttu-id="37de5-117">Считывание свойств и связей объекта [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-117">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="37de5-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="37de5-118">Properties</span></span>
|<span data-ttu-id="37de5-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="37de5-119">Property</span></span>|<span data-ttu-id="37de5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="37de5-120">Type</span></span>|<span data-ttu-id="37de5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="37de5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37de5-122">id</span><span class="sxs-lookup"><span data-stu-id="37de5-122">id</span></span>|<span data-ttu-id="37de5-123">String</span><span class="sxs-lookup"><span data-stu-id="37de5-123">String</span></span>|<span data-ttu-id="37de5-124">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="37de5-124">Key of the entity.</span></span> <span data-ttu-id="37de5-125">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-126">displayName</span><span class="sxs-lookup"><span data-stu-id="37de5-126">displayName</span></span>|<span data-ttu-id="37de5-127">String</span><span class="sxs-lookup"><span data-stu-id="37de5-127">String</span></span>|<span data-ttu-id="37de5-128">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="37de5-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="37de5-129">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-130">description</span><span class="sxs-lookup"><span data-stu-id="37de5-130">description</span></span>|<span data-ttu-id="37de5-131">String</span><span class="sxs-lookup"><span data-stu-id="37de5-131">String</span></span>|<span data-ttu-id="37de5-132">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="37de5-132">The description of the app.</span></span> <span data-ttu-id="37de5-133">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-134">publisher</span><span class="sxs-lookup"><span data-stu-id="37de5-134">publisher</span></span>|<span data-ttu-id="37de5-135">String</span><span class="sxs-lookup"><span data-stu-id="37de5-135">String</span></span>|<span data-ttu-id="37de5-136">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="37de5-136">The publisher of the app.</span></span> <span data-ttu-id="37de5-137">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="37de5-138">largeIcon</span></span>|[<span data-ttu-id="37de5-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="37de5-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="37de5-140">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="37de5-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="37de5-141">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37de5-142">createdDateTime</span></span>|<span data-ttu-id="37de5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37de5-143">DateTimeOffset</span></span>|<span data-ttu-id="37de5-144">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="37de5-144">The date and time the app was created.</span></span> <span data-ttu-id="37de5-145">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37de5-146">lastModifiedDateTime</span></span>|<span data-ttu-id="37de5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37de5-147">DateTimeOffset</span></span>|<span data-ttu-id="37de5-148">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="37de5-148">The date and time the app was last modified.</span></span> <span data-ttu-id="37de5-149">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="37de5-150">isFeatured</span></span>|<span data-ttu-id="37de5-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="37de5-151">Boolean</span></span>|<span data-ttu-id="37de5-152">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="37de5-153">privacyInformationUrl</span></span>|<span data-ttu-id="37de5-154">String</span><span class="sxs-lookup"><span data-stu-id="37de5-154">String</span></span>|<span data-ttu-id="37de5-155">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="37de5-155">The privacy statement Url.</span></span> <span data-ttu-id="37de5-156">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="37de5-157">informationUrl</span></span>|<span data-ttu-id="37de5-158">String</span><span class="sxs-lookup"><span data-stu-id="37de5-158">String</span></span>|<span data-ttu-id="37de5-159">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="37de5-159">The more information Url.</span></span> <span data-ttu-id="37de5-160">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-161">owner</span><span class="sxs-lookup"><span data-stu-id="37de5-161">owner</span></span>|<span data-ttu-id="37de5-162">String</span><span class="sxs-lookup"><span data-stu-id="37de5-162">String</span></span>|<span data-ttu-id="37de5-163">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="37de5-163">The owner of the app.</span></span> <span data-ttu-id="37de5-164">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-165">developer</span><span class="sxs-lookup"><span data-stu-id="37de5-165">developer</span></span>|<span data-ttu-id="37de5-166">String</span><span class="sxs-lookup"><span data-stu-id="37de5-166">String</span></span>|<span data-ttu-id="37de5-167">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="37de5-167">The developer of the app.</span></span> <span data-ttu-id="37de5-168">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-169">notes</span><span class="sxs-lookup"><span data-stu-id="37de5-169">notes</span></span>|<span data-ttu-id="37de5-170">String</span><span class="sxs-lookup"><span data-stu-id="37de5-170">String</span></span>|<span data-ttu-id="37de5-171">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="37de5-171">Notes for the app.</span></span> <span data-ttu-id="37de5-172">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="37de5-173">publishingState</span></span>|[<span data-ttu-id="37de5-174">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="37de5-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="37de5-175">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="37de5-175">The publishing state for the app.</span></span> <span data-ttu-id="37de5-176">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="37de5-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="37de5-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="37de5-178">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="37de5-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="37de5-179">appAvailability</span><span class="sxs-lookup"><span data-stu-id="37de5-179">appAvailability</span></span>|[<span data-ttu-id="37de5-180">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="37de5-180">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="37de5-181">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="37de5-181">The Application's availability.</span></span> <span data-ttu-id="37de5-182">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="37de5-182">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="37de5-183">version</span><span class="sxs-lookup"><span data-stu-id="37de5-183">version</span></span>|<span data-ttu-id="37de5-184">String</span><span class="sxs-lookup"><span data-stu-id="37de5-184">String</span></span>|<span data-ttu-id="37de5-185">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="37de5-185">The Application's version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37de5-186">Связи</span><span class="sxs-lookup"><span data-stu-id="37de5-186">Relationships</span></span>
|<span data-ttu-id="37de5-187">Связь</span><span class="sxs-lookup"><span data-stu-id="37de5-187">Relationship</span></span>|<span data-ttu-id="37de5-188">Тип</span><span class="sxs-lookup"><span data-stu-id="37de5-188">Type</span></span>|<span data-ttu-id="37de5-189">Описание</span><span class="sxs-lookup"><span data-stu-id="37de5-189">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37de5-190">categories</span><span class="sxs-lookup"><span data-stu-id="37de5-190">categories</span></span>|<span data-ttu-id="37de5-191">Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="37de5-191">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="37de5-192">Список категорий для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="37de5-192">The list of categories for this app.</span></span> <span data-ttu-id="37de5-193">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-193">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="37de5-194">assignments</span><span class="sxs-lookup"><span data-stu-id="37de5-194">assignments</span></span>|<span data-ttu-id="37de5-195">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="37de5-195">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="37de5-196">Список назначений группы для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="37de5-196">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="37de5-197">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="37de5-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37de5-198">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37de5-198">JSON Representation</span></span>
<span data-ttu-id="37de5-199">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37de5-199">Here is a JSON representation of the resource.</span></span>
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









