---
title: Тип ресурса mobileApp
description: Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c5b7af252c27f60a1b6dd78f7a69bc7a712541b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938456"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="eba5a-103">Тип ресурса mobileApp</span><span class="sxs-lookup"><span data-stu-id="eba5a-103">mobileApp resource type</span></span>

> <span data-ttu-id="eba5a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eba5a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eba5a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eba5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eba5a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eba5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eba5a-107">Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="eba5a-107">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="eba5a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="eba5a-108">Methods</span></span>
|<span data-ttu-id="eba5a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="eba5a-109">Method</span></span>|<span data-ttu-id="eba5a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eba5a-110">Return Type</span></span>|<span data-ttu-id="eba5a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eba5a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eba5a-112">Список mobileApps</span><span class="sxs-lookup"><span data-stu-id="eba5a-112">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="eba5a-113">Коллекция [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eba5a-113">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="eba5a-114">Список свойств и связей объектов [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eba5a-114">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="eba5a-115">Получение объекта mobileApp</span><span class="sxs-lookup"><span data-stu-id="eba5a-115">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="eba5a-116">mobileApp</span><span class="sxs-lookup"><span data-stu-id="eba5a-116">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="eba5a-117">Чтение свойств и связей объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eba5a-117">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="eba5a-118">assign action</span><span class="sxs-lookup"><span data-stu-id="eba5a-118">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="eba5a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="eba5a-119">None</span></span>|<span data-ttu-id="eba5a-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="eba5a-120">Not yet documented</span></span>|
|[<span data-ttu-id="eba5a-121">функция getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="eba5a-121">getMobileAppCount function</span></span>](../api/intune-apps-mobileapp-getmobileappcount.md)|<span data-ttu-id="eba5a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="eba5a-122">Int64</span></span>|<span data-ttu-id="eba5a-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="eba5a-123">Not yet documented</span></span>|
|[<span data-ttu-id="eba5a-124">функция getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="eba5a-124">getTopMobileApps function</span></span>](../api/intune-apps-mobileapp-gettopmobileapps.md)|<span data-ttu-id="eba5a-125">Коллекция [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eba5a-125">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="eba5a-126">Н/Д</span><span class="sxs-lookup"><span data-stu-id="eba5a-126">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="eba5a-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="eba5a-127">Properties</span></span>
|<span data-ttu-id="eba5a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="eba5a-128">Property</span></span>|<span data-ttu-id="eba5a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="eba5a-129">Type</span></span>|<span data-ttu-id="eba5a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="eba5a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eba5a-131">id</span><span class="sxs-lookup"><span data-stu-id="eba5a-131">id</span></span>|<span data-ttu-id="eba5a-132">String</span><span class="sxs-lookup"><span data-stu-id="eba5a-132">String</span></span>|<span data-ttu-id="eba5a-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eba5a-133">Key of the entity.</span></span>|
|<span data-ttu-id="eba5a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="eba5a-134">displayName</span></span>|<span data-ttu-id="eba5a-135">String</span><span class="sxs-lookup"><span data-stu-id="eba5a-135">String</span></span>|<span data-ttu-id="eba5a-136">Администратор предоставил или импортировал название приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-136">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="eba5a-137">описание</span><span class="sxs-lookup"><span data-stu-id="eba5a-137">description</span></span>|<span data-ttu-id="eba5a-138">String</span><span class="sxs-lookup"><span data-stu-id="eba5a-138">String</span></span>|<span data-ttu-id="eba5a-139">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-139">The description of the app.</span></span>|
|<span data-ttu-id="eba5a-140">publisher</span><span class="sxs-lookup"><span data-stu-id="eba5a-140">publisher</span></span>|<span data-ttu-id="eba5a-141">String</span><span class="sxs-lookup"><span data-stu-id="eba5a-141">String</span></span>|<span data-ttu-id="eba5a-142">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-142">The publisher of the app.</span></span>|
|<span data-ttu-id="eba5a-143">largeIcon</span><span class="sxs-lookup"><span data-stu-id="eba5a-143">largeIcon</span></span>|[<span data-ttu-id="eba5a-144">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eba5a-144">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eba5a-145">Большой значок, отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="eba5a-145">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="eba5a-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eba5a-146">createdDateTime</span></span>|<span data-ttu-id="eba5a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eba5a-147">DateTimeOffset</span></span>|<span data-ttu-id="eba5a-148">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-148">The date and time the app was created.</span></span>|
|<span data-ttu-id="eba5a-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eba5a-149">lastModifiedDateTime</span></span>|<span data-ttu-id="eba5a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eba5a-150">DateTimeOffset</span></span>|<span data-ttu-id="eba5a-151">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-151">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="eba5a-152">isFeatured</span><span class="sxs-lookup"><span data-stu-id="eba5a-152">isFeatured</span></span>|<span data-ttu-id="eba5a-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="eba5a-153">Boolean</span></span>|<span data-ttu-id="eba5a-154">Значение, которое показывает, отмечено ли приложение как подобранное администратором.</span><span class="sxs-lookup"><span data-stu-id="eba5a-154">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="eba5a-155">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eba5a-155">privacyInformationUrl</span></span>|<span data-ttu-id="eba5a-156">String</span><span class="sxs-lookup"><span data-stu-id="eba5a-156">String</span></span>|<span data-ttu-id="eba5a-157">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="eba5a-157">The privacy statement Url.</span></span>|
|<span data-ttu-id="eba5a-158">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eba5a-158">informationUrl</span></span>|<span data-ttu-id="eba5a-159">String</span><span class="sxs-lookup"><span data-stu-id="eba5a-159">String</span></span>|<span data-ttu-id="eba5a-160">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="eba5a-160">The more information Url.</span></span>|
|<span data-ttu-id="eba5a-161">owner</span><span class="sxs-lookup"><span data-stu-id="eba5a-161">owner</span></span>|<span data-ttu-id="eba5a-162">String</span><span class="sxs-lookup"><span data-stu-id="eba5a-162">String</span></span>|<span data-ttu-id="eba5a-163">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-163">The owner of the app.</span></span>|
|<span data-ttu-id="eba5a-164">developer</span><span class="sxs-lookup"><span data-stu-id="eba5a-164">developer</span></span>|<span data-ttu-id="eba5a-165">String</span><span class="sxs-lookup"><span data-stu-id="eba5a-165">String</span></span>|<span data-ttu-id="eba5a-166">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-166">The developer of the app.</span></span>|
|<span data-ttu-id="eba5a-167">notes</span><span class="sxs-lookup"><span data-stu-id="eba5a-167">notes</span></span>|<span data-ttu-id="eba5a-168">String</span><span class="sxs-lookup"><span data-stu-id="eba5a-168">String</span></span>|<span data-ttu-id="eba5a-169">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="eba5a-169">Notes for the app.</span></span>|
|<span data-ttu-id="eba5a-170">uploadState</span><span class="sxs-lookup"><span data-stu-id="eba5a-170">uploadState</span></span>|<span data-ttu-id="eba5a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="eba5a-171">Int32</span></span>|<span data-ttu-id="eba5a-172">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="eba5a-172">The upload state.</span></span>|
|<span data-ttu-id="eba5a-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="eba5a-173">publishingState</span></span>|[<span data-ttu-id="eba5a-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="eba5a-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="eba5a-175">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-175">The publishing state for the app.</span></span> <span data-ttu-id="eba5a-176">Приложение не может быть назначено, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="eba5a-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="eba5a-177">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="eba5a-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eba5a-178">Связи</span><span class="sxs-lookup"><span data-stu-id="eba5a-178">Relationships</span></span>
|<span data-ttu-id="eba5a-179">Связь</span><span class="sxs-lookup"><span data-stu-id="eba5a-179">Relationship</span></span>|<span data-ttu-id="eba5a-180">Тип</span><span class="sxs-lookup"><span data-stu-id="eba5a-180">Type</span></span>|<span data-ttu-id="eba5a-181">Описание</span><span class="sxs-lookup"><span data-stu-id="eba5a-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eba5a-182">categories</span><span class="sxs-lookup"><span data-stu-id="eba5a-182">categories</span></span>|<span data-ttu-id="eba5a-183">Коллекция объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="eba5a-183">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="eba5a-184">Список категорий для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-184">The list of categories for this app.</span></span>|
|<span data-ttu-id="eba5a-185">assignments</span><span class="sxs-lookup"><span data-stu-id="eba5a-185">assignments</span></span>|<span data-ttu-id="eba5a-186">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eba5a-186">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="eba5a-187">Список назначений группы для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-187">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="eba5a-188">installSummary</span><span class="sxs-lookup"><span data-stu-id="eba5a-188">installSummary</span></span>|<span data-ttu-id="eba5a-189">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);</span><span class="sxs-lookup"><span data-stu-id="eba5a-189">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)</span></span>|<span data-ttu-id="eba5a-190">Сводка по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-190">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="eba5a-191">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="eba5a-191">deviceStatuses</span></span>|<span data-ttu-id="eba5a-192">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="eba5a-192">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="eba5a-193">Список состояния установки для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-193">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="eba5a-194">userStatuses</span><span class="sxs-lookup"><span data-stu-id="eba5a-194">userStatuses</span></span>|<span data-ttu-id="eba5a-195">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="eba5a-195">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="eba5a-196">Список состояния установки для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="eba5a-196">The list of installation states for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eba5a-197">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eba5a-197">JSON Representation</span></span>
<span data-ttu-id="eba5a-198">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eba5a-198">Here is a JSON representation of the resource.</span></span>
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
  "uploadState": 1024,
  "publishingState": "String"
}
```





