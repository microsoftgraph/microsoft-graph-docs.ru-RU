---
title: Тип ресурса mobileApp
description: Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7bdc0222f63a881ddf756b6fc436bbf5e49bd831
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466147"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="22032-103">Тип ресурса mobileApp</span><span class="sxs-lookup"><span data-stu-id="22032-103">mobileApp resource type</span></span>

<span data-ttu-id="22032-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22032-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22032-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22032-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22032-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22032-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22032-107">Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.</span><span class="sxs-lookup"><span data-stu-id="22032-107">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="22032-108">Методы</span><span class="sxs-lookup"><span data-stu-id="22032-108">Methods</span></span>
|<span data-ttu-id="22032-109">Метод</span><span class="sxs-lookup"><span data-stu-id="22032-109">Method</span></span>|<span data-ttu-id="22032-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="22032-110">Return Type</span></span>|<span data-ttu-id="22032-111">Описание</span><span class="sxs-lookup"><span data-stu-id="22032-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22032-112">Список mobileApps</span><span class="sxs-lookup"><span data-stu-id="22032-112">List mobileApps</span></span>](../api/intune-shared-mobileapp-list.md)|<span data-ttu-id="22032-113">Коллекция [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22032-113">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="22032-114">Список свойств и связей объектов [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22032-114">List properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="22032-115">Получение объекта mobileApp</span><span class="sxs-lookup"><span data-stu-id="22032-115">Get mobileApp</span></span>](../api/intune-shared-mobileapp-get.md)|[<span data-ttu-id="22032-116">mobileApp</span><span class="sxs-lookup"><span data-stu-id="22032-116">mobileApp</span></span>](../resources/intune-shared-mobileapp.md)|<span data-ttu-id="22032-117">Чтение свойств и связей объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="22032-117">Read properties and relationships of the [mobileApp](../resources/intune-shared-mobileapp.md) object.</span></span>|
|<span data-ttu-id="22032-118">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="22032-118">**Apps**</span></span>|
|[<span data-ttu-id="22032-119">Действие assign</span><span class="sxs-lookup"><span data-stu-id="22032-119">assign action</span></span>](../api/intune-shared-mobileapp-assign.md)|<span data-ttu-id="22032-120">Нет</span><span class="sxs-lookup"><span data-stu-id="22032-120">None</span></span>|<span data-ttu-id="22032-121">Н/Д</span><span class="sxs-lookup"><span data-stu-id="22032-121">Not yet documented</span></span>|
|[<span data-ttu-id="22032-122">Функция getMobileAppCount</span><span class="sxs-lookup"><span data-stu-id="22032-122">getMobileAppCount function</span></span>](../api/intune-shared-mobileapp-getmobileappcount.md)|<span data-ttu-id="22032-123">Int64</span><span class="sxs-lookup"><span data-stu-id="22032-123">Int64</span></span>|<span data-ttu-id="22032-124">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="22032-124">Not yet documented</span></span>|
|[<span data-ttu-id="22032-125">Функция getTopMobileApps</span><span class="sxs-lookup"><span data-stu-id="22032-125">getTopMobileApps function</span></span>](../api/intune-shared-mobileapp-gettopmobileapps.md)|<span data-ttu-id="22032-126">Коллекция [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="22032-126">[mobileApp](../resources/intune-shared-mobileapp.md) collection</span></span>|<span data-ttu-id="22032-127">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="22032-127">Not yet documented</span></span>|
|[<span data-ttu-id="22032-128">действие Упдатерелатионшипс</span><span class="sxs-lookup"><span data-stu-id="22032-128">updateRelationships action</span></span>](../api/intune-shared-mobileapp-updaterelationships.md)|<span data-ttu-id="22032-129">Нет</span><span class="sxs-lookup"><span data-stu-id="22032-129">None</span></span>|<span data-ttu-id="22032-130">Н/Д</span><span class="sxs-lookup"><span data-stu-id="22032-130">Not yet documented</span></span>|
|[<span data-ttu-id="22032-131">Функция Жетрелатедаппстатес</span><span class="sxs-lookup"><span data-stu-id="22032-131">getRelatedAppStates function</span></span>](../api/intune-shared-mobileapp-getrelatedappstates.md)|<span data-ttu-id="22032-132">Коллекция [мобилеаппрелатионшипстате](../resources/intune-apps-mobileapprelationshipstate.md)</span><span class="sxs-lookup"><span data-stu-id="22032-132">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection</span></span>|<span data-ttu-id="22032-133">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="22032-133">Not yet documented</span></span>|
|<span data-ttu-id="22032-134">**Набор политик**</span><span class="sxs-lookup"><span data-stu-id="22032-134">**Policy Set**</span></span>|
|[<span data-ttu-id="22032-135">действие Хаспайлоадлинкс</span><span class="sxs-lookup"><span data-stu-id="22032-135">hasPayloadLinks action</span></span>](../api/intune-shared-mobileapp-haspayloadlinks.md)|<span data-ttu-id="22032-136">Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="22032-136">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="22032-137">Н/Д</span><span class="sxs-lookup"><span data-stu-id="22032-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="22032-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="22032-138">Properties</span></span>
|<span data-ttu-id="22032-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="22032-139">Property</span></span>|<span data-ttu-id="22032-140">Тип</span><span class="sxs-lookup"><span data-stu-id="22032-140">Type</span></span>|<span data-ttu-id="22032-141">Описание</span><span class="sxs-lookup"><span data-stu-id="22032-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22032-142">id</span><span class="sxs-lookup"><span data-stu-id="22032-142">id</span></span>|<span data-ttu-id="22032-143">Строка</span><span class="sxs-lookup"><span data-stu-id="22032-143">String</span></span>|<span data-ttu-id="22032-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="22032-144">Key of the entity.</span></span>|
|<span data-ttu-id="22032-145">displayName</span><span class="sxs-lookup"><span data-stu-id="22032-145">displayName</span></span>|<span data-ttu-id="22032-146">Строка</span><span class="sxs-lookup"><span data-stu-id="22032-146">String</span></span>|<span data-ttu-id="22032-147">Администратор предоставил или импортировал название приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-147">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="22032-148">description</span><span class="sxs-lookup"><span data-stu-id="22032-148">description</span></span>|<span data-ttu-id="22032-149">Строка</span><span class="sxs-lookup"><span data-stu-id="22032-149">String</span></span>|<span data-ttu-id="22032-150">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-150">The description of the app.</span></span>|
|<span data-ttu-id="22032-151">publisher</span><span class="sxs-lookup"><span data-stu-id="22032-151">publisher</span></span>|<span data-ttu-id="22032-152">String</span><span class="sxs-lookup"><span data-stu-id="22032-152">String</span></span>|<span data-ttu-id="22032-153">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-153">The publisher of the app.</span></span>|
|<span data-ttu-id="22032-154">largeIcon</span><span class="sxs-lookup"><span data-stu-id="22032-154">largeIcon</span></span>|[<span data-ttu-id="22032-155">mimeContent</span><span class="sxs-lookup"><span data-stu-id="22032-155">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="22032-156">Большой значок, отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="22032-156">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="22032-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22032-157">createdDateTime</span></span>|<span data-ttu-id="22032-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22032-158">DateTimeOffset</span></span>|<span data-ttu-id="22032-159">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-159">The date and time the app was created.</span></span>|
|<span data-ttu-id="22032-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22032-160">lastModifiedDateTime</span></span>|<span data-ttu-id="22032-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22032-161">DateTimeOffset</span></span>|<span data-ttu-id="22032-162">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-162">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="22032-163">isFeatured</span><span class="sxs-lookup"><span data-stu-id="22032-163">isFeatured</span></span>|<span data-ttu-id="22032-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="22032-164">Boolean</span></span>|<span data-ttu-id="22032-165">Значение, которое показывает, отмечено ли приложение как подобранное администратором.</span><span class="sxs-lookup"><span data-stu-id="22032-165">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="22032-166">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="22032-166">privacyInformationUrl</span></span>|<span data-ttu-id="22032-167">String</span><span class="sxs-lookup"><span data-stu-id="22032-167">String</span></span>|<span data-ttu-id="22032-168">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="22032-168">The privacy statement Url.</span></span>|
|<span data-ttu-id="22032-169">informationUrl</span><span class="sxs-lookup"><span data-stu-id="22032-169">informationUrl</span></span>|<span data-ttu-id="22032-170">String</span><span class="sxs-lookup"><span data-stu-id="22032-170">String</span></span>|<span data-ttu-id="22032-171">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="22032-171">The more information Url.</span></span>|
|<span data-ttu-id="22032-172">owner</span><span class="sxs-lookup"><span data-stu-id="22032-172">owner</span></span>|<span data-ttu-id="22032-173">String</span><span class="sxs-lookup"><span data-stu-id="22032-173">String</span></span>|<span data-ttu-id="22032-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-174">The owner of the app.</span></span>|
|<span data-ttu-id="22032-175">developer</span><span class="sxs-lookup"><span data-stu-id="22032-175">developer</span></span>|<span data-ttu-id="22032-176">String</span><span class="sxs-lookup"><span data-stu-id="22032-176">String</span></span>|<span data-ttu-id="22032-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-177">The developer of the app.</span></span>|
|<span data-ttu-id="22032-178">notes</span><span class="sxs-lookup"><span data-stu-id="22032-178">notes</span></span>|<span data-ttu-id="22032-179">String</span><span class="sxs-lookup"><span data-stu-id="22032-179">String</span></span>|<span data-ttu-id="22032-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-180">Notes for the app.</span></span>|
|<span data-ttu-id="22032-181">uploadState</span><span class="sxs-lookup"><span data-stu-id="22032-181">uploadState</span></span>|<span data-ttu-id="22032-182">Int32</span><span class="sxs-lookup"><span data-stu-id="22032-182">Int32</span></span>|<span data-ttu-id="22032-183">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="22032-183">The upload state.</span></span>|
|<span data-ttu-id="22032-184">publishingState</span><span class="sxs-lookup"><span data-stu-id="22032-184">publishingState</span></span>|[<span data-ttu-id="22032-185">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="22032-185">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="22032-186">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-186">The publishing state for the app.</span></span> <span data-ttu-id="22032-187">Приложение не может быть назначено, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="22032-187">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="22032-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="22032-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="22032-189">isAssigned</span><span class="sxs-lookup"><span data-stu-id="22032-189">isAssigned</span></span>|<span data-ttu-id="22032-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="22032-190">Boolean</span></span>|<span data-ttu-id="22032-191">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="22032-191">The value indicating whether the app is assigned to at least one group.</span></span>|
|<span data-ttu-id="22032-192">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22032-192">roleScopeTagIds</span></span>|<span data-ttu-id="22032-193">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="22032-193">String collection</span></span>|<span data-ttu-id="22032-194">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-194">List of scope tag ids for this mobile app.</span></span>|
|<span data-ttu-id="22032-195">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="22032-195">dependentAppCount</span></span>|<span data-ttu-id="22032-196">Int32</span><span class="sxs-lookup"><span data-stu-id="22032-196">Int32</span></span>|<span data-ttu-id="22032-197">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-197">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22032-198">Отношения</span><span class="sxs-lookup"><span data-stu-id="22032-198">Relationships</span></span>
|<span data-ttu-id="22032-199">Связь</span><span class="sxs-lookup"><span data-stu-id="22032-199">Relationship</span></span>|<span data-ttu-id="22032-200">Тип</span><span class="sxs-lookup"><span data-stu-id="22032-200">Type</span></span>|<span data-ttu-id="22032-201">Описание</span><span class="sxs-lookup"><span data-stu-id="22032-201">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22032-202">**Приложения**</span><span class="sxs-lookup"><span data-stu-id="22032-202">**Apps**</span></span>|
|<span data-ttu-id="22032-203">categories</span><span class="sxs-lookup"><span data-stu-id="22032-203">categories</span></span>|<span data-ttu-id="22032-204">Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)</span><span class="sxs-lookup"><span data-stu-id="22032-204">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="22032-205">Список категорий для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-205">The list of categories for this app.</span></span>|
|<span data-ttu-id="22032-206">assignments</span><span class="sxs-lookup"><span data-stu-id="22032-206">assignments</span></span>|<span data-ttu-id="22032-207">Коллекция [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="22032-207">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="22032-208">Список назначений группы для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-208">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="22032-209">installSummary</span><span class="sxs-lookup"><span data-stu-id="22032-209">installSummary</span></span>|<span data-ttu-id="22032-210">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);</span><span class="sxs-lookup"><span data-stu-id="22032-210">[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)</span></span>|<span data-ttu-id="22032-211">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-211">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="22032-212">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="22032-212">deviceStatuses</span></span>|<span data-ttu-id="22032-213">Коллекция [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="22032-213">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="22032-214">Список состояний установки для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-214">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="22032-215">userStatuses</span><span class="sxs-lookup"><span data-stu-id="22032-215">userStatuses</span></span>|<span data-ttu-id="22032-216">Коллекция [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="22032-216">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="22032-217">Список состояний установки для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-217">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="22032-218">Таблица</span><span class="sxs-lookup"><span data-stu-id="22032-218">relationships</span></span>|<span data-ttu-id="22032-219">Коллекция [мобилеаппрелатионшип](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="22032-219">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="22032-220">Список отношений для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="22032-220">List of relationships for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22032-221">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22032-221">JSON Representation</span></span>
<span data-ttu-id="22032-222">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22032-222">Here is a JSON representation of the resource.</span></span>
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
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024
}
```



