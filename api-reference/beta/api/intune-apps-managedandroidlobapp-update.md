---
title: Update managedAndroidLobApp
description: Обновление свойств объекта managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3bbc94d183afd4fb9315261dbd7bec8af871ac09
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157311"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="f0973-103">Update managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="f0973-103">Update managedAndroidLobApp</span></span>

<span data-ttu-id="f0973-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0973-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0973-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0973-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0973-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0973-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0973-107">Обновление свойств объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-107">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0973-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f0973-108">Prerequisites</span></span>
<span data-ttu-id="f0973-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0973-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0973-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0973-111">Permission type</span></span>|<span data-ttu-id="f0973-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0973-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0973-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0973-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0973-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0973-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f0973-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0973-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0973-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0973-116">Not supported.</span></span>|
|<span data-ttu-id="f0973-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0973-117">Application</span></span>|<span data-ttu-id="f0973-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0973-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0973-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0973-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f0973-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f0973-120">Request headers</span></span>
|<span data-ttu-id="f0973-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0973-121">Header</span></span>|<span data-ttu-id="f0973-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0973-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0973-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0973-123">Authorization</span></span>|<span data-ttu-id="f0973-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0973-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0973-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0973-125">Accept</span></span>|<span data-ttu-id="f0973-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0973-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0973-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0973-127">Request body</span></span>
<span data-ttu-id="f0973-128">В теле запроса добавьте представление объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0973-128">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="f0973-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-129">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="f0973-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0973-130">Property</span></span>|<span data-ttu-id="f0973-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f0973-131">Type</span></span>|<span data-ttu-id="f0973-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f0973-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0973-133">id</span><span class="sxs-lookup"><span data-stu-id="f0973-133">id</span></span>|<span data-ttu-id="f0973-134">String</span><span class="sxs-lookup"><span data-stu-id="f0973-134">String</span></span>|<span data-ttu-id="f0973-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f0973-135">Key of the entity.</span></span> <span data-ttu-id="f0973-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f0973-137">displayName</span></span>|<span data-ttu-id="f0973-138">String</span><span class="sxs-lookup"><span data-stu-id="f0973-138">String</span></span>|<span data-ttu-id="f0973-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="f0973-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f0973-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-141">description</span><span class="sxs-lookup"><span data-stu-id="f0973-141">description</span></span>|<span data-ttu-id="f0973-142">String</span><span class="sxs-lookup"><span data-stu-id="f0973-142">String</span></span>|<span data-ttu-id="f0973-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-143">The description of the app.</span></span> <span data-ttu-id="f0973-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f0973-145">publisher</span></span>|<span data-ttu-id="f0973-146">String</span><span class="sxs-lookup"><span data-stu-id="f0973-146">String</span></span>|<span data-ttu-id="f0973-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-147">The publisher of the app.</span></span> <span data-ttu-id="f0973-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f0973-149">largeIcon</span></span>|[<span data-ttu-id="f0973-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f0973-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f0973-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f0973-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f0973-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0973-153">createdDateTime</span></span>|<span data-ttu-id="f0973-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0973-154">DateTimeOffset</span></span>|<span data-ttu-id="f0973-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-155">The date and time the app was created.</span></span> <span data-ttu-id="f0973-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0973-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f0973-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0973-158">DateTimeOffset</span></span>|<span data-ttu-id="f0973-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f0973-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f0973-161">isFeatured</span></span>|<span data-ttu-id="f0973-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0973-162">Boolean</span></span>|<span data-ttu-id="f0973-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f0973-164">privacyInformationUrl</span></span>|<span data-ttu-id="f0973-165">String</span><span class="sxs-lookup"><span data-stu-id="f0973-165">String</span></span>|<span data-ttu-id="f0973-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f0973-166">The privacy statement Url.</span></span> <span data-ttu-id="f0973-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f0973-168">informationUrl</span></span>|<span data-ttu-id="f0973-169">String</span><span class="sxs-lookup"><span data-stu-id="f0973-169">String</span></span>|<span data-ttu-id="f0973-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f0973-170">The more information Url.</span></span> <span data-ttu-id="f0973-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-172">owner</span><span class="sxs-lookup"><span data-stu-id="f0973-172">owner</span></span>|<span data-ttu-id="f0973-173">String</span><span class="sxs-lookup"><span data-stu-id="f0973-173">String</span></span>|<span data-ttu-id="f0973-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-174">The owner of the app.</span></span> <span data-ttu-id="f0973-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-176">developer</span><span class="sxs-lookup"><span data-stu-id="f0973-176">developer</span></span>|<span data-ttu-id="f0973-177">String</span><span class="sxs-lookup"><span data-stu-id="f0973-177">String</span></span>|<span data-ttu-id="f0973-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-178">The developer of the app.</span></span> <span data-ttu-id="f0973-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-180">notes</span><span class="sxs-lookup"><span data-stu-id="f0973-180">notes</span></span>|<span data-ttu-id="f0973-181">String</span><span class="sxs-lookup"><span data-stu-id="f0973-181">String</span></span>|<span data-ttu-id="f0973-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-182">Notes for the app.</span></span> <span data-ttu-id="f0973-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f0973-184">uploadState</span></span>|<span data-ttu-id="f0973-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f0973-185">Int32</span></span>|<span data-ttu-id="f0973-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="f0973-186">The upload state.</span></span> <span data-ttu-id="f0973-187">Возможные значения: 0- `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="f0973-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="f0973-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="f0973-189">publishingState</span></span>|[<span data-ttu-id="f0973-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f0973-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f0973-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-191">The publishing state for the app.</span></span> <span data-ttu-id="f0973-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f0973-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f0973-193">Наследуется от [mobileApp.](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0973-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f0973-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f0973-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f0973-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f0973-195">isAssigned</span></span>|<span data-ttu-id="f0973-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0973-196">Boolean</span></span>|<span data-ttu-id="f0973-197">Значение, указывающее, назначено ли приложению хотя бы одна группа.</span><span class="sxs-lookup"><span data-stu-id="f0973-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f0973-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0973-199">roleScopeTagIds</span></span>|<span data-ttu-id="f0973-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f0973-200">String collection</span></span>|<span data-ttu-id="f0973-201">Список ид тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f0973-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f0973-203">dependentAppCount</span></span>|<span data-ttu-id="f0973-204">Int32</span><span class="sxs-lookup"><span data-stu-id="f0973-204">Int32</span></span>|<span data-ttu-id="f0973-205">Общее количество зависимостей, которые есть у этого приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f0973-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="f0973-207">supersedingAppCount</span></span>|<span data-ttu-id="f0973-208">Int32</span><span class="sxs-lookup"><span data-stu-id="f0973-208">Int32</span></span>|<span data-ttu-id="f0973-209">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="f0973-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="f0973-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="f0973-211">supersededAppCount</span></span>|<span data-ttu-id="f0973-212">Int32</span><span class="sxs-lookup"><span data-stu-id="f0973-212">Int32</span></span>|<span data-ttu-id="f0973-213">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="f0973-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="f0973-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f0973-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f0973-215">appAvailability</span></span>|[<span data-ttu-id="f0973-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f0973-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f0973-217">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-217">The Application's availability.</span></span> <span data-ttu-id="f0973-218">Наследуется от [managedApp.](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f0973-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="f0973-219">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="f0973-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f0973-220">version</span><span class="sxs-lookup"><span data-stu-id="f0973-220">version</span></span>|<span data-ttu-id="f0973-221">String</span><span class="sxs-lookup"><span data-stu-id="f0973-221">String</span></span>|<span data-ttu-id="f0973-222">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-222">The Application's version.</span></span> <span data-ttu-id="f0973-223">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="f0973-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f0973-224">committedContentVersion</span></span>|<span data-ttu-id="f0973-225">String</span><span class="sxs-lookup"><span data-stu-id="f0973-225">String</span></span>|<span data-ttu-id="f0973-226">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="f0973-226">The internal committed content version.</span></span> <span data-ttu-id="f0973-227">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f0973-228">fileName</span><span class="sxs-lookup"><span data-stu-id="f0973-228">fileName</span></span>|<span data-ttu-id="f0973-229">String</span><span class="sxs-lookup"><span data-stu-id="f0973-229">String</span></span>|<span data-ttu-id="f0973-230">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="f0973-230">The name of the main Lob application file.</span></span> <span data-ttu-id="f0973-231">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f0973-232">size</span><span class="sxs-lookup"><span data-stu-id="f0973-232">size</span></span>|<span data-ttu-id="f0973-233">Int64</span><span class="sxs-lookup"><span data-stu-id="f0973-233">Int64</span></span>|<span data-ttu-id="f0973-234">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="f0973-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="f0973-235">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f0973-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f0973-236">packageId</span><span class="sxs-lookup"><span data-stu-id="f0973-236">packageId</span></span>|<span data-ttu-id="f0973-237">String</span><span class="sxs-lookup"><span data-stu-id="f0973-237">String</span></span>|<span data-ttu-id="f0973-238">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="f0973-238">The package identifier.</span></span>|
|<span data-ttu-id="f0973-239">identityName</span><span class="sxs-lookup"><span data-stu-id="f0973-239">identityName</span></span>|<span data-ttu-id="f0973-240">String</span><span class="sxs-lookup"><span data-stu-id="f0973-240">String</span></span>|<span data-ttu-id="f0973-241">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f0973-241">The Identity Name.</span></span>|
|<span data-ttu-id="f0973-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f0973-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f0973-243">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f0973-243">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="f0973-244">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="f0973-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f0973-245">versionName</span><span class="sxs-lookup"><span data-stu-id="f0973-245">versionName</span></span>|<span data-ttu-id="f0973-246">String</span><span class="sxs-lookup"><span data-stu-id="f0973-246">String</span></span>|<span data-ttu-id="f0973-247">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="f0973-247">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f0973-248">versionCode</span><span class="sxs-lookup"><span data-stu-id="f0973-248">versionCode</span></span>|<span data-ttu-id="f0973-249">String</span><span class="sxs-lookup"><span data-stu-id="f0973-249">String</span></span>|<span data-ttu-id="f0973-250">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="f0973-250">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f0973-251">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f0973-251">identityVersion</span></span>|<span data-ttu-id="f0973-252">String</span><span class="sxs-lookup"><span data-stu-id="f0973-252">String</span></span>|<span data-ttu-id="f0973-253">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f0973-253">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f0973-254">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0973-254">Response</span></span>
<span data-ttu-id="f0973-255">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f0973-255">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0973-256">Пример</span><span class="sxs-lookup"><span data-stu-id="f0973-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0973-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0973-257">Request</span></span>
<span data-ttu-id="f0973-258">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0973-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1588

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="f0973-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0973-259">Response</span></span>
<span data-ttu-id="f0973-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0973-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1760

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




