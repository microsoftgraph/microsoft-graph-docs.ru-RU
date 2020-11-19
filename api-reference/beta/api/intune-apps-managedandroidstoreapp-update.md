---
title: Update managedAndroidStoreApp
description: Обновление свойств объекта managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01d8c2125e3059e6393d22a640276577dad9e1e5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49250613"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="47923-103">Update managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="47923-103">Update managedAndroidStoreApp</span></span>

<span data-ttu-id="47923-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47923-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47923-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47923-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47923-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47923-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47923-107">Обновление свойств объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-107">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47923-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="47923-108">Prerequisites</span></span>
<span data-ttu-id="47923-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47923-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47923-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47923-111">Permission type</span></span>|<span data-ttu-id="47923-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47923-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47923-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47923-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47923-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47923-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="47923-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47923-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47923-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47923-116">Not supported.</span></span>|
|<span data-ttu-id="47923-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="47923-117">Application</span></span>|<span data-ttu-id="47923-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47923-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47923-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47923-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="47923-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="47923-120">Request headers</span></span>
|<span data-ttu-id="47923-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47923-121">Header</span></span>|<span data-ttu-id="47923-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47923-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47923-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47923-123">Authorization</span></span>|<span data-ttu-id="47923-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47923-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47923-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47923-125">Accept</span></span>|<span data-ttu-id="47923-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47923-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47923-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47923-127">Request body</span></span>
<span data-ttu-id="47923-128">В теле запроса добавьте представление объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47923-128">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="47923-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-129">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="47923-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="47923-130">Property</span></span>|<span data-ttu-id="47923-131">Тип</span><span class="sxs-lookup"><span data-stu-id="47923-131">Type</span></span>|<span data-ttu-id="47923-132">Описание</span><span class="sxs-lookup"><span data-stu-id="47923-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47923-133">id</span><span class="sxs-lookup"><span data-stu-id="47923-133">id</span></span>|<span data-ttu-id="47923-134">String</span><span class="sxs-lookup"><span data-stu-id="47923-134">String</span></span>|<span data-ttu-id="47923-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47923-135">Key of the entity.</span></span> <span data-ttu-id="47923-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-137">displayName</span><span class="sxs-lookup"><span data-stu-id="47923-137">displayName</span></span>|<span data-ttu-id="47923-138">String</span><span class="sxs-lookup"><span data-stu-id="47923-138">String</span></span>|<span data-ttu-id="47923-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="47923-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="47923-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-141">description</span><span class="sxs-lookup"><span data-stu-id="47923-141">description</span></span>|<span data-ttu-id="47923-142">String</span><span class="sxs-lookup"><span data-stu-id="47923-142">String</span></span>|<span data-ttu-id="47923-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-143">The description of the app.</span></span> <span data-ttu-id="47923-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-145">publisher</span><span class="sxs-lookup"><span data-stu-id="47923-145">publisher</span></span>|<span data-ttu-id="47923-146">String</span><span class="sxs-lookup"><span data-stu-id="47923-146">String</span></span>|<span data-ttu-id="47923-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-147">The publisher of the app.</span></span> <span data-ttu-id="47923-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="47923-149">largeIcon</span></span>|[<span data-ttu-id="47923-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="47923-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="47923-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="47923-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="47923-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47923-153">createdDateTime</span></span>|<span data-ttu-id="47923-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47923-154">DateTimeOffset</span></span>|<span data-ttu-id="47923-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-155">The date and time the app was created.</span></span> <span data-ttu-id="47923-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47923-157">lastModifiedDateTime</span></span>|<span data-ttu-id="47923-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47923-158">DateTimeOffset</span></span>|<span data-ttu-id="47923-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-159">The date and time the app was last modified.</span></span> <span data-ttu-id="47923-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="47923-161">isFeatured</span></span>|<span data-ttu-id="47923-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="47923-162">Boolean</span></span>|<span data-ttu-id="47923-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="47923-164">privacyInformationUrl</span></span>|<span data-ttu-id="47923-165">String</span><span class="sxs-lookup"><span data-stu-id="47923-165">String</span></span>|<span data-ttu-id="47923-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="47923-166">The privacy statement Url.</span></span> <span data-ttu-id="47923-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="47923-168">informationUrl</span></span>|<span data-ttu-id="47923-169">String</span><span class="sxs-lookup"><span data-stu-id="47923-169">String</span></span>|<span data-ttu-id="47923-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="47923-170">The more information Url.</span></span> <span data-ttu-id="47923-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-172">owner</span><span class="sxs-lookup"><span data-stu-id="47923-172">owner</span></span>|<span data-ttu-id="47923-173">String</span><span class="sxs-lookup"><span data-stu-id="47923-173">String</span></span>|<span data-ttu-id="47923-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-174">The owner of the app.</span></span> <span data-ttu-id="47923-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-176">developer</span><span class="sxs-lookup"><span data-stu-id="47923-176">developer</span></span>|<span data-ttu-id="47923-177">String</span><span class="sxs-lookup"><span data-stu-id="47923-177">String</span></span>|<span data-ttu-id="47923-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-178">The developer of the app.</span></span> <span data-ttu-id="47923-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-180">notes</span><span class="sxs-lookup"><span data-stu-id="47923-180">notes</span></span>|<span data-ttu-id="47923-181">String</span><span class="sxs-lookup"><span data-stu-id="47923-181">String</span></span>|<span data-ttu-id="47923-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-182">Notes for the app.</span></span> <span data-ttu-id="47923-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="47923-184">uploadState</span></span>|<span data-ttu-id="47923-185">Int32</span><span class="sxs-lookup"><span data-stu-id="47923-185">Int32</span></span>|<span data-ttu-id="47923-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="47923-186">The upload state.</span></span> <span data-ttu-id="47923-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="47923-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="47923-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="47923-189">publishingState</span></span>|[<span data-ttu-id="47923-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="47923-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="47923-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-191">The publishing state for the app.</span></span> <span data-ttu-id="47923-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="47923-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="47923-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="47923-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="47923-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="47923-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="47923-195">isAssigned</span></span>|<span data-ttu-id="47923-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="47923-196">Boolean</span></span>|<span data-ttu-id="47923-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="47923-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="47923-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47923-199">roleScopeTagIds</span></span>|<span data-ttu-id="47923-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="47923-200">String collection</span></span>|<span data-ttu-id="47923-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="47923-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="47923-203">dependentAppCount</span></span>|<span data-ttu-id="47923-204">Int32</span><span class="sxs-lookup"><span data-stu-id="47923-204">Int32</span></span>|<span data-ttu-id="47923-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="47923-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="47923-207">supersedingAppCount</span></span>|<span data-ttu-id="47923-208">Int32</span><span class="sxs-lookup"><span data-stu-id="47923-208">Int32</span></span>|<span data-ttu-id="47923-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="47923-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="47923-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="47923-211">supersededAppCount</span></span>|<span data-ttu-id="47923-212">Int32</span><span class="sxs-lookup"><span data-stu-id="47923-212">Int32</span></span>|<span data-ttu-id="47923-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="47923-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="47923-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47923-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="47923-215">appAvailability</span></span>|[<span data-ttu-id="47923-216">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="47923-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="47923-217">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-217">The Application's availability.</span></span> <span data-ttu-id="47923-218">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="47923-219">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="47923-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="47923-220">version</span><span class="sxs-lookup"><span data-stu-id="47923-220">version</span></span>|<span data-ttu-id="47923-221">String</span><span class="sxs-lookup"><span data-stu-id="47923-221">String</span></span>|<span data-ttu-id="47923-222">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-222">The Application's version.</span></span> <span data-ttu-id="47923-223">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="47923-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="47923-224">packageId</span><span class="sxs-lookup"><span data-stu-id="47923-224">packageId</span></span>|<span data-ttu-id="47923-225">String</span><span class="sxs-lookup"><span data-stu-id="47923-225">String</span></span>|<span data-ttu-id="47923-226">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="47923-226">The app's package ID.</span></span>|
|<span data-ttu-id="47923-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="47923-227">appStoreUrl</span></span>|<span data-ttu-id="47923-228">String</span><span class="sxs-lookup"><span data-stu-id="47923-228">String</span></span>|<span data-ttu-id="47923-229">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="47923-229">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="47923-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="47923-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="47923-231">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="47923-231">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="47923-232">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="47923-232">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="47923-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="47923-233">Response</span></span>
<span data-ttu-id="47923-234">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="47923-234">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47923-235">Пример</span><span class="sxs-lookup"><span data-stu-id="47923-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="47923-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="47923-236">Request</span></span>
<span data-ttu-id="47923-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47923-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1321

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
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="47923-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="47923-238">Response</span></span>
<span data-ttu-id="47923-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47923-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1493

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
    "v9_0": true
  }
}
```




