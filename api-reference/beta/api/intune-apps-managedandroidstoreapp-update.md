---
title: Update managedAndroidStoreApp
description: Обновление свойств объекта managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1ad1a1983cb83159ea9c3a17361635ad85c0f23a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140274"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="c064e-103">Update managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="c064e-103">Update managedAndroidStoreApp</span></span>

<span data-ttu-id="c064e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c064e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c064e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c064e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c064e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c064e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c064e-107">Обновление свойств объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-107">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c064e-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c064e-108">Prerequisites</span></span>
<span data-ttu-id="c064e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c064e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c064e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c064e-111">Permission type</span></span>|<span data-ttu-id="c064e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c064e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c064e-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c064e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c064e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c064e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c064e-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c064e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c064e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c064e-116">Not supported.</span></span>|
|<span data-ttu-id="c064e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c064e-117">Application</span></span>|<span data-ttu-id="c064e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c064e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c064e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c064e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="c064e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c064e-120">Request headers</span></span>
|<span data-ttu-id="c064e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c064e-121">Header</span></span>|<span data-ttu-id="c064e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c064e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c064e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c064e-123">Authorization</span></span>|<span data-ttu-id="c064e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c064e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c064e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c064e-125">Accept</span></span>|<span data-ttu-id="c064e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c064e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c064e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c064e-127">Request body</span></span>
<span data-ttu-id="c064e-128">В теле запроса добавьте представление объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c064e-128">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="c064e-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-129">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="c064e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c064e-130">Property</span></span>|<span data-ttu-id="c064e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c064e-131">Type</span></span>|<span data-ttu-id="c064e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c064e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c064e-133">id</span><span class="sxs-lookup"><span data-stu-id="c064e-133">id</span></span>|<span data-ttu-id="c064e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c064e-134">String</span></span>|<span data-ttu-id="c064e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c064e-135">Key of the entity.</span></span> <span data-ttu-id="c064e-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c064e-137">displayName</span></span>|<span data-ttu-id="c064e-138">Строка</span><span class="sxs-lookup"><span data-stu-id="c064e-138">String</span></span>|<span data-ttu-id="c064e-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c064e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c064e-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-141">description</span><span class="sxs-lookup"><span data-stu-id="c064e-141">description</span></span>|<span data-ttu-id="c064e-142">Строка</span><span class="sxs-lookup"><span data-stu-id="c064e-142">String</span></span>|<span data-ttu-id="c064e-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c064e-143">The description of the app.</span></span> <span data-ttu-id="c064e-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c064e-145">publisher</span></span>|<span data-ttu-id="c064e-146">String</span><span class="sxs-lookup"><span data-stu-id="c064e-146">String</span></span>|<span data-ttu-id="c064e-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c064e-147">The publisher of the app.</span></span> <span data-ttu-id="c064e-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c064e-149">largeIcon</span></span>|[<span data-ttu-id="c064e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c064e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c064e-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="c064e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c064e-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c064e-153">createdDateTime</span></span>|<span data-ttu-id="c064e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c064e-154">DateTimeOffset</span></span>|<span data-ttu-id="c064e-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="c064e-155">The date and time the app was created.</span></span> <span data-ttu-id="c064e-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c064e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c064e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c064e-158">DateTimeOffset</span></span>|<span data-ttu-id="c064e-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="c064e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c064e-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c064e-161">isFeatured</span></span>|<span data-ttu-id="c064e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c064e-162">Boolean</span></span>|<span data-ttu-id="c064e-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c064e-164">privacyInformationUrl</span></span>|<span data-ttu-id="c064e-165">String</span><span class="sxs-lookup"><span data-stu-id="c064e-165">String</span></span>|<span data-ttu-id="c064e-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c064e-166">The privacy statement Url.</span></span> <span data-ttu-id="c064e-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c064e-168">informationUrl</span></span>|<span data-ttu-id="c064e-169">String</span><span class="sxs-lookup"><span data-stu-id="c064e-169">String</span></span>|<span data-ttu-id="c064e-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="c064e-170">The more information Url.</span></span> <span data-ttu-id="c064e-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-172">owner</span><span class="sxs-lookup"><span data-stu-id="c064e-172">owner</span></span>|<span data-ttu-id="c064e-173">String</span><span class="sxs-lookup"><span data-stu-id="c064e-173">String</span></span>|<span data-ttu-id="c064e-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="c064e-174">The owner of the app.</span></span> <span data-ttu-id="c064e-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-176">developer</span><span class="sxs-lookup"><span data-stu-id="c064e-176">developer</span></span>|<span data-ttu-id="c064e-177">String</span><span class="sxs-lookup"><span data-stu-id="c064e-177">String</span></span>|<span data-ttu-id="c064e-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="c064e-178">The developer of the app.</span></span> <span data-ttu-id="c064e-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-180">notes</span><span class="sxs-lookup"><span data-stu-id="c064e-180">notes</span></span>|<span data-ttu-id="c064e-181">String</span><span class="sxs-lookup"><span data-stu-id="c064e-181">String</span></span>|<span data-ttu-id="c064e-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="c064e-182">Notes for the app.</span></span> <span data-ttu-id="c064e-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c064e-184">uploadState</span></span>|<span data-ttu-id="c064e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c064e-185">Int32</span></span>|<span data-ttu-id="c064e-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="c064e-186">The upload state.</span></span> <span data-ttu-id="c064e-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="c064e-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="c064e-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="c064e-189">publishingState</span></span>|[<span data-ttu-id="c064e-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c064e-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c064e-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="c064e-191">The publishing state for the app.</span></span> <span data-ttu-id="c064e-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="c064e-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c064e-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="c064e-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c064e-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c064e-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c064e-195">isAssigned</span></span>|<span data-ttu-id="c064e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="c064e-196">Boolean</span></span>|<span data-ttu-id="c064e-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="c064e-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c064e-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c064e-199">roleScopeTagIds</span></span>|<span data-ttu-id="c064e-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c064e-200">String collection</span></span>|<span data-ttu-id="c064e-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="c064e-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c064e-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="c064e-203">dependentAppCount</span></span>|<span data-ttu-id="c064e-204">Int32</span><span class="sxs-lookup"><span data-stu-id="c064e-204">Int32</span></span>|<span data-ttu-id="c064e-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="c064e-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="c064e-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="c064e-207">supersedingAppCount</span></span>|<span data-ttu-id="c064e-208">Int32</span><span class="sxs-lookup"><span data-stu-id="c064e-208">Int32</span></span>|<span data-ttu-id="c064e-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="c064e-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="c064e-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="c064e-211">supersededAppCount</span></span>|<span data-ttu-id="c064e-212">Int32</span><span class="sxs-lookup"><span data-stu-id="c064e-212">Int32</span></span>|<span data-ttu-id="c064e-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="c064e-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="c064e-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c064e-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="c064e-215">appAvailability</span></span>|[<span data-ttu-id="c064e-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="c064e-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="c064e-217">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="c064e-217">The Application's availability.</span></span> <span data-ttu-id="c064e-218">Унаследованный от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="c064e-219">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="c064e-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="c064e-220">version</span><span class="sxs-lookup"><span data-stu-id="c064e-220">version</span></span>|<span data-ttu-id="c064e-221">String</span><span class="sxs-lookup"><span data-stu-id="c064e-221">String</span></span>|<span data-ttu-id="c064e-222">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="c064e-222">The Application's version.</span></span> <span data-ttu-id="c064e-223">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c064e-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="c064e-224">packageId</span><span class="sxs-lookup"><span data-stu-id="c064e-224">packageId</span></span>|<span data-ttu-id="c064e-225">String</span><span class="sxs-lookup"><span data-stu-id="c064e-225">String</span></span>|<span data-ttu-id="c064e-226">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="c064e-226">The app's package ID.</span></span>|
|<span data-ttu-id="c064e-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c064e-227">appStoreUrl</span></span>|<span data-ttu-id="c064e-228">String</span><span class="sxs-lookup"><span data-stu-id="c064e-228">String</span></span>|<span data-ttu-id="c064e-229">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="c064e-229">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="c064e-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c064e-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c064e-231">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c064e-231">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="c064e-232">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="c064e-232">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="c064e-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="c064e-233">Response</span></span>
<span data-ttu-id="c064e-234">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c064e-234">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c064e-235">Пример</span><span class="sxs-lookup"><span data-stu-id="c064e-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="c064e-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="c064e-236">Request</span></span>
<span data-ttu-id="c064e-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c064e-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1361

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="c064e-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="c064e-238">Response</span></span>
<span data-ttu-id="c064e-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c064e-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1533

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```




