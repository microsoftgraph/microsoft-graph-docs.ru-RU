---
title: Update iosStoreApp
description: Обновление свойств объекта iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ea6354c3d6e2996ab15903f1ad38ee9f1079478c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070130"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="10dfb-103">Update iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="10dfb-103">Update iosStoreApp</span></span>

<span data-ttu-id="10dfb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10dfb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10dfb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10dfb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10dfb-106">Обновление свойств объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-106">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10dfb-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="10dfb-107">Prerequisites</span></span>
<span data-ttu-id="10dfb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="10dfb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10dfb-110">Permission type</span></span>|<span data-ttu-id="10dfb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10dfb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10dfb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10dfb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10dfb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10dfb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="10dfb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10dfb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10dfb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10dfb-115">Not supported.</span></span>|
|<span data-ttu-id="10dfb-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="10dfb-116">Application</span></span>|<span data-ttu-id="10dfb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10dfb-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10dfb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10dfb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="10dfb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="10dfb-119">Request headers</span></span>
|<span data-ttu-id="10dfb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10dfb-120">Header</span></span>|<span data-ttu-id="10dfb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="10dfb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10dfb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10dfb-122">Authorization</span></span>|<span data-ttu-id="10dfb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10dfb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10dfb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="10dfb-124">Accept</span></span>|<span data-ttu-id="10dfb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10dfb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10dfb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10dfb-126">Request body</span></span>
<span data-ttu-id="10dfb-127">В тексте запроса добавьте представление объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10dfb-127">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="10dfb-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-128">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="10dfb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="10dfb-129">Property</span></span>|<span data-ttu-id="10dfb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="10dfb-130">Type</span></span>|<span data-ttu-id="10dfb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="10dfb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10dfb-132">id</span><span class="sxs-lookup"><span data-stu-id="10dfb-132">id</span></span>|<span data-ttu-id="10dfb-133">Строка</span><span class="sxs-lookup"><span data-stu-id="10dfb-133">String</span></span>|<span data-ttu-id="10dfb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="10dfb-134">Key of the entity.</span></span> <span data-ttu-id="10dfb-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="10dfb-136">displayName</span></span>|<span data-ttu-id="10dfb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="10dfb-137">String</span></span>|<span data-ttu-id="10dfb-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="10dfb-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="10dfb-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-140">description</span><span class="sxs-lookup"><span data-stu-id="10dfb-140">description</span></span>|<span data-ttu-id="10dfb-141">Строка</span><span class="sxs-lookup"><span data-stu-id="10dfb-141">String</span></span>|<span data-ttu-id="10dfb-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="10dfb-142">The description of the app.</span></span> <span data-ttu-id="10dfb-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-144">publisher</span><span class="sxs-lookup"><span data-stu-id="10dfb-144">publisher</span></span>|<span data-ttu-id="10dfb-145">String</span><span class="sxs-lookup"><span data-stu-id="10dfb-145">String</span></span>|<span data-ttu-id="10dfb-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="10dfb-146">The publisher of the app.</span></span> <span data-ttu-id="10dfb-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="10dfb-148">largeIcon</span></span>|[<span data-ttu-id="10dfb-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="10dfb-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="10dfb-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="10dfb-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="10dfb-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10dfb-152">createdDateTime</span></span>|<span data-ttu-id="10dfb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10dfb-153">DateTimeOffset</span></span>|<span data-ttu-id="10dfb-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="10dfb-154">The date and time the app was created.</span></span> <span data-ttu-id="10dfb-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10dfb-156">lastModifiedDateTime</span></span>|<span data-ttu-id="10dfb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10dfb-157">DateTimeOffset</span></span>|<span data-ttu-id="10dfb-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="10dfb-158">The date and time the app was last modified.</span></span> <span data-ttu-id="10dfb-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="10dfb-160">isFeatured</span></span>|<span data-ttu-id="10dfb-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="10dfb-161">Boolean</span></span>|<span data-ttu-id="10dfb-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="10dfb-163">privacyInformationUrl</span></span>|<span data-ttu-id="10dfb-164">String</span><span class="sxs-lookup"><span data-stu-id="10dfb-164">String</span></span>|<span data-ttu-id="10dfb-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="10dfb-165">The privacy statement Url.</span></span> <span data-ttu-id="10dfb-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="10dfb-167">informationUrl</span></span>|<span data-ttu-id="10dfb-168">String</span><span class="sxs-lookup"><span data-stu-id="10dfb-168">String</span></span>|<span data-ttu-id="10dfb-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="10dfb-169">The more information Url.</span></span> <span data-ttu-id="10dfb-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-171">owner</span><span class="sxs-lookup"><span data-stu-id="10dfb-171">owner</span></span>|<span data-ttu-id="10dfb-172">String</span><span class="sxs-lookup"><span data-stu-id="10dfb-172">String</span></span>|<span data-ttu-id="10dfb-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="10dfb-173">The owner of the app.</span></span> <span data-ttu-id="10dfb-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-175">developer</span><span class="sxs-lookup"><span data-stu-id="10dfb-175">developer</span></span>|<span data-ttu-id="10dfb-176">String</span><span class="sxs-lookup"><span data-stu-id="10dfb-176">String</span></span>|<span data-ttu-id="10dfb-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="10dfb-177">The developer of the app.</span></span> <span data-ttu-id="10dfb-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-179">notes</span><span class="sxs-lookup"><span data-stu-id="10dfb-179">notes</span></span>|<span data-ttu-id="10dfb-180">String</span><span class="sxs-lookup"><span data-stu-id="10dfb-180">String</span></span>|<span data-ttu-id="10dfb-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="10dfb-181">Notes for the app.</span></span> <span data-ttu-id="10dfb-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="10dfb-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="10dfb-183">publishingState</span></span>|[<span data-ttu-id="10dfb-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="10dfb-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="10dfb-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="10dfb-185">The publishing state for the app.</span></span> <span data-ttu-id="10dfb-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="10dfb-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="10dfb-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="10dfb-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="10dfb-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="10dfb-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="10dfb-189">bundleId</span><span class="sxs-lookup"><span data-stu-id="10dfb-189">bundleId</span></span>|<span data-ttu-id="10dfb-190">String</span><span class="sxs-lookup"><span data-stu-id="10dfb-190">String</span></span>|<span data-ttu-id="10dfb-191">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="10dfb-191">The Identity Name.</span></span>|
|<span data-ttu-id="10dfb-192">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="10dfb-192">appStoreUrl</span></span>|<span data-ttu-id="10dfb-193">String</span><span class="sxs-lookup"><span data-stu-id="10dfb-193">String</span></span>|<span data-ttu-id="10dfb-194">URL-адрес в Apple App Store</span><span class="sxs-lookup"><span data-stu-id="10dfb-194">The Apple App Store URL</span></span>|
|<span data-ttu-id="10dfb-195">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="10dfb-195">applicableDeviceType</span></span>|[<span data-ttu-id="10dfb-196">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="10dfb-196">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="10dfb-197">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="10dfb-197">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="10dfb-198">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="10dfb-198">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="10dfb-199">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="10dfb-199">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="10dfb-200">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="10dfb-200">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="10dfb-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="10dfb-201">Response</span></span>
<span data-ttu-id="10dfb-202">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="10dfb-202">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10dfb-203">Пример</span><span class="sxs-lookup"><span data-stu-id="10dfb-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="10dfb-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="10dfb-204">Request</span></span>
<span data-ttu-id="10dfb-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10dfb-205">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="10dfb-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="10dfb-206">Response</span></span>
<span data-ttu-id="10dfb-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10dfb-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









