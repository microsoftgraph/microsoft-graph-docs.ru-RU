---
title: Update microsoftStoreForBusinessApp
description: Обновление свойств объекта microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e23afba48af0ad72c90d288684cc7cecadb8c65
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140945"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="1b21a-103">Update microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="1b21a-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="1b21a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b21a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b21a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b21a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b21a-106">Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-106">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b21a-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1b21a-107">Prerequisites</span></span>
<span data-ttu-id="1b21a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1b21a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b21a-110">Permission type</span></span>|<span data-ttu-id="1b21a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b21a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b21a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b21a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b21a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b21a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b21a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b21a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b21a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b21a-115">Not supported.</span></span>|
|<span data-ttu-id="1b21a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b21a-116">Application</span></span>|<span data-ttu-id="1b21a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b21a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b21a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b21a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="1b21a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b21a-119">Request headers</span></span>
|<span data-ttu-id="1b21a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b21a-120">Header</span></span>|<span data-ttu-id="1b21a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1b21a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b21a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b21a-122">Authorization</span></span>|<span data-ttu-id="1b21a-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1b21a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b21a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1b21a-124">Accept</span></span>|<span data-ttu-id="1b21a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b21a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b21a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b21a-126">Request body</span></span>
<span data-ttu-id="1b21a-127">В теле запроса добавьте представление объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b21a-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="1b21a-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="1b21a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b21a-129">Property</span></span>|<span data-ttu-id="1b21a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1b21a-130">Type</span></span>|<span data-ttu-id="1b21a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1b21a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b21a-132">id</span><span class="sxs-lookup"><span data-stu-id="1b21a-132">id</span></span>|<span data-ttu-id="1b21a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1b21a-133">String</span></span>|<span data-ttu-id="1b21a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1b21a-134">Key of the entity.</span></span> <span data-ttu-id="1b21a-135">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1b21a-136">displayName</span></span>|<span data-ttu-id="1b21a-137">String</span><span class="sxs-lookup"><span data-stu-id="1b21a-137">String</span></span>|<span data-ttu-id="1b21a-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="1b21a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1b21a-139">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-140">description</span><span class="sxs-lookup"><span data-stu-id="1b21a-140">description</span></span>|<span data-ttu-id="1b21a-141">Строка</span><span class="sxs-lookup"><span data-stu-id="1b21a-141">String</span></span>|<span data-ttu-id="1b21a-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="1b21a-142">The description of the app.</span></span> <span data-ttu-id="1b21a-143">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-144">publisher</span><span class="sxs-lookup"><span data-stu-id="1b21a-144">publisher</span></span>|<span data-ttu-id="1b21a-145">String</span><span class="sxs-lookup"><span data-stu-id="1b21a-145">String</span></span>|<span data-ttu-id="1b21a-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="1b21a-146">The publisher of the app.</span></span> <span data-ttu-id="1b21a-147">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1b21a-148">largeIcon</span></span>|[<span data-ttu-id="1b21a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1b21a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1b21a-150">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="1b21a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1b21a-151">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b21a-152">createdDateTime</span></span>|<span data-ttu-id="1b21a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b21a-153">DateTimeOffset</span></span>|<span data-ttu-id="1b21a-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="1b21a-154">The date and time the app was created.</span></span> <span data-ttu-id="1b21a-155">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b21a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="1b21a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b21a-157">DateTimeOffset</span></span>|<span data-ttu-id="1b21a-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="1b21a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="1b21a-159">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1b21a-160">isFeatured</span></span>|<span data-ttu-id="1b21a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b21a-161">Boolean</span></span>|<span data-ttu-id="1b21a-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1b21a-163">privacyInformationUrl</span></span>|<span data-ttu-id="1b21a-164">String</span><span class="sxs-lookup"><span data-stu-id="1b21a-164">String</span></span>|<span data-ttu-id="1b21a-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="1b21a-165">The privacy statement Url.</span></span> <span data-ttu-id="1b21a-166">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1b21a-167">informationUrl</span></span>|<span data-ttu-id="1b21a-168">String</span><span class="sxs-lookup"><span data-stu-id="1b21a-168">String</span></span>|<span data-ttu-id="1b21a-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="1b21a-169">The more information Url.</span></span> <span data-ttu-id="1b21a-170">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-171">owner</span><span class="sxs-lookup"><span data-stu-id="1b21a-171">owner</span></span>|<span data-ttu-id="1b21a-172">String</span><span class="sxs-lookup"><span data-stu-id="1b21a-172">String</span></span>|<span data-ttu-id="1b21a-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="1b21a-173">The owner of the app.</span></span> <span data-ttu-id="1b21a-174">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-175">developer</span><span class="sxs-lookup"><span data-stu-id="1b21a-175">developer</span></span>|<span data-ttu-id="1b21a-176">String</span><span class="sxs-lookup"><span data-stu-id="1b21a-176">String</span></span>|<span data-ttu-id="1b21a-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="1b21a-177">The developer of the app.</span></span> <span data-ttu-id="1b21a-178">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-179">notes</span><span class="sxs-lookup"><span data-stu-id="1b21a-179">notes</span></span>|<span data-ttu-id="1b21a-180">String</span><span class="sxs-lookup"><span data-stu-id="1b21a-180">String</span></span>|<span data-ttu-id="1b21a-181">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="1b21a-181">Notes for the app.</span></span> <span data-ttu-id="1b21a-182">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="1b21a-183">uploadState</span></span>|<span data-ttu-id="1b21a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1b21a-184">Int32</span></span>|<span data-ttu-id="1b21a-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="1b21a-185">The upload state.</span></span> <span data-ttu-id="1b21a-186">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="1b21a-187">publishingState</span></span>|[<span data-ttu-id="1b21a-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="1b21a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1b21a-189">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="1b21a-189">The publishing state for the app.</span></span> <span data-ttu-id="1b21a-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="1b21a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1b21a-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1b21a-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1b21a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1b21a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1b21a-193">isAssigned</span></span>|<span data-ttu-id="1b21a-194">Логический</span><span class="sxs-lookup"><span data-stu-id="1b21a-194">Boolean</span></span>|<span data-ttu-id="1b21a-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="1b21a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1b21a-196">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1b21a-197">roleScopeTagIds</span></span>|<span data-ttu-id="1b21a-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1b21a-198">String collection</span></span>|<span data-ttu-id="1b21a-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="1b21a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1b21a-200">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b21a-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b21a-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1b21a-201">usedLicenseCount</span></span>|<span data-ttu-id="1b21a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="1b21a-202">Int32</span></span>|<span data-ttu-id="1b21a-203">Количество используемых лицензий Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1b21a-203">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="1b21a-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1b21a-204">totalLicenseCount</span></span>|<span data-ttu-id="1b21a-205">Int32</span><span class="sxs-lookup"><span data-stu-id="1b21a-205">Int32</span></span>|<span data-ttu-id="1b21a-206">Общее количество лицензий Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1b21a-206">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="1b21a-207">productKey</span><span class="sxs-lookup"><span data-stu-id="1b21a-207">productKey</span></span>|<span data-ttu-id="1b21a-208">Строка</span><span class="sxs-lookup"><span data-stu-id="1b21a-208">String</span></span>|<span data-ttu-id="1b21a-209">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="1b21a-209">The app product key</span></span>|
|<span data-ttu-id="1b21a-210">licenseType</span><span class="sxs-lookup"><span data-stu-id="1b21a-210">licenseType</span></span>|[<span data-ttu-id="1b21a-211">Микрософтсторефорбусинесслиценсетипе</span><span class="sxs-lookup"><span data-stu-id="1b21a-211">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="1b21a-212">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="1b21a-212">The app license type.</span></span> <span data-ttu-id="1b21a-213">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="1b21a-213">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="1b21a-214">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="1b21a-214">packageIdentityName</span></span>|<span data-ttu-id="1b21a-215">String</span><span class="sxs-lookup"><span data-stu-id="1b21a-215">String</span></span>|<span data-ttu-id="1b21a-216">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="1b21a-216">The app package identifier</span></span>|
|<span data-ttu-id="1b21a-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="1b21a-217">licensingType</span></span>|[<span data-ttu-id="1b21a-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="1b21a-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="1b21a-219">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="1b21a-219">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="1b21a-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b21a-220">Response</span></span>
<span data-ttu-id="1b21a-221">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1b21a-221">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b21a-222">Пример</span><span class="sxs-lookup"><span data-stu-id="1b21a-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b21a-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b21a-223">Request</span></span>
<span data-ttu-id="1b21a-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b21a-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1105

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

### <a name="response"></a><span data-ttu-id="1b21a-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b21a-225">Response</span></span>
<span data-ttu-id="1b21a-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1b21a-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1277

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




