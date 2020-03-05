---
title: Update microsoftStoreForBusinessApp
description: Обновление свойств объекта microsoftStoreForBusinessApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 67c5d9ddd8bd6d703f22d7a883f37234f15b4192
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445038"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="95db7-103">Update microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="95db7-103">Update microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="95db7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="95db7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95db7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95db7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95db7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95db7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95db7-107">Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-107">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95db7-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="95db7-108">Prerequisites</span></span>
<span data-ttu-id="95db7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95db7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95db7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95db7-111">Permission type</span></span>|<span data-ttu-id="95db7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95db7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95db7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95db7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95db7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95db7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95db7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95db7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95db7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95db7-116">Not supported.</span></span>|
|<span data-ttu-id="95db7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95db7-117">Application</span></span>|<span data-ttu-id="95db7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95db7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95db7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95db7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="95db7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="95db7-120">Request headers</span></span>
|<span data-ttu-id="95db7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95db7-121">Header</span></span>|<span data-ttu-id="95db7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="95db7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95db7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95db7-123">Authorization</span></span>|<span data-ttu-id="95db7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95db7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95db7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95db7-125">Accept</span></span>|<span data-ttu-id="95db7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95db7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95db7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95db7-127">Request body</span></span>
<span data-ttu-id="95db7-128">В теле запроса добавьте представление объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95db7-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="95db7-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="95db7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="95db7-130">Property</span></span>|<span data-ttu-id="95db7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="95db7-131">Type</span></span>|<span data-ttu-id="95db7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="95db7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95db7-133">id</span><span class="sxs-lookup"><span data-stu-id="95db7-133">id</span></span>|<span data-ttu-id="95db7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="95db7-134">String</span></span>|<span data-ttu-id="95db7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="95db7-135">Key of the entity.</span></span> <span data-ttu-id="95db7-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="95db7-137">displayName</span></span>|<span data-ttu-id="95db7-138">Строка</span><span class="sxs-lookup"><span data-stu-id="95db7-138">String</span></span>|<span data-ttu-id="95db7-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="95db7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="95db7-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-141">description</span><span class="sxs-lookup"><span data-stu-id="95db7-141">description</span></span>|<span data-ttu-id="95db7-142">String</span><span class="sxs-lookup"><span data-stu-id="95db7-142">String</span></span>|<span data-ttu-id="95db7-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="95db7-143">The description of the app.</span></span> <span data-ttu-id="95db7-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="95db7-145">publisher</span></span>|<span data-ttu-id="95db7-146">String</span><span class="sxs-lookup"><span data-stu-id="95db7-146">String</span></span>|<span data-ttu-id="95db7-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="95db7-147">The publisher of the app.</span></span> <span data-ttu-id="95db7-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="95db7-149">largeIcon</span></span>|[<span data-ttu-id="95db7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="95db7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="95db7-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="95db7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="95db7-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95db7-153">createdDateTime</span></span>|<span data-ttu-id="95db7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95db7-154">DateTimeOffset</span></span>|<span data-ttu-id="95db7-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="95db7-155">The date and time the app was created.</span></span> <span data-ttu-id="95db7-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95db7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="95db7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95db7-158">DateTimeOffset</span></span>|<span data-ttu-id="95db7-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="95db7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="95db7-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="95db7-161">isFeatured</span></span>|<span data-ttu-id="95db7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="95db7-162">Boolean</span></span>|<span data-ttu-id="95db7-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="95db7-164">privacyInformationUrl</span></span>|<span data-ttu-id="95db7-165">String</span><span class="sxs-lookup"><span data-stu-id="95db7-165">String</span></span>|<span data-ttu-id="95db7-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="95db7-166">The privacy statement Url.</span></span> <span data-ttu-id="95db7-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="95db7-168">informationUrl</span></span>|<span data-ttu-id="95db7-169">String</span><span class="sxs-lookup"><span data-stu-id="95db7-169">String</span></span>|<span data-ttu-id="95db7-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="95db7-170">The more information Url.</span></span> <span data-ttu-id="95db7-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-172">owner</span><span class="sxs-lookup"><span data-stu-id="95db7-172">owner</span></span>|<span data-ttu-id="95db7-173">String</span><span class="sxs-lookup"><span data-stu-id="95db7-173">String</span></span>|<span data-ttu-id="95db7-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="95db7-174">The owner of the app.</span></span> <span data-ttu-id="95db7-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-176">developer</span><span class="sxs-lookup"><span data-stu-id="95db7-176">developer</span></span>|<span data-ttu-id="95db7-177">String</span><span class="sxs-lookup"><span data-stu-id="95db7-177">String</span></span>|<span data-ttu-id="95db7-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="95db7-178">The developer of the app.</span></span> <span data-ttu-id="95db7-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-180">notes</span><span class="sxs-lookup"><span data-stu-id="95db7-180">notes</span></span>|<span data-ttu-id="95db7-181">String</span><span class="sxs-lookup"><span data-stu-id="95db7-181">String</span></span>|<span data-ttu-id="95db7-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="95db7-182">Notes for the app.</span></span> <span data-ttu-id="95db7-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="95db7-184">uploadState</span></span>|<span data-ttu-id="95db7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="95db7-185">Int32</span></span>|<span data-ttu-id="95db7-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="95db7-186">The upload state.</span></span> <span data-ttu-id="95db7-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="95db7-188">publishingState</span></span>|[<span data-ttu-id="95db7-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="95db7-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="95db7-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="95db7-190">The publishing state for the app.</span></span> <span data-ttu-id="95db7-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="95db7-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="95db7-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="95db7-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="95db7-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="95db7-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="95db7-194">isAssigned</span></span>|<span data-ttu-id="95db7-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="95db7-195">Boolean</span></span>|<span data-ttu-id="95db7-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="95db7-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="95db7-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95db7-198">roleScopeTagIds</span></span>|<span data-ttu-id="95db7-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="95db7-199">String collection</span></span>|<span data-ttu-id="95db7-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="95db7-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="95db7-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="95db7-202">dependentAppCount</span></span>|<span data-ttu-id="95db7-203">Int32</span><span class="sxs-lookup"><span data-stu-id="95db7-203">Int32</span></span>|<span data-ttu-id="95db7-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="95db7-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="95db7-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95db7-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95db7-206">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="95db7-206">usedLicenseCount</span></span>|<span data-ttu-id="95db7-207">Int32</span><span class="sxs-lookup"><span data-stu-id="95db7-207">Int32</span></span>|<span data-ttu-id="95db7-208">Количество используемых лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="95db7-208">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="95db7-209">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="95db7-209">totalLicenseCount</span></span>|<span data-ttu-id="95db7-210">Int32</span><span class="sxs-lookup"><span data-stu-id="95db7-210">Int32</span></span>|<span data-ttu-id="95db7-211">Общее количество лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="95db7-211">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="95db7-212">productKey</span><span class="sxs-lookup"><span data-stu-id="95db7-212">productKey</span></span>|<span data-ttu-id="95db7-213">Строка</span><span class="sxs-lookup"><span data-stu-id="95db7-213">String</span></span>|<span data-ttu-id="95db7-214">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="95db7-214">The app product key</span></span>|
|<span data-ttu-id="95db7-215">licenseType</span><span class="sxs-lookup"><span data-stu-id="95db7-215">licenseType</span></span>|[<span data-ttu-id="95db7-216">микрософтсторефорбусинесслиценсетипе</span><span class="sxs-lookup"><span data-stu-id="95db7-216">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="95db7-217">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="95db7-217">The app license type.</span></span> <span data-ttu-id="95db7-218">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="95db7-218">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="95db7-219">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="95db7-219">packageIdentityName</span></span>|<span data-ttu-id="95db7-220">String</span><span class="sxs-lookup"><span data-stu-id="95db7-220">String</span></span>|<span data-ttu-id="95db7-221">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="95db7-221">The app package identifier</span></span>|
|<span data-ttu-id="95db7-222">licensingType</span><span class="sxs-lookup"><span data-stu-id="95db7-222">licensingType</span></span>|[<span data-ttu-id="95db7-223">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="95db7-223">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="95db7-224">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="95db7-224">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="95db7-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="95db7-225">Response</span></span>
<span data-ttu-id="95db7-226">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="95db7-226">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95db7-227">Пример</span><span class="sxs-lookup"><span data-stu-id="95db7-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="95db7-228">Запрос</span><span class="sxs-lookup"><span data-stu-id="95db7-228">Request</span></span>
<span data-ttu-id="95db7-229">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95db7-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1132

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```

### <a name="response"></a><span data-ttu-id="95db7-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="95db7-230">Response</span></span>
<span data-ttu-id="95db7-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95db7-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1304

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```





