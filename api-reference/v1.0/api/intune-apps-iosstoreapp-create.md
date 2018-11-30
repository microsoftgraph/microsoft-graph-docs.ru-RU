---
title: Create iosStoreApp
description: Создание объекта iosStoreApp.
ms.openlocfilehash: 7dbf1dd5ff0318d054d99bc4f7ae9a8fcfce8523
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026861"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="84bea-103">Create iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="84bea-103">Create iosStoreApp</span></span>

> <span data-ttu-id="84bea-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="84bea-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84bea-105">Создание объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-105">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84bea-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="84bea-106">Prerequisites</span></span>
<span data-ttu-id="84bea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84bea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84bea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84bea-109">Permission type</span></span>|<span data-ttu-id="84bea-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84bea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84bea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84bea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="84bea-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84bea-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="84bea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84bea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84bea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84bea-114">Not supported.</span></span>|
|<span data-ttu-id="84bea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84bea-115">Application</span></span>|<span data-ttu-id="84bea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84bea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84bea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84bea-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="84bea-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84bea-118">Request headers</span></span>
|<span data-ttu-id="84bea-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84bea-119">Header</span></span>|<span data-ttu-id="84bea-120">Значение</span><span class="sxs-lookup"><span data-stu-id="84bea-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84bea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="84bea-121">Authorization</span></span>|<span data-ttu-id="84bea-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="84bea-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84bea-123">Accept</span><span class="sxs-lookup"><span data-stu-id="84bea-123">Accept</span></span>|<span data-ttu-id="84bea-124">application/json</span><span class="sxs-lookup"><span data-stu-id="84bea-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84bea-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84bea-125">Request body</span></span>
<span data-ttu-id="84bea-126">В теле запроса добавьте представление объекта iosStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84bea-126">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="84bea-127">Ниже показаны свойства, которые необходимо указывать при создании объекта iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="84bea-127">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="84bea-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="84bea-128">Property</span></span>|<span data-ttu-id="84bea-129">Тип</span><span class="sxs-lookup"><span data-stu-id="84bea-129">Type</span></span>|<span data-ttu-id="84bea-130">Описание</span><span class="sxs-lookup"><span data-stu-id="84bea-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84bea-131">id</span><span class="sxs-lookup"><span data-stu-id="84bea-131">id</span></span>|<span data-ttu-id="84bea-132">String</span><span class="sxs-lookup"><span data-stu-id="84bea-132">String</span></span>|<span data-ttu-id="84bea-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="84bea-133">Key of the entity.</span></span> <span data-ttu-id="84bea-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-135">displayName</span><span class="sxs-lookup"><span data-stu-id="84bea-135">displayName</span></span>|<span data-ttu-id="84bea-136">String</span><span class="sxs-lookup"><span data-stu-id="84bea-136">String</span></span>|<span data-ttu-id="84bea-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="84bea-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="84bea-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-139">описание</span><span class="sxs-lookup"><span data-stu-id="84bea-139">description</span></span>|<span data-ttu-id="84bea-140">String</span><span class="sxs-lookup"><span data-stu-id="84bea-140">String</span></span>|<span data-ttu-id="84bea-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="84bea-141">The description of the app.</span></span> <span data-ttu-id="84bea-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-143">publisher</span><span class="sxs-lookup"><span data-stu-id="84bea-143">publisher</span></span>|<span data-ttu-id="84bea-144">String</span><span class="sxs-lookup"><span data-stu-id="84bea-144">String</span></span>|<span data-ttu-id="84bea-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="84bea-145">The publisher of the app.</span></span> <span data-ttu-id="84bea-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="84bea-147">largeIcon</span></span>|[<span data-ttu-id="84bea-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="84bea-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="84bea-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="84bea-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="84bea-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84bea-151">createdDateTime</span></span>|<span data-ttu-id="84bea-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84bea-152">DateTimeOffset</span></span>|<span data-ttu-id="84bea-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="84bea-153">The date and time the app was created.</span></span> <span data-ttu-id="84bea-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84bea-155">lastModifiedDateTime</span></span>|<span data-ttu-id="84bea-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84bea-156">DateTimeOffset</span></span>|<span data-ttu-id="84bea-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="84bea-157">The date and time the app was last modified.</span></span> <span data-ttu-id="84bea-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="84bea-159">isFeatured</span></span>|<span data-ttu-id="84bea-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="84bea-160">Boolean</span></span>|<span data-ttu-id="84bea-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="84bea-162">privacyInformationUrl</span></span>|<span data-ttu-id="84bea-163">String</span><span class="sxs-lookup"><span data-stu-id="84bea-163">String</span></span>|<span data-ttu-id="84bea-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="84bea-164">The privacy statement Url.</span></span> <span data-ttu-id="84bea-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="84bea-166">informationUrl</span></span>|<span data-ttu-id="84bea-167">String</span><span class="sxs-lookup"><span data-stu-id="84bea-167">String</span></span>|<span data-ttu-id="84bea-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="84bea-168">The more information Url.</span></span> <span data-ttu-id="84bea-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-170">owner</span><span class="sxs-lookup"><span data-stu-id="84bea-170">owner</span></span>|<span data-ttu-id="84bea-171">String</span><span class="sxs-lookup"><span data-stu-id="84bea-171">String</span></span>|<span data-ttu-id="84bea-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="84bea-172">The owner of the app.</span></span> <span data-ttu-id="84bea-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-174">developer</span><span class="sxs-lookup"><span data-stu-id="84bea-174">developer</span></span>|<span data-ttu-id="84bea-175">String</span><span class="sxs-lookup"><span data-stu-id="84bea-175">String</span></span>|<span data-ttu-id="84bea-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="84bea-176">The developer of the app.</span></span> <span data-ttu-id="84bea-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-178">notes</span><span class="sxs-lookup"><span data-stu-id="84bea-178">notes</span></span>|<span data-ttu-id="84bea-179">String</span><span class="sxs-lookup"><span data-stu-id="84bea-179">String</span></span>|<span data-ttu-id="84bea-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="84bea-180">Notes for the app.</span></span> <span data-ttu-id="84bea-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="84bea-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="84bea-182">publishingState</span></span>|[<span data-ttu-id="84bea-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="84bea-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="84bea-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="84bea-184">The publishing state for the app.</span></span> <span data-ttu-id="84bea-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="84bea-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="84bea-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84bea-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="84bea-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="84bea-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="84bea-188">bundleId</span><span class="sxs-lookup"><span data-stu-id="84bea-188">bundleId</span></span>|<span data-ttu-id="84bea-189">String</span><span class="sxs-lookup"><span data-stu-id="84bea-189">String</span></span>|<span data-ttu-id="84bea-190">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="84bea-190">The Identity Name.</span></span>|
|<span data-ttu-id="84bea-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="84bea-191">appStoreUrl</span></span>|<span data-ttu-id="84bea-192">String</span><span class="sxs-lookup"><span data-stu-id="84bea-192">String</span></span>|<span data-ttu-id="84bea-193">URL-адрес в Apple App Store</span><span class="sxs-lookup"><span data-stu-id="84bea-193">The Apple App Store URL</span></span>|
|<span data-ttu-id="84bea-194">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="84bea-194">applicableDeviceType</span></span>|[<span data-ttu-id="84bea-195">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="84bea-195">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="84bea-196">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="84bea-196">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="84bea-197">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="84bea-197">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="84bea-198">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="84bea-198">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="84bea-199">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="84bea-199">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="84bea-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="84bea-200">Response</span></span>
<span data-ttu-id="84bea-201">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="84bea-201">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84bea-202">Пример</span><span class="sxs-lookup"><span data-stu-id="84bea-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="84bea-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="84bea-203">Request</span></span>
<span data-ttu-id="84bea-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84bea-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1006

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
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="84bea-205">Ответ</span><span class="sxs-lookup"><span data-stu-id="84bea-205">Response</span></span>
<span data-ttu-id="84bea-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="84bea-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1178

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
    "v12_0": true
  }
}
```



