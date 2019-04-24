---
title: Update microsoftStoreForBusinessApp
description: Обновление свойств объекта microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44e6d282610f2cd836689a6d68d77e33714ae20b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32490985"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="be7c9-103">Update microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="be7c9-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="be7c9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be7c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be7c9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be7c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be7c9-106">Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-106">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be7c9-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="be7c9-107">Prerequisites</span></span>
<span data-ttu-id="be7c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be7c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be7c9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be7c9-110">Permission type</span></span>|<span data-ttu-id="be7c9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be7c9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be7c9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be7c9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be7c9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be7c9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="be7c9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be7c9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be7c9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be7c9-115">Not supported.</span></span>|
|<span data-ttu-id="be7c9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be7c9-116">Application</span></span>|<span data-ttu-id="be7c9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be7c9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be7c9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be7c9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="be7c9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be7c9-119">Request headers</span></span>
|<span data-ttu-id="be7c9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be7c9-120">Header</span></span>|<span data-ttu-id="be7c9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="be7c9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be7c9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be7c9-122">Authorization</span></span>|<span data-ttu-id="be7c9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be7c9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be7c9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="be7c9-124">Accept</span></span>|<span data-ttu-id="be7c9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be7c9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be7c9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be7c9-126">Request body</span></span>
<span data-ttu-id="be7c9-127">В теле запроса добавьте представление объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be7c9-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="be7c9-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="be7c9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="be7c9-129">Property</span></span>|<span data-ttu-id="be7c9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="be7c9-130">Type</span></span>|<span data-ttu-id="be7c9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="be7c9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be7c9-132">id</span><span class="sxs-lookup"><span data-stu-id="be7c9-132">id</span></span>|<span data-ttu-id="be7c9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="be7c9-133">String</span></span>|<span data-ttu-id="be7c9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="be7c9-134">Key of the entity.</span></span> <span data-ttu-id="be7c9-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="be7c9-136">displayName</span></span>|<span data-ttu-id="be7c9-137">String</span><span class="sxs-lookup"><span data-stu-id="be7c9-137">String</span></span>|<span data-ttu-id="be7c9-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="be7c9-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="be7c9-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-140">description</span><span class="sxs-lookup"><span data-stu-id="be7c9-140">description</span></span>|<span data-ttu-id="be7c9-141">String</span><span class="sxs-lookup"><span data-stu-id="be7c9-141">String</span></span>|<span data-ttu-id="be7c9-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="be7c9-142">The description of the app.</span></span> <span data-ttu-id="be7c9-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-144">publisher</span><span class="sxs-lookup"><span data-stu-id="be7c9-144">publisher</span></span>|<span data-ttu-id="be7c9-145">String</span><span class="sxs-lookup"><span data-stu-id="be7c9-145">String</span></span>|<span data-ttu-id="be7c9-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="be7c9-146">The publisher of the app.</span></span> <span data-ttu-id="be7c9-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="be7c9-148">largeIcon</span></span>|[<span data-ttu-id="be7c9-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="be7c9-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="be7c9-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="be7c9-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="be7c9-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be7c9-152">createdDateTime</span></span>|<span data-ttu-id="be7c9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be7c9-153">DateTimeOffset</span></span>|<span data-ttu-id="be7c9-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="be7c9-154">The date and time the app was created.</span></span> <span data-ttu-id="be7c9-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be7c9-156">lastModifiedDateTime</span></span>|<span data-ttu-id="be7c9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be7c9-157">DateTimeOffset</span></span>|<span data-ttu-id="be7c9-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="be7c9-158">The date and time the app was last modified.</span></span> <span data-ttu-id="be7c9-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="be7c9-160">isFeatured</span></span>|<span data-ttu-id="be7c9-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="be7c9-161">Boolean</span></span>|<span data-ttu-id="be7c9-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="be7c9-163">privacyInformationUrl</span></span>|<span data-ttu-id="be7c9-164">String</span><span class="sxs-lookup"><span data-stu-id="be7c9-164">String</span></span>|<span data-ttu-id="be7c9-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="be7c9-165">The privacy statement Url.</span></span> <span data-ttu-id="be7c9-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="be7c9-167">informationUrl</span></span>|<span data-ttu-id="be7c9-168">String</span><span class="sxs-lookup"><span data-stu-id="be7c9-168">String</span></span>|<span data-ttu-id="be7c9-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="be7c9-169">The more information Url.</span></span> <span data-ttu-id="be7c9-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-171">owner</span><span class="sxs-lookup"><span data-stu-id="be7c9-171">owner</span></span>|<span data-ttu-id="be7c9-172">String</span><span class="sxs-lookup"><span data-stu-id="be7c9-172">String</span></span>|<span data-ttu-id="be7c9-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="be7c9-173">The owner of the app.</span></span> <span data-ttu-id="be7c9-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-175">developer</span><span class="sxs-lookup"><span data-stu-id="be7c9-175">developer</span></span>|<span data-ttu-id="be7c9-176">String</span><span class="sxs-lookup"><span data-stu-id="be7c9-176">String</span></span>|<span data-ttu-id="be7c9-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="be7c9-177">The developer of the app.</span></span> <span data-ttu-id="be7c9-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-179">notes</span><span class="sxs-lookup"><span data-stu-id="be7c9-179">notes</span></span>|<span data-ttu-id="be7c9-180">String</span><span class="sxs-lookup"><span data-stu-id="be7c9-180">String</span></span>|<span data-ttu-id="be7c9-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="be7c9-181">Notes for the app.</span></span> <span data-ttu-id="be7c9-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="be7c9-183">uploadState</span></span>|<span data-ttu-id="be7c9-184">Int32</span><span class="sxs-lookup"><span data-stu-id="be7c9-184">Int32</span></span>|<span data-ttu-id="be7c9-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="be7c9-185">The upload state.</span></span> <span data-ttu-id="be7c9-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="be7c9-187">publishingState</span></span>|[<span data-ttu-id="be7c9-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="be7c9-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="be7c9-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="be7c9-189">The publishing state for the app.</span></span> <span data-ttu-id="be7c9-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="be7c9-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="be7c9-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="be7c9-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="be7c9-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="be7c9-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="be7c9-193">isAssigned</span></span>|<span data-ttu-id="be7c9-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="be7c9-194">Boolean</span></span>|<span data-ttu-id="be7c9-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="be7c9-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="be7c9-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="be7c9-197">roleScopeTagIds</span></span>|<span data-ttu-id="be7c9-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="be7c9-198">String collection</span></span>|<span data-ttu-id="be7c9-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="be7c9-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="be7c9-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="be7c9-201">dependentAppCount</span></span>|<span data-ttu-id="be7c9-202">Int32</span><span class="sxs-lookup"><span data-stu-id="be7c9-202">Int32</span></span>|<span data-ttu-id="be7c9-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="be7c9-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="be7c9-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="be7c9-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be7c9-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="be7c9-205">usedLicenseCount</span></span>|<span data-ttu-id="be7c9-206">Int32</span><span class="sxs-lookup"><span data-stu-id="be7c9-206">Int32</span></span>|<span data-ttu-id="be7c9-207">Количество используемых лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="be7c9-207">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="be7c9-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="be7c9-208">totalLicenseCount</span></span>|<span data-ttu-id="be7c9-209">Int32</span><span class="sxs-lookup"><span data-stu-id="be7c9-209">Int32</span></span>|<span data-ttu-id="be7c9-210">Общее количество лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="be7c9-210">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="be7c9-211">productKey</span><span class="sxs-lookup"><span data-stu-id="be7c9-211">productKey</span></span>|<span data-ttu-id="be7c9-212">Строка</span><span class="sxs-lookup"><span data-stu-id="be7c9-212">String</span></span>|<span data-ttu-id="be7c9-213">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="be7c9-213">The app product key</span></span>|
|<span data-ttu-id="be7c9-214">licenseType</span><span class="sxs-lookup"><span data-stu-id="be7c9-214">licenseType</span></span>|[<span data-ttu-id="be7c9-215">Микрософтсторефорбусинесслиценсетипе</span><span class="sxs-lookup"><span data-stu-id="be7c9-215">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="be7c9-216">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="be7c9-216">The app license type.</span></span> <span data-ttu-id="be7c9-217">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="be7c9-217">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="be7c9-218">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="be7c9-218">packageIdentityName</span></span>|<span data-ttu-id="be7c9-219">String</span><span class="sxs-lookup"><span data-stu-id="be7c9-219">String</span></span>|<span data-ttu-id="be7c9-220">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="be7c9-220">The app package identifier</span></span>|
|<span data-ttu-id="be7c9-221">licensingType</span><span class="sxs-lookup"><span data-stu-id="be7c9-221">licensingType</span></span>|[<span data-ttu-id="be7c9-222">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="be7c9-222">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="be7c9-223">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="be7c9-223">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="be7c9-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="be7c9-224">Response</span></span>
<span data-ttu-id="be7c9-225">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="be7c9-225">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be7c9-226">Пример</span><span class="sxs-lookup"><span data-stu-id="be7c9-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="be7c9-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="be7c9-227">Request</span></span>
<span data-ttu-id="be7c9-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be7c9-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be7c9-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="be7c9-229">Response</span></span>
<span data-ttu-id="be7c9-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be7c9-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





