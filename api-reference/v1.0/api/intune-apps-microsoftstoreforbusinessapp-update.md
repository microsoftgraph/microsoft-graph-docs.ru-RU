---
title: Update microsoftStoreForBusinessApp
description: Обновление свойств объекта microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 053721e2bc58258e4f6d4d28478ce1bbd736e520
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002113"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="57afc-103">Update microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="57afc-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="57afc-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57afc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57afc-105">Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-105">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57afc-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="57afc-106">Prerequisites</span></span>
<span data-ttu-id="57afc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57afc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57afc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57afc-109">Permission type</span></span>|<span data-ttu-id="57afc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57afc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57afc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57afc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="57afc-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57afc-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="57afc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57afc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57afc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57afc-114">Not supported.</span></span>|
|<span data-ttu-id="57afc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57afc-115">Application</span></span>|<span data-ttu-id="57afc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57afc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57afc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57afc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="57afc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57afc-118">Request headers</span></span>
|<span data-ttu-id="57afc-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57afc-119">Header</span></span>|<span data-ttu-id="57afc-120">Значение</span><span class="sxs-lookup"><span data-stu-id="57afc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57afc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57afc-121">Authorization</span></span>|<span data-ttu-id="57afc-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57afc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57afc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="57afc-123">Accept</span></span>|<span data-ttu-id="57afc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="57afc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57afc-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="57afc-125">Request body</span></span>
<span data-ttu-id="57afc-126">В теле запроса добавьте представление объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57afc-126">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="57afc-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-127">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="57afc-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="57afc-128">Property</span></span>|<span data-ttu-id="57afc-129">Тип</span><span class="sxs-lookup"><span data-stu-id="57afc-129">Type</span></span>|<span data-ttu-id="57afc-130">Описание</span><span class="sxs-lookup"><span data-stu-id="57afc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57afc-131">id</span><span class="sxs-lookup"><span data-stu-id="57afc-131">id</span></span>|<span data-ttu-id="57afc-132">Строка</span><span class="sxs-lookup"><span data-stu-id="57afc-132">String</span></span>|<span data-ttu-id="57afc-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="57afc-133">Key of the entity.</span></span> <span data-ttu-id="57afc-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="57afc-135">displayName</span></span>|<span data-ttu-id="57afc-136">Строка</span><span class="sxs-lookup"><span data-stu-id="57afc-136">String</span></span>|<span data-ttu-id="57afc-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="57afc-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="57afc-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-139">description</span><span class="sxs-lookup"><span data-stu-id="57afc-139">description</span></span>|<span data-ttu-id="57afc-140">String</span><span class="sxs-lookup"><span data-stu-id="57afc-140">String</span></span>|<span data-ttu-id="57afc-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="57afc-141">The description of the app.</span></span> <span data-ttu-id="57afc-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-143">publisher</span><span class="sxs-lookup"><span data-stu-id="57afc-143">publisher</span></span>|<span data-ttu-id="57afc-144">String</span><span class="sxs-lookup"><span data-stu-id="57afc-144">String</span></span>|<span data-ttu-id="57afc-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="57afc-145">The publisher of the app.</span></span> <span data-ttu-id="57afc-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="57afc-147">largeIcon</span></span>|[<span data-ttu-id="57afc-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="57afc-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="57afc-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="57afc-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="57afc-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57afc-151">createdDateTime</span></span>|<span data-ttu-id="57afc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57afc-152">DateTimeOffset</span></span>|<span data-ttu-id="57afc-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="57afc-153">The date and time the app was created.</span></span> <span data-ttu-id="57afc-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57afc-155">lastModifiedDateTime</span></span>|<span data-ttu-id="57afc-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57afc-156">DateTimeOffset</span></span>|<span data-ttu-id="57afc-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="57afc-157">The date and time the app was last modified.</span></span> <span data-ttu-id="57afc-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="57afc-159">isFeatured</span></span>|<span data-ttu-id="57afc-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="57afc-160">Boolean</span></span>|<span data-ttu-id="57afc-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="57afc-162">privacyInformationUrl</span></span>|<span data-ttu-id="57afc-163">String</span><span class="sxs-lookup"><span data-stu-id="57afc-163">String</span></span>|<span data-ttu-id="57afc-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="57afc-164">The privacy statement Url.</span></span> <span data-ttu-id="57afc-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="57afc-166">informationUrl</span></span>|<span data-ttu-id="57afc-167">String</span><span class="sxs-lookup"><span data-stu-id="57afc-167">String</span></span>|<span data-ttu-id="57afc-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="57afc-168">The more information Url.</span></span> <span data-ttu-id="57afc-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-170">owner</span><span class="sxs-lookup"><span data-stu-id="57afc-170">owner</span></span>|<span data-ttu-id="57afc-171">String</span><span class="sxs-lookup"><span data-stu-id="57afc-171">String</span></span>|<span data-ttu-id="57afc-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="57afc-172">The owner of the app.</span></span> <span data-ttu-id="57afc-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-174">developer</span><span class="sxs-lookup"><span data-stu-id="57afc-174">developer</span></span>|<span data-ttu-id="57afc-175">String</span><span class="sxs-lookup"><span data-stu-id="57afc-175">String</span></span>|<span data-ttu-id="57afc-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="57afc-176">The developer of the app.</span></span> <span data-ttu-id="57afc-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-178">notes</span><span class="sxs-lookup"><span data-stu-id="57afc-178">notes</span></span>|<span data-ttu-id="57afc-179">String</span><span class="sxs-lookup"><span data-stu-id="57afc-179">String</span></span>|<span data-ttu-id="57afc-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="57afc-180">Notes for the app.</span></span> <span data-ttu-id="57afc-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="57afc-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="57afc-182">publishingState</span></span>|[<span data-ttu-id="57afc-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="57afc-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="57afc-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="57afc-184">The publishing state for the app.</span></span> <span data-ttu-id="57afc-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="57afc-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="57afc-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57afc-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="57afc-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="57afc-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="57afc-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="57afc-188">usedLicenseCount</span></span>|<span data-ttu-id="57afc-189">Int32</span><span class="sxs-lookup"><span data-stu-id="57afc-189">Int32</span></span>|<span data-ttu-id="57afc-190">Количество используемых лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="57afc-190">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="57afc-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="57afc-191">totalLicenseCount</span></span>|<span data-ttu-id="57afc-192">Int32</span><span class="sxs-lookup"><span data-stu-id="57afc-192">Int32</span></span>|<span data-ttu-id="57afc-193">Общее количество лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="57afc-193">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="57afc-194">productKey</span><span class="sxs-lookup"><span data-stu-id="57afc-194">productKey</span></span>|<span data-ttu-id="57afc-195">Строка</span><span class="sxs-lookup"><span data-stu-id="57afc-195">String</span></span>|<span data-ttu-id="57afc-196">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="57afc-196">The app product key</span></span>|
|<span data-ttu-id="57afc-197">licenseType</span><span class="sxs-lookup"><span data-stu-id="57afc-197">licenseType</span></span>|[<span data-ttu-id="57afc-198">Микрософтсторефорбусинесслиценсетипе</span><span class="sxs-lookup"><span data-stu-id="57afc-198">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="57afc-199">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="57afc-199">The app license type.</span></span> <span data-ttu-id="57afc-200">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="57afc-200">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="57afc-201">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="57afc-201">packageIdentityName</span></span>|<span data-ttu-id="57afc-202">String</span><span class="sxs-lookup"><span data-stu-id="57afc-202">String</span></span>|<span data-ttu-id="57afc-203">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="57afc-203">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="57afc-204">Ответ</span><span class="sxs-lookup"><span data-stu-id="57afc-204">Response</span></span>
<span data-ttu-id="57afc-205">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="57afc-205">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57afc-206">Пример</span><span class="sxs-lookup"><span data-stu-id="57afc-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="57afc-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="57afc-207">Request</span></span>
<span data-ttu-id="57afc-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57afc-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 769

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
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="57afc-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="57afc-209">Response</span></span>
<span data-ttu-id="57afc-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57afc-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 941

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
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```



