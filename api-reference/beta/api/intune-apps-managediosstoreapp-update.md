---
title: Обновление managedIOSStoreApp
description: Обновляет свойства объекта managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba7ad1ce33a77b93dd029483261bce1fb514881c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980829"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="02e72-103">Обновление managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="02e72-103">Update managedIOSStoreApp</span></span>

<span data-ttu-id="02e72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02e72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02e72-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02e72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02e72-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02e72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02e72-107">Обновляет свойства объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-107">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02e72-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="02e72-108">Prerequisites</span></span>
<span data-ttu-id="02e72-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02e72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02e72-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02e72-111">Permission type</span></span>|<span data-ttu-id="02e72-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="02e72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02e72-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02e72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02e72-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02e72-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="02e72-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02e72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02e72-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02e72-116">Not supported.</span></span>|
|<span data-ttu-id="02e72-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02e72-117">Application</span></span>|<span data-ttu-id="02e72-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02e72-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02e72-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02e72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="02e72-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="02e72-120">Request headers</span></span>
|<span data-ttu-id="02e72-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02e72-121">Header</span></span>|<span data-ttu-id="02e72-122">Значение</span><span class="sxs-lookup"><span data-stu-id="02e72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02e72-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02e72-123">Authorization</span></span>|<span data-ttu-id="02e72-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02e72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02e72-125">Accept</span><span class="sxs-lookup"><span data-stu-id="02e72-125">Accept</span></span>|<span data-ttu-id="02e72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02e72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02e72-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="02e72-127">Request body</span></span>
<span data-ttu-id="02e72-128">В теле запроса добавьте представление объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02e72-128">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="02e72-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-129">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="02e72-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="02e72-130">Property</span></span>|<span data-ttu-id="02e72-131">Тип</span><span class="sxs-lookup"><span data-stu-id="02e72-131">Type</span></span>|<span data-ttu-id="02e72-132">Описание</span><span class="sxs-lookup"><span data-stu-id="02e72-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02e72-133">id</span><span class="sxs-lookup"><span data-stu-id="02e72-133">id</span></span>|<span data-ttu-id="02e72-134">String</span><span class="sxs-lookup"><span data-stu-id="02e72-134">String</span></span>|<span data-ttu-id="02e72-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="02e72-135">Key of the entity.</span></span> <span data-ttu-id="02e72-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-137">displayName</span><span class="sxs-lookup"><span data-stu-id="02e72-137">displayName</span></span>|<span data-ttu-id="02e72-138">String</span><span class="sxs-lookup"><span data-stu-id="02e72-138">String</span></span>|<span data-ttu-id="02e72-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="02e72-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="02e72-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-141">description</span><span class="sxs-lookup"><span data-stu-id="02e72-141">description</span></span>|<span data-ttu-id="02e72-142">String</span><span class="sxs-lookup"><span data-stu-id="02e72-142">String</span></span>|<span data-ttu-id="02e72-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-143">The description of the app.</span></span> <span data-ttu-id="02e72-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-145">publisher</span><span class="sxs-lookup"><span data-stu-id="02e72-145">publisher</span></span>|<span data-ttu-id="02e72-146">String</span><span class="sxs-lookup"><span data-stu-id="02e72-146">String</span></span>|<span data-ttu-id="02e72-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-147">The publisher of the app.</span></span> <span data-ttu-id="02e72-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="02e72-149">largeIcon</span></span>|[<span data-ttu-id="02e72-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="02e72-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="02e72-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="02e72-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="02e72-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02e72-153">createdDateTime</span></span>|<span data-ttu-id="02e72-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02e72-154">DateTimeOffset</span></span>|<span data-ttu-id="02e72-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-155">The date and time the app was created.</span></span> <span data-ttu-id="02e72-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02e72-157">lastModifiedDateTime</span></span>|<span data-ttu-id="02e72-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02e72-158">DateTimeOffset</span></span>|<span data-ttu-id="02e72-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-159">The date and time the app was last modified.</span></span> <span data-ttu-id="02e72-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="02e72-161">isFeatured</span></span>|<span data-ttu-id="02e72-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="02e72-162">Boolean</span></span>|<span data-ttu-id="02e72-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="02e72-164">privacyInformationUrl</span></span>|<span data-ttu-id="02e72-165">String</span><span class="sxs-lookup"><span data-stu-id="02e72-165">String</span></span>|<span data-ttu-id="02e72-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="02e72-166">The privacy statement Url.</span></span> <span data-ttu-id="02e72-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="02e72-168">informationUrl</span></span>|<span data-ttu-id="02e72-169">String</span><span class="sxs-lookup"><span data-stu-id="02e72-169">String</span></span>|<span data-ttu-id="02e72-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="02e72-170">The more information Url.</span></span> <span data-ttu-id="02e72-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-172">owner</span><span class="sxs-lookup"><span data-stu-id="02e72-172">owner</span></span>|<span data-ttu-id="02e72-173">String</span><span class="sxs-lookup"><span data-stu-id="02e72-173">String</span></span>|<span data-ttu-id="02e72-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-174">The owner of the app.</span></span> <span data-ttu-id="02e72-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-176">developer</span><span class="sxs-lookup"><span data-stu-id="02e72-176">developer</span></span>|<span data-ttu-id="02e72-177">String</span><span class="sxs-lookup"><span data-stu-id="02e72-177">String</span></span>|<span data-ttu-id="02e72-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-178">The developer of the app.</span></span> <span data-ttu-id="02e72-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-180">notes</span><span class="sxs-lookup"><span data-stu-id="02e72-180">notes</span></span>|<span data-ttu-id="02e72-181">String</span><span class="sxs-lookup"><span data-stu-id="02e72-181">String</span></span>|<span data-ttu-id="02e72-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-182">Notes for the app.</span></span> <span data-ttu-id="02e72-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="02e72-184">uploadState</span></span>|<span data-ttu-id="02e72-185">Int32</span><span class="sxs-lookup"><span data-stu-id="02e72-185">Int32</span></span>|<span data-ttu-id="02e72-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="02e72-186">The upload state.</span></span> <span data-ttu-id="02e72-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="02e72-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="02e72-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="02e72-189">publishingState</span></span>|[<span data-ttu-id="02e72-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="02e72-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="02e72-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-191">The publishing state for the app.</span></span> <span data-ttu-id="02e72-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="02e72-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="02e72-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="02e72-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="02e72-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="02e72-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="02e72-195">isAssigned</span></span>|<span data-ttu-id="02e72-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="02e72-196">Boolean</span></span>|<span data-ttu-id="02e72-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="02e72-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="02e72-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="02e72-199">roleScopeTagIds</span></span>|<span data-ttu-id="02e72-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="02e72-200">String collection</span></span>|<span data-ttu-id="02e72-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="02e72-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="02e72-203">dependentAppCount</span></span>|<span data-ttu-id="02e72-204">Int32</span><span class="sxs-lookup"><span data-stu-id="02e72-204">Int32</span></span>|<span data-ttu-id="02e72-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="02e72-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="02e72-207">supersedingAppCount</span></span>|<span data-ttu-id="02e72-208">Int32</span><span class="sxs-lookup"><span data-stu-id="02e72-208">Int32</span></span>|<span data-ttu-id="02e72-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="02e72-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="02e72-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="02e72-211">supersededAppCount</span></span>|<span data-ttu-id="02e72-212">Int32</span><span class="sxs-lookup"><span data-stu-id="02e72-212">Int32</span></span>|<span data-ttu-id="02e72-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="02e72-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="02e72-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="02e72-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="02e72-215">appAvailability</span></span>|[<span data-ttu-id="02e72-216">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="02e72-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="02e72-217">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-217">The Application's availability.</span></span> <span data-ttu-id="02e72-218">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="02e72-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="02e72-219">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="02e72-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="02e72-220">version</span><span class="sxs-lookup"><span data-stu-id="02e72-220">version</span></span>|<span data-ttu-id="02e72-221">String</span><span class="sxs-lookup"><span data-stu-id="02e72-221">String</span></span>|<span data-ttu-id="02e72-222">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-222">The Application's version.</span></span> <span data-ttu-id="02e72-223">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="02e72-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="02e72-224">bundleId</span><span class="sxs-lookup"><span data-stu-id="02e72-224">bundleId</span></span>|<span data-ttu-id="02e72-225">String</span><span class="sxs-lookup"><span data-stu-id="02e72-225">String</span></span>|<span data-ttu-id="02e72-226">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="02e72-226">The app's Bundle ID.</span></span>|
|<span data-ttu-id="02e72-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="02e72-227">appStoreUrl</span></span>|<span data-ttu-id="02e72-228">String</span><span class="sxs-lookup"><span data-stu-id="02e72-228">String</span></span>|<span data-ttu-id="02e72-229">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="02e72-229">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="02e72-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="02e72-230">applicableDeviceType</span></span>|[<span data-ttu-id="02e72-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="02e72-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="02e72-232">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="02e72-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="02e72-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="02e72-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="02e72-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="02e72-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="02e72-235">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="02e72-235">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="02e72-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="02e72-236">Response</span></span>
<span data-ttu-id="02e72-237">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="02e72-237">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02e72-238">Пример</span><span class="sxs-lookup"><span data-stu-id="02e72-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="02e72-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="02e72-239">Request</span></span>
<span data-ttu-id="02e72-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02e72-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1295

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="02e72-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="02e72-241">Response</span></span>
<span data-ttu-id="02e72-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02e72-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1467

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  }
}
```






