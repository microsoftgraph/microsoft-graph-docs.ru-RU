---
title: Create microsoftStoreForBusinessApp
description: Создание объекта microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc3b4f8b4a7e82aa888cb4b843e15499724d6bec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073231"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="dcde6-103">Create microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="dcde6-103">Create microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="dcde6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcde6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcde6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dcde6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcde6-106">Создание объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcde6-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dcde6-107">Prerequisites</span></span>
<span data-ttu-id="dcde6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcde6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcde6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcde6-110">Permission type</span></span>|<span data-ttu-id="dcde6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcde6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcde6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcde6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dcde6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcde6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dcde6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcde6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcde6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcde6-115">Not supported.</span></span>|
|<span data-ttu-id="dcde6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dcde6-116">Application</span></span>|<span data-ttu-id="dcde6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcde6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcde6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcde6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="dcde6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dcde6-119">Request headers</span></span>
|<span data-ttu-id="dcde6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dcde6-120">Header</span></span>|<span data-ttu-id="dcde6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dcde6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcde6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcde6-122">Authorization</span></span>|<span data-ttu-id="dcde6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcde6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcde6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dcde6-124">Accept</span></span>|<span data-ttu-id="dcde6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dcde6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcde6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dcde6-126">Request body</span></span>
<span data-ttu-id="dcde6-127">В тексте запроса добавьте представление объекта microsoftStoreForBusinessApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcde6-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="dcde6-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="dcde6-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="dcde6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dcde6-129">Property</span></span>|<span data-ttu-id="dcde6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dcde6-130">Type</span></span>|<span data-ttu-id="dcde6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dcde6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcde6-132">id</span><span class="sxs-lookup"><span data-stu-id="dcde6-132">id</span></span>|<span data-ttu-id="dcde6-133">Строка</span><span class="sxs-lookup"><span data-stu-id="dcde6-133">String</span></span>|<span data-ttu-id="dcde6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dcde6-134">Key of the entity.</span></span> <span data-ttu-id="dcde6-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="dcde6-136">displayName</span></span>|<span data-ttu-id="dcde6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="dcde6-137">String</span></span>|<span data-ttu-id="dcde6-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="dcde6-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dcde6-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-140">description</span><span class="sxs-lookup"><span data-stu-id="dcde6-140">description</span></span>|<span data-ttu-id="dcde6-141">Строка</span><span class="sxs-lookup"><span data-stu-id="dcde6-141">String</span></span>|<span data-ttu-id="dcde6-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="dcde6-142">The description of the app.</span></span> <span data-ttu-id="dcde6-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-144">publisher</span><span class="sxs-lookup"><span data-stu-id="dcde6-144">publisher</span></span>|<span data-ttu-id="dcde6-145">String</span><span class="sxs-lookup"><span data-stu-id="dcde6-145">String</span></span>|<span data-ttu-id="dcde6-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="dcde6-146">The publisher of the app.</span></span> <span data-ttu-id="dcde6-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dcde6-148">largeIcon</span></span>|[<span data-ttu-id="dcde6-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dcde6-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dcde6-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="dcde6-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dcde6-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dcde6-152">createdDateTime</span></span>|<span data-ttu-id="dcde6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcde6-153">DateTimeOffset</span></span>|<span data-ttu-id="dcde6-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="dcde6-154">The date and time the app was created.</span></span> <span data-ttu-id="dcde6-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dcde6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="dcde6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcde6-157">DateTimeOffset</span></span>|<span data-ttu-id="dcde6-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="dcde6-158">The date and time the app was last modified.</span></span> <span data-ttu-id="dcde6-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dcde6-160">isFeatured</span></span>|<span data-ttu-id="dcde6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="dcde6-161">Boolean</span></span>|<span data-ttu-id="dcde6-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dcde6-163">privacyInformationUrl</span></span>|<span data-ttu-id="dcde6-164">String</span><span class="sxs-lookup"><span data-stu-id="dcde6-164">String</span></span>|<span data-ttu-id="dcde6-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="dcde6-165">The privacy statement Url.</span></span> <span data-ttu-id="dcde6-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dcde6-167">informationUrl</span></span>|<span data-ttu-id="dcde6-168">String</span><span class="sxs-lookup"><span data-stu-id="dcde6-168">String</span></span>|<span data-ttu-id="dcde6-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="dcde6-169">The more information Url.</span></span> <span data-ttu-id="dcde6-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-171">owner</span><span class="sxs-lookup"><span data-stu-id="dcde6-171">owner</span></span>|<span data-ttu-id="dcde6-172">String</span><span class="sxs-lookup"><span data-stu-id="dcde6-172">String</span></span>|<span data-ttu-id="dcde6-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="dcde6-173">The owner of the app.</span></span> <span data-ttu-id="dcde6-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-175">developer</span><span class="sxs-lookup"><span data-stu-id="dcde6-175">developer</span></span>|<span data-ttu-id="dcde6-176">String</span><span class="sxs-lookup"><span data-stu-id="dcde6-176">String</span></span>|<span data-ttu-id="dcde6-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="dcde6-177">The developer of the app.</span></span> <span data-ttu-id="dcde6-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-179">notes</span><span class="sxs-lookup"><span data-stu-id="dcde6-179">notes</span></span>|<span data-ttu-id="dcde6-180">String</span><span class="sxs-lookup"><span data-stu-id="dcde6-180">String</span></span>|<span data-ttu-id="dcde6-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="dcde6-181">Notes for the app.</span></span> <span data-ttu-id="dcde6-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dcde6-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="dcde6-183">publishingState</span></span>|[<span data-ttu-id="dcde6-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="dcde6-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dcde6-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="dcde6-185">The publishing state for the app.</span></span> <span data-ttu-id="dcde6-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="dcde6-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dcde6-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcde6-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dcde6-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="dcde6-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dcde6-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="dcde6-189">usedLicenseCount</span></span>|<span data-ttu-id="dcde6-190">Int32</span><span class="sxs-lookup"><span data-stu-id="dcde6-190">Int32</span></span>|<span data-ttu-id="dcde6-191">Количество используемых лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="dcde6-191">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="dcde6-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="dcde6-192">totalLicenseCount</span></span>|<span data-ttu-id="dcde6-193">Int32</span><span class="sxs-lookup"><span data-stu-id="dcde6-193">Int32</span></span>|<span data-ttu-id="dcde6-194">Общее количество лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="dcde6-194">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="dcde6-195">productKey</span><span class="sxs-lookup"><span data-stu-id="dcde6-195">productKey</span></span>|<span data-ttu-id="dcde6-196">String</span><span class="sxs-lookup"><span data-stu-id="dcde6-196">String</span></span>|<span data-ttu-id="dcde6-197">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="dcde6-197">The app product key</span></span>|
|<span data-ttu-id="dcde6-198">licenseType</span><span class="sxs-lookup"><span data-stu-id="dcde6-198">licenseType</span></span>|[<span data-ttu-id="dcde6-199">микрософтсторефорбусинесслиценсетипе</span><span class="sxs-lookup"><span data-stu-id="dcde6-199">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="dcde6-200">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="dcde6-200">The app license type.</span></span> <span data-ttu-id="dcde6-201">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="dcde6-201">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="dcde6-202">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="dcde6-202">packageIdentityName</span></span>|<span data-ttu-id="dcde6-203">String</span><span class="sxs-lookup"><span data-stu-id="dcde6-203">String</span></span>|<span data-ttu-id="dcde6-204">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="dcde6-204">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="dcde6-205">Ответ</span><span class="sxs-lookup"><span data-stu-id="dcde6-205">Response</span></span>
<span data-ttu-id="dcde6-206">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dcde6-206">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcde6-207">Пример</span><span class="sxs-lookup"><span data-stu-id="dcde6-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcde6-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcde6-208">Request</span></span>
<span data-ttu-id="dcde6-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcde6-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="dcde6-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcde6-210">Response</span></span>
<span data-ttu-id="dcde6-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dcde6-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









