---
title: Create iosStoreApp
description: Создание объекта iosStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8cc760c71480e796be1e36ca37a74f0531e878f1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196205"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="550a6-103">Create iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="550a6-103">Create iosStoreApp</span></span>

> <span data-ttu-id="550a6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="550a6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="550a6-105">Создание объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-105">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="550a6-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="550a6-106">Prerequisites</span></span>
<span data-ttu-id="550a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="550a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="550a6-109">Permission type</span></span>|<span data-ttu-id="550a6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="550a6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="550a6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="550a6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="550a6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="550a6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="550a6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="550a6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="550a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="550a6-114">Not supported.</span></span>|
|<span data-ttu-id="550a6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="550a6-115">Application</span></span>|<span data-ttu-id="550a6-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="550a6-116">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="550a6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="550a6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="550a6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="550a6-118">Request headers</span></span>
|<span data-ttu-id="550a6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="550a6-119">Header</span></span>|<span data-ttu-id="550a6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="550a6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="550a6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="550a6-121">Authorization</span></span>|<span data-ttu-id="550a6-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="550a6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="550a6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="550a6-123">Accept</span></span>|<span data-ttu-id="550a6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="550a6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="550a6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="550a6-125">Request body</span></span>
<span data-ttu-id="550a6-126">В теле запроса добавьте представление объекта iosStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="550a6-126">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="550a6-127">Ниже показаны свойства, которые необходимо указывать при создании объекта iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="550a6-127">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="550a6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="550a6-128">Property</span></span>|<span data-ttu-id="550a6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="550a6-129">Type</span></span>|<span data-ttu-id="550a6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="550a6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="550a6-131">id</span><span class="sxs-lookup"><span data-stu-id="550a6-131">id</span></span>|<span data-ttu-id="550a6-132">Строка</span><span class="sxs-lookup"><span data-stu-id="550a6-132">String</span></span>|<span data-ttu-id="550a6-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="550a6-133">Key of the entity.</span></span> <span data-ttu-id="550a6-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="550a6-135">displayName</span></span>|<span data-ttu-id="550a6-136">Строка</span><span class="sxs-lookup"><span data-stu-id="550a6-136">String</span></span>|<span data-ttu-id="550a6-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="550a6-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="550a6-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-139">description</span><span class="sxs-lookup"><span data-stu-id="550a6-139">description</span></span>|<span data-ttu-id="550a6-140">Строка</span><span class="sxs-lookup"><span data-stu-id="550a6-140">String</span></span>|<span data-ttu-id="550a6-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="550a6-141">The description of the app.</span></span> <span data-ttu-id="550a6-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-143">publisher</span><span class="sxs-lookup"><span data-stu-id="550a6-143">publisher</span></span>|<span data-ttu-id="550a6-144">String.</span><span class="sxs-lookup"><span data-stu-id="550a6-144">String</span></span>|<span data-ttu-id="550a6-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="550a6-145">The publisher of the app.</span></span> <span data-ttu-id="550a6-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="550a6-147">largeIcon</span></span>|[<span data-ttu-id="550a6-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="550a6-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="550a6-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="550a6-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="550a6-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="550a6-151">createdDateTime</span></span>|<span data-ttu-id="550a6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="550a6-152">DateTimeOffset</span></span>|<span data-ttu-id="550a6-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="550a6-153">The date and time the app was created.</span></span> <span data-ttu-id="550a6-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="550a6-155">lastModifiedDateTime</span></span>|<span data-ttu-id="550a6-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="550a6-156">DateTimeOffset</span></span>|<span data-ttu-id="550a6-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="550a6-157">The date and time the app was last modified.</span></span> <span data-ttu-id="550a6-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="550a6-159">isFeatured</span></span>|<span data-ttu-id="550a6-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="550a6-160">Boolean</span></span>|<span data-ttu-id="550a6-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="550a6-162">privacyInformationUrl</span></span>|<span data-ttu-id="550a6-163">String.</span><span class="sxs-lookup"><span data-stu-id="550a6-163">String</span></span>|<span data-ttu-id="550a6-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="550a6-164">The privacy statement Url.</span></span> <span data-ttu-id="550a6-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="550a6-166">informationUrl</span></span>|<span data-ttu-id="550a6-167">String.</span><span class="sxs-lookup"><span data-stu-id="550a6-167">String</span></span>|<span data-ttu-id="550a6-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="550a6-168">The more information Url.</span></span> <span data-ttu-id="550a6-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-170">owner</span><span class="sxs-lookup"><span data-stu-id="550a6-170">owner</span></span>|<span data-ttu-id="550a6-171">String</span><span class="sxs-lookup"><span data-stu-id="550a6-171">String</span></span>|<span data-ttu-id="550a6-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="550a6-172">The owner of the app.</span></span> <span data-ttu-id="550a6-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-174">developer</span><span class="sxs-lookup"><span data-stu-id="550a6-174">developer</span></span>|<span data-ttu-id="550a6-175">String.</span><span class="sxs-lookup"><span data-stu-id="550a6-175">String</span></span>|<span data-ttu-id="550a6-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="550a6-176">The developer of the app.</span></span> <span data-ttu-id="550a6-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-178">notes</span><span class="sxs-lookup"><span data-stu-id="550a6-178">notes</span></span>|<span data-ttu-id="550a6-179">String.</span><span class="sxs-lookup"><span data-stu-id="550a6-179">String</span></span>|<span data-ttu-id="550a6-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="550a6-180">Notes for the app.</span></span> <span data-ttu-id="550a6-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="550a6-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="550a6-182">publishingState</span></span>|[<span data-ttu-id="550a6-183">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="550a6-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="550a6-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="550a6-184">The publishing state for the app.</span></span> <span data-ttu-id="550a6-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="550a6-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="550a6-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="550a6-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="550a6-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="550a6-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="550a6-188">bundleId</span><span class="sxs-lookup"><span data-stu-id="550a6-188">bundleId</span></span>|<span data-ttu-id="550a6-189">String</span><span class="sxs-lookup"><span data-stu-id="550a6-189">String</span></span>|<span data-ttu-id="550a6-190">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="550a6-190">The Identity Name.</span></span>|
|<span data-ttu-id="550a6-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="550a6-191">appStoreUrl</span></span>|<span data-ttu-id="550a6-192">String</span><span class="sxs-lookup"><span data-stu-id="550a6-192">String</span></span>|<span data-ttu-id="550a6-193">URL-адрес в Apple App Store</span><span class="sxs-lookup"><span data-stu-id="550a6-193">The Apple App Store URL</span></span>|
|<span data-ttu-id="550a6-194">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="550a6-194">applicableDeviceType</span></span>|[<span data-ttu-id="550a6-195">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="550a6-195">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="550a6-196">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="550a6-196">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="550a6-197">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="550a6-197">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="550a6-198">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="550a6-198">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="550a6-199">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="550a6-199">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="550a6-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="550a6-200">Response</span></span>
<span data-ttu-id="550a6-201">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="550a6-201">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="550a6-202">Пример</span><span class="sxs-lookup"><span data-stu-id="550a6-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="550a6-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="550a6-203">Request</span></span>
<span data-ttu-id="550a6-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="550a6-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1026

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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

### <a name="response"></a><span data-ttu-id="550a6-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="550a6-205">Response</span></span>
<span data-ttu-id="550a6-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="550a6-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1198

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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



