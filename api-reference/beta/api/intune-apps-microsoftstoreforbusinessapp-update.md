---
title: Update microsoftStoreForBusinessApp
description: Обновление свойств объекта microsoftStoreForBusinessApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 114f2acc847fb0812a123afe840a3ccd315a16e5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935463"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="f00f3-103">Update microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="f00f3-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="f00f3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f00f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f00f3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f00f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f00f3-106">Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-106">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f00f3-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f00f3-107">Prerequisites</span></span>
<span data-ttu-id="f00f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f00f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f00f3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f00f3-110">Permission type</span></span>|<span data-ttu-id="f00f3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f00f3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f00f3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f00f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f00f3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f00f3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f00f3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f00f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f00f3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f00f3-115">Not supported.</span></span>|
|<span data-ttu-id="f00f3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f00f3-116">Application</span></span>|<span data-ttu-id="f00f3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f00f3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f00f3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f00f3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f00f3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f00f3-119">Request headers</span></span>
|<span data-ttu-id="f00f3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f00f3-120">Header</span></span>|<span data-ttu-id="f00f3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f00f3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f00f3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f00f3-122">Authorization</span></span>|<span data-ttu-id="f00f3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f00f3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f00f3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f00f3-124">Accept</span></span>|<span data-ttu-id="f00f3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f00f3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f00f3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f00f3-126">Request body</span></span>
<span data-ttu-id="f00f3-127">В теле запроса добавьте представление объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f00f3-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="f00f3-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="f00f3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f00f3-129">Property</span></span>|<span data-ttu-id="f00f3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f00f3-130">Type</span></span>|<span data-ttu-id="f00f3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f00f3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f00f3-132">id</span><span class="sxs-lookup"><span data-stu-id="f00f3-132">id</span></span>|<span data-ttu-id="f00f3-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f00f3-133">String</span></span>|<span data-ttu-id="f00f3-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f00f3-134">Key of the entity.</span></span> <span data-ttu-id="f00f3-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f00f3-136">displayName</span></span>|<span data-ttu-id="f00f3-137">Строка</span><span class="sxs-lookup"><span data-stu-id="f00f3-137">String</span></span>|<span data-ttu-id="f00f3-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="f00f3-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f00f3-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-140">description</span><span class="sxs-lookup"><span data-stu-id="f00f3-140">description</span></span>|<span data-ttu-id="f00f3-141">Строка</span><span class="sxs-lookup"><span data-stu-id="f00f3-141">String</span></span>|<span data-ttu-id="f00f3-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f00f3-142">The description of the app.</span></span> <span data-ttu-id="f00f3-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f00f3-144">publisher</span></span>|<span data-ttu-id="f00f3-145">Строка</span><span class="sxs-lookup"><span data-stu-id="f00f3-145">String</span></span>|<span data-ttu-id="f00f3-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f00f3-146">The publisher of the app.</span></span> <span data-ttu-id="f00f3-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f00f3-148">largeIcon</span></span>|[<span data-ttu-id="f00f3-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f00f3-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f00f3-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f00f3-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f00f3-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f00f3-152">createdDateTime</span></span>|<span data-ttu-id="f00f3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f00f3-153">DateTimeOffset</span></span>|<span data-ttu-id="f00f3-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f00f3-154">The date and time the app was created.</span></span> <span data-ttu-id="f00f3-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f00f3-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f00f3-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f00f3-157">DateTimeOffset</span></span>|<span data-ttu-id="f00f3-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f00f3-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f00f3-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f00f3-160">isFeatured</span></span>|<span data-ttu-id="f00f3-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f00f3-161">Boolean</span></span>|<span data-ttu-id="f00f3-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f00f3-163">privacyInformationUrl</span></span>|<span data-ttu-id="f00f3-164">Строка</span><span class="sxs-lookup"><span data-stu-id="f00f3-164">String</span></span>|<span data-ttu-id="f00f3-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f00f3-165">The privacy statement Url.</span></span> <span data-ttu-id="f00f3-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f00f3-167">informationUrl</span></span>|<span data-ttu-id="f00f3-168">Строка</span><span class="sxs-lookup"><span data-stu-id="f00f3-168">String</span></span>|<span data-ttu-id="f00f3-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f00f3-169">The more information Url.</span></span> <span data-ttu-id="f00f3-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-171">owner</span><span class="sxs-lookup"><span data-stu-id="f00f3-171">owner</span></span>|<span data-ttu-id="f00f3-172">String</span><span class="sxs-lookup"><span data-stu-id="f00f3-172">String</span></span>|<span data-ttu-id="f00f3-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f00f3-173">The owner of the app.</span></span> <span data-ttu-id="f00f3-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-175">developer</span><span class="sxs-lookup"><span data-stu-id="f00f3-175">developer</span></span>|<span data-ttu-id="f00f3-176">Строка</span><span class="sxs-lookup"><span data-stu-id="f00f3-176">String</span></span>|<span data-ttu-id="f00f3-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f00f3-177">The developer of the app.</span></span> <span data-ttu-id="f00f3-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-179">notes</span><span class="sxs-lookup"><span data-stu-id="f00f3-179">notes</span></span>|<span data-ttu-id="f00f3-180">Строка</span><span class="sxs-lookup"><span data-stu-id="f00f3-180">String</span></span>|<span data-ttu-id="f00f3-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="f00f3-181">Notes for the app.</span></span> <span data-ttu-id="f00f3-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f00f3-183">uploadState</span></span>|<span data-ttu-id="f00f3-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f00f3-184">Int32</span></span>|<span data-ttu-id="f00f3-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="f00f3-185">The upload state.</span></span> <span data-ttu-id="f00f3-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f00f3-187">publishingState</span></span>|[<span data-ttu-id="f00f3-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="f00f3-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f00f3-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="f00f3-189">The publishing state for the app.</span></span> <span data-ttu-id="f00f3-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f00f3-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f00f3-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f00f3-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f00f3-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f00f3-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f00f3-193">isAssigned</span></span>|<span data-ttu-id="f00f3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f00f3-194">Boolean</span></span>|<span data-ttu-id="f00f3-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="f00f3-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f00f3-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f00f3-197">roleScopeTagIds</span></span>|<span data-ttu-id="f00f3-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f00f3-198">String collection</span></span>|<span data-ttu-id="f00f3-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f00f3-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f00f3-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="f00f3-201">dependentAppCount</span></span>|<span data-ttu-id="f00f3-202">Int32</span><span class="sxs-lookup"><span data-stu-id="f00f3-202">Int32</span></span>|<span data-ttu-id="f00f3-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="f00f3-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f00f3-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f00f3-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f00f3-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f00f3-205">usedLicenseCount</span></span>|<span data-ttu-id="f00f3-206">Int32</span><span class="sxs-lookup"><span data-stu-id="f00f3-206">Int32</span></span>|<span data-ttu-id="f00f3-207">Количество используемых лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f00f3-207">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="f00f3-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f00f3-208">totalLicenseCount</span></span>|<span data-ttu-id="f00f3-209">Int32</span><span class="sxs-lookup"><span data-stu-id="f00f3-209">Int32</span></span>|<span data-ttu-id="f00f3-210">Общее количество лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f00f3-210">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="f00f3-211">productKey</span><span class="sxs-lookup"><span data-stu-id="f00f3-211">productKey</span></span>|<span data-ttu-id="f00f3-212">Строка</span><span class="sxs-lookup"><span data-stu-id="f00f3-212">String</span></span>|<span data-ttu-id="f00f3-213">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="f00f3-213">The app product key</span></span>|
|<span data-ttu-id="f00f3-214">licenseType</span><span class="sxs-lookup"><span data-stu-id="f00f3-214">licenseType</span></span>|[<span data-ttu-id="f00f3-215">Микрософтсторефорбусинесслиценсетипе</span><span class="sxs-lookup"><span data-stu-id="f00f3-215">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="f00f3-216">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="f00f3-216">The app license type.</span></span> <span data-ttu-id="f00f3-217">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="f00f3-217">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="f00f3-218">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="f00f3-218">packageIdentityName</span></span>|<span data-ttu-id="f00f3-219">String</span><span class="sxs-lookup"><span data-stu-id="f00f3-219">String</span></span>|<span data-ttu-id="f00f3-220">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="f00f3-220">The app package identifier</span></span>|
|<span data-ttu-id="f00f3-221">licensingType</span><span class="sxs-lookup"><span data-stu-id="f00f3-221">licensingType</span></span>|[<span data-ttu-id="f00f3-222">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="f00f3-222">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="f00f3-223">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="f00f3-223">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="f00f3-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="f00f3-224">Response</span></span>
<span data-ttu-id="f00f3-225">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f00f3-225">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f00f3-226">Пример</span><span class="sxs-lookup"><span data-stu-id="f00f3-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="f00f3-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="f00f3-227">Request</span></span>
<span data-ttu-id="f00f3-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f00f3-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f00f3-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="f00f3-229">Response</span></span>
<span data-ttu-id="f00f3-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f00f3-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




