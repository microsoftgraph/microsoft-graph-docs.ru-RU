---
title: Update iosStoreApp
description: Обновление свойств объекта iosStoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 69b407288c0005747fe27e077bfc7dfcf0477e4a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355563"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="1d903-103">Update iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="1d903-103">Update iosStoreApp</span></span>

> <span data-ttu-id="1d903-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d903-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d903-105">Обновление свойств объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-105">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d903-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1d903-106">Prerequisites</span></span>
<span data-ttu-id="1d903-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1d903-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d903-109">Permission type</span></span>|<span data-ttu-id="1d903-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d903-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d903-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d903-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1d903-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d903-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1d903-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d903-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d903-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d903-114">Not supported.</span></span>|
|<span data-ttu-id="1d903-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d903-115">Application</span></span>|<span data-ttu-id="1d903-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d903-116">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d903-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d903-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="1d903-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d903-118">Request headers</span></span>
|<span data-ttu-id="1d903-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d903-119">Header</span></span>|<span data-ttu-id="1d903-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1d903-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d903-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d903-121">Authorization</span></span>|<span data-ttu-id="1d903-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d903-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d903-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1d903-123">Accept</span></span>|<span data-ttu-id="1d903-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1d903-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d903-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d903-125">Request body</span></span>
<span data-ttu-id="1d903-126">В тексте запроса добавьте представление объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d903-126">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="1d903-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-127">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="1d903-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d903-128">Property</span></span>|<span data-ttu-id="1d903-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1d903-129">Type</span></span>|<span data-ttu-id="1d903-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1d903-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d903-131">id</span><span class="sxs-lookup"><span data-stu-id="1d903-131">id</span></span>|<span data-ttu-id="1d903-132">Строка</span><span class="sxs-lookup"><span data-stu-id="1d903-132">String</span></span>|<span data-ttu-id="1d903-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1d903-133">Key of the entity.</span></span> <span data-ttu-id="1d903-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1d903-135">displayName</span></span>|<span data-ttu-id="1d903-136">Строка</span><span class="sxs-lookup"><span data-stu-id="1d903-136">String</span></span>|<span data-ttu-id="1d903-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="1d903-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1d903-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-139">description</span><span class="sxs-lookup"><span data-stu-id="1d903-139">description</span></span>|<span data-ttu-id="1d903-140">Строка</span><span class="sxs-lookup"><span data-stu-id="1d903-140">String</span></span>|<span data-ttu-id="1d903-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="1d903-141">The description of the app.</span></span> <span data-ttu-id="1d903-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-143">publisher</span><span class="sxs-lookup"><span data-stu-id="1d903-143">publisher</span></span>|<span data-ttu-id="1d903-144">String</span><span class="sxs-lookup"><span data-stu-id="1d903-144">String</span></span>|<span data-ttu-id="1d903-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="1d903-145">The publisher of the app.</span></span> <span data-ttu-id="1d903-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1d903-147">largeIcon</span></span>|[<span data-ttu-id="1d903-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1d903-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1d903-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="1d903-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1d903-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d903-151">createdDateTime</span></span>|<span data-ttu-id="1d903-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d903-152">DateTimeOffset</span></span>|<span data-ttu-id="1d903-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="1d903-153">The date and time the app was created.</span></span> <span data-ttu-id="1d903-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d903-155">lastModifiedDateTime</span></span>|<span data-ttu-id="1d903-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d903-156">DateTimeOffset</span></span>|<span data-ttu-id="1d903-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="1d903-157">The date and time the app was last modified.</span></span> <span data-ttu-id="1d903-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1d903-159">isFeatured</span></span>|<span data-ttu-id="1d903-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d903-160">Boolean</span></span>|<span data-ttu-id="1d903-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1d903-162">privacyInformationUrl</span></span>|<span data-ttu-id="1d903-163">String</span><span class="sxs-lookup"><span data-stu-id="1d903-163">String</span></span>|<span data-ttu-id="1d903-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="1d903-164">The privacy statement Url.</span></span> <span data-ttu-id="1d903-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1d903-166">informationUrl</span></span>|<span data-ttu-id="1d903-167">String</span><span class="sxs-lookup"><span data-stu-id="1d903-167">String</span></span>|<span data-ttu-id="1d903-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="1d903-168">The more information Url.</span></span> <span data-ttu-id="1d903-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-170">owner</span><span class="sxs-lookup"><span data-stu-id="1d903-170">owner</span></span>|<span data-ttu-id="1d903-171">String</span><span class="sxs-lookup"><span data-stu-id="1d903-171">String</span></span>|<span data-ttu-id="1d903-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="1d903-172">The owner of the app.</span></span> <span data-ttu-id="1d903-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-174">developer</span><span class="sxs-lookup"><span data-stu-id="1d903-174">developer</span></span>|<span data-ttu-id="1d903-175">String</span><span class="sxs-lookup"><span data-stu-id="1d903-175">String</span></span>|<span data-ttu-id="1d903-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="1d903-176">The developer of the app.</span></span> <span data-ttu-id="1d903-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-178">notes</span><span class="sxs-lookup"><span data-stu-id="1d903-178">notes</span></span>|<span data-ttu-id="1d903-179">String</span><span class="sxs-lookup"><span data-stu-id="1d903-179">String</span></span>|<span data-ttu-id="1d903-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="1d903-180">Notes for the app.</span></span> <span data-ttu-id="1d903-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1d903-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="1d903-182">publishingState</span></span>|[<span data-ttu-id="1d903-183">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="1d903-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1d903-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="1d903-184">The publishing state for the app.</span></span> <span data-ttu-id="1d903-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="1d903-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1d903-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d903-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1d903-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1d903-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1d903-188">bundleId</span><span class="sxs-lookup"><span data-stu-id="1d903-188">bundleId</span></span>|<span data-ttu-id="1d903-189">String</span><span class="sxs-lookup"><span data-stu-id="1d903-189">String</span></span>|<span data-ttu-id="1d903-190">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="1d903-190">The Identity Name.</span></span>|
|<span data-ttu-id="1d903-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1d903-191">appStoreUrl</span></span>|<span data-ttu-id="1d903-192">String</span><span class="sxs-lookup"><span data-stu-id="1d903-192">String</span></span>|<span data-ttu-id="1d903-193">URL-адрес в Apple App Store</span><span class="sxs-lookup"><span data-stu-id="1d903-193">The Apple App Store URL</span></span>|
|<span data-ttu-id="1d903-194">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1d903-194">applicableDeviceType</span></span>|[<span data-ttu-id="1d903-195">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1d903-195">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="1d903-196">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="1d903-196">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="1d903-197">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1d903-197">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1d903-198">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1d903-198">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="1d903-199">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="1d903-199">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="1d903-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d903-200">Response</span></span>
<span data-ttu-id="1d903-201">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1d903-201">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d903-202">Пример</span><span class="sxs-lookup"><span data-stu-id="1d903-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d903-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d903-203">Request</span></span>
<span data-ttu-id="1d903-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d903-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="1d903-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d903-205">Response</span></span>
<span data-ttu-id="1d903-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d903-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




