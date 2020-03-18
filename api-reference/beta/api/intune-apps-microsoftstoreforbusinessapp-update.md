---
title: Update microsoftStoreForBusinessApp
description: Обновление свойств объекта microsoftStoreForBusinessApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d261429bf13e8b48076d6688ec2f073f57832304
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761470"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="30b97-103">Update microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="30b97-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="30b97-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30b97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30b97-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30b97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30b97-106">Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-106">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30b97-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="30b97-107">Prerequisites</span></span>
<span data-ttu-id="30b97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30b97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30b97-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30b97-110">Permission type</span></span>|<span data-ttu-id="30b97-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30b97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30b97-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30b97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30b97-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b97-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30b97-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30b97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30b97-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30b97-115">Not supported.</span></span>|
|<span data-ttu-id="30b97-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="30b97-116">Application</span></span>|<span data-ttu-id="30b97-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b97-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30b97-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30b97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="30b97-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="30b97-119">Request headers</span></span>
|<span data-ttu-id="30b97-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30b97-120">Header</span></span>|<span data-ttu-id="30b97-121">Значение</span><span class="sxs-lookup"><span data-stu-id="30b97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30b97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="30b97-122">Authorization</span></span>|<span data-ttu-id="30b97-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30b97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30b97-124">Accept</span><span class="sxs-lookup"><span data-stu-id="30b97-124">Accept</span></span>|<span data-ttu-id="30b97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30b97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30b97-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30b97-126">Request body</span></span>
<span data-ttu-id="30b97-127">В теле запроса добавьте представление объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30b97-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="30b97-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="30b97-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="30b97-129">Property</span></span>|<span data-ttu-id="30b97-130">Тип</span><span class="sxs-lookup"><span data-stu-id="30b97-130">Type</span></span>|<span data-ttu-id="30b97-131">Описание</span><span class="sxs-lookup"><span data-stu-id="30b97-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30b97-132">id</span><span class="sxs-lookup"><span data-stu-id="30b97-132">id</span></span>|<span data-ttu-id="30b97-133">Строка</span><span class="sxs-lookup"><span data-stu-id="30b97-133">String</span></span>|<span data-ttu-id="30b97-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="30b97-134">Key of the entity.</span></span> <span data-ttu-id="30b97-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-136">displayName</span><span class="sxs-lookup"><span data-stu-id="30b97-136">displayName</span></span>|<span data-ttu-id="30b97-137">Строка</span><span class="sxs-lookup"><span data-stu-id="30b97-137">String</span></span>|<span data-ttu-id="30b97-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="30b97-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="30b97-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-140">description</span><span class="sxs-lookup"><span data-stu-id="30b97-140">description</span></span>|<span data-ttu-id="30b97-141">String</span><span class="sxs-lookup"><span data-stu-id="30b97-141">String</span></span>|<span data-ttu-id="30b97-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="30b97-142">The description of the app.</span></span> <span data-ttu-id="30b97-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-144">publisher</span><span class="sxs-lookup"><span data-stu-id="30b97-144">publisher</span></span>|<span data-ttu-id="30b97-145">String</span><span class="sxs-lookup"><span data-stu-id="30b97-145">String</span></span>|<span data-ttu-id="30b97-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="30b97-146">The publisher of the app.</span></span> <span data-ttu-id="30b97-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="30b97-148">largeIcon</span></span>|[<span data-ttu-id="30b97-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="30b97-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="30b97-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="30b97-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="30b97-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30b97-152">createdDateTime</span></span>|<span data-ttu-id="30b97-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30b97-153">DateTimeOffset</span></span>|<span data-ttu-id="30b97-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="30b97-154">The date and time the app was created.</span></span> <span data-ttu-id="30b97-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30b97-156">lastModifiedDateTime</span></span>|<span data-ttu-id="30b97-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30b97-157">DateTimeOffset</span></span>|<span data-ttu-id="30b97-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="30b97-158">The date and time the app was last modified.</span></span> <span data-ttu-id="30b97-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="30b97-160">isFeatured</span></span>|<span data-ttu-id="30b97-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="30b97-161">Boolean</span></span>|<span data-ttu-id="30b97-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="30b97-163">privacyInformationUrl</span></span>|<span data-ttu-id="30b97-164">String</span><span class="sxs-lookup"><span data-stu-id="30b97-164">String</span></span>|<span data-ttu-id="30b97-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="30b97-165">The privacy statement Url.</span></span> <span data-ttu-id="30b97-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="30b97-167">informationUrl</span></span>|<span data-ttu-id="30b97-168">String</span><span class="sxs-lookup"><span data-stu-id="30b97-168">String</span></span>|<span data-ttu-id="30b97-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="30b97-169">The more information Url.</span></span> <span data-ttu-id="30b97-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-171">owner</span><span class="sxs-lookup"><span data-stu-id="30b97-171">owner</span></span>|<span data-ttu-id="30b97-172">String</span><span class="sxs-lookup"><span data-stu-id="30b97-172">String</span></span>|<span data-ttu-id="30b97-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="30b97-173">The owner of the app.</span></span> <span data-ttu-id="30b97-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-175">developer</span><span class="sxs-lookup"><span data-stu-id="30b97-175">developer</span></span>|<span data-ttu-id="30b97-176">String</span><span class="sxs-lookup"><span data-stu-id="30b97-176">String</span></span>|<span data-ttu-id="30b97-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="30b97-177">The developer of the app.</span></span> <span data-ttu-id="30b97-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-179">notes</span><span class="sxs-lookup"><span data-stu-id="30b97-179">notes</span></span>|<span data-ttu-id="30b97-180">String</span><span class="sxs-lookup"><span data-stu-id="30b97-180">String</span></span>|<span data-ttu-id="30b97-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="30b97-181">Notes for the app.</span></span> <span data-ttu-id="30b97-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="30b97-183">uploadState</span></span>|<span data-ttu-id="30b97-184">Int32</span><span class="sxs-lookup"><span data-stu-id="30b97-184">Int32</span></span>|<span data-ttu-id="30b97-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="30b97-185">The upload state.</span></span> <span data-ttu-id="30b97-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="30b97-187">publishingState</span></span>|[<span data-ttu-id="30b97-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="30b97-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="30b97-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="30b97-189">The publishing state for the app.</span></span> <span data-ttu-id="30b97-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="30b97-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="30b97-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="30b97-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="30b97-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="30b97-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="30b97-193">isAssigned</span></span>|<span data-ttu-id="30b97-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="30b97-194">Boolean</span></span>|<span data-ttu-id="30b97-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="30b97-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="30b97-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="30b97-197">roleScopeTagIds</span></span>|<span data-ttu-id="30b97-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="30b97-198">String collection</span></span>|<span data-ttu-id="30b97-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="30b97-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="30b97-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="30b97-201">dependentAppCount</span></span>|<span data-ttu-id="30b97-202">Int32</span><span class="sxs-lookup"><span data-stu-id="30b97-202">Int32</span></span>|<span data-ttu-id="30b97-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="30b97-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="30b97-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30b97-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30b97-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="30b97-205">usedLicenseCount</span></span>|<span data-ttu-id="30b97-206">Int32</span><span class="sxs-lookup"><span data-stu-id="30b97-206">Int32</span></span>|<span data-ttu-id="30b97-207">Количество используемых лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="30b97-207">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="30b97-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="30b97-208">totalLicenseCount</span></span>|<span data-ttu-id="30b97-209">Int32</span><span class="sxs-lookup"><span data-stu-id="30b97-209">Int32</span></span>|<span data-ttu-id="30b97-210">Общее количество лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="30b97-210">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="30b97-211">productKey</span><span class="sxs-lookup"><span data-stu-id="30b97-211">productKey</span></span>|<span data-ttu-id="30b97-212">Строка</span><span class="sxs-lookup"><span data-stu-id="30b97-212">String</span></span>|<span data-ttu-id="30b97-213">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="30b97-213">The app product key</span></span>|
|<span data-ttu-id="30b97-214">licenseType</span><span class="sxs-lookup"><span data-stu-id="30b97-214">licenseType</span></span>|[<span data-ttu-id="30b97-215">микрософтсторефорбусинесслиценсетипе</span><span class="sxs-lookup"><span data-stu-id="30b97-215">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="30b97-216">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="30b97-216">The app license type.</span></span> <span data-ttu-id="30b97-217">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="30b97-217">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="30b97-218">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="30b97-218">packageIdentityName</span></span>|<span data-ttu-id="30b97-219">String</span><span class="sxs-lookup"><span data-stu-id="30b97-219">String</span></span>|<span data-ttu-id="30b97-220">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="30b97-220">The app package identifier</span></span>|
|<span data-ttu-id="30b97-221">licensingType</span><span class="sxs-lookup"><span data-stu-id="30b97-221">licensingType</span></span>|[<span data-ttu-id="30b97-222">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="30b97-222">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="30b97-223">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="30b97-223">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="30b97-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="30b97-224">Response</span></span>
<span data-ttu-id="30b97-225">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="30b97-225">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30b97-226">Пример</span><span class="sxs-lookup"><span data-stu-id="30b97-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="30b97-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="30b97-227">Request</span></span>
<span data-ttu-id="30b97-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30b97-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30b97-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="30b97-229">Response</span></span>
<span data-ttu-id="30b97-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30b97-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




