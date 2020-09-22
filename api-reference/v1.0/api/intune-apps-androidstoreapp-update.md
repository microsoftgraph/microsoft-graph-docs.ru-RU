---
title: Update androidStoreApp
description: Обновление свойств объекта androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d8a6b0c39cf81c36c787982df1f178453800b90a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992316"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="0c859-103">Update androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="0c859-103">Update androidStoreApp</span></span>

<span data-ttu-id="0c859-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c859-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c859-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c859-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c859-106">Обновление свойств объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-106">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c859-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0c859-107">Prerequisites</span></span>
<span data-ttu-id="0c859-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c859-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c859-110">Permission type</span></span>|<span data-ttu-id="0c859-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c859-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c859-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c859-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c859-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c859-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c859-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c859-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c859-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c859-115">Not supported.</span></span>|
|<span data-ttu-id="0c859-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c859-116">Application</span></span>|<span data-ttu-id="0c859-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c859-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c859-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c859-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="0c859-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0c859-119">Request headers</span></span>
|<span data-ttu-id="0c859-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c859-120">Header</span></span>|<span data-ttu-id="0c859-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0c859-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c859-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c859-122">Authorization</span></span>|<span data-ttu-id="0c859-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c859-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c859-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0c859-124">Accept</span></span>|<span data-ttu-id="0c859-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c859-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c859-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c859-126">Request body</span></span>
<span data-ttu-id="0c859-127">В теле запроса добавьте представление объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c859-127">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="0c859-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-128">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="0c859-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c859-129">Property</span></span>|<span data-ttu-id="0c859-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0c859-130">Type</span></span>|<span data-ttu-id="0c859-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0c859-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c859-132">id</span><span class="sxs-lookup"><span data-stu-id="0c859-132">id</span></span>|<span data-ttu-id="0c859-133">String</span><span class="sxs-lookup"><span data-stu-id="0c859-133">String</span></span>|<span data-ttu-id="0c859-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0c859-134">Key of the entity.</span></span> <span data-ttu-id="0c859-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0c859-136">displayName</span></span>|<span data-ttu-id="0c859-137">String</span><span class="sxs-lookup"><span data-stu-id="0c859-137">String</span></span>|<span data-ttu-id="0c859-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="0c859-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0c859-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-140">description</span><span class="sxs-lookup"><span data-stu-id="0c859-140">description</span></span>|<span data-ttu-id="0c859-141">String</span><span class="sxs-lookup"><span data-stu-id="0c859-141">String</span></span>|<span data-ttu-id="0c859-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="0c859-142">The description of the app.</span></span> <span data-ttu-id="0c859-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-144">publisher</span><span class="sxs-lookup"><span data-stu-id="0c859-144">publisher</span></span>|<span data-ttu-id="0c859-145">String</span><span class="sxs-lookup"><span data-stu-id="0c859-145">String</span></span>|<span data-ttu-id="0c859-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="0c859-146">The publisher of the app.</span></span> <span data-ttu-id="0c859-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0c859-148">largeIcon</span></span>|[<span data-ttu-id="0c859-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0c859-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0c859-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="0c859-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0c859-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c859-152">createdDateTime</span></span>|<span data-ttu-id="0c859-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c859-153">DateTimeOffset</span></span>|<span data-ttu-id="0c859-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="0c859-154">The date and time the app was created.</span></span> <span data-ttu-id="0c859-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c859-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0c859-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c859-157">DateTimeOffset</span></span>|<span data-ttu-id="0c859-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="0c859-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0c859-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0c859-160">isFeatured</span></span>|<span data-ttu-id="0c859-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c859-161">Boolean</span></span>|<span data-ttu-id="0c859-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0c859-163">privacyInformationUrl</span></span>|<span data-ttu-id="0c859-164">String</span><span class="sxs-lookup"><span data-stu-id="0c859-164">String</span></span>|<span data-ttu-id="0c859-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="0c859-165">The privacy statement Url.</span></span> <span data-ttu-id="0c859-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0c859-167">informationUrl</span></span>|<span data-ttu-id="0c859-168">String</span><span class="sxs-lookup"><span data-stu-id="0c859-168">String</span></span>|<span data-ttu-id="0c859-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="0c859-169">The more information Url.</span></span> <span data-ttu-id="0c859-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-171">owner</span><span class="sxs-lookup"><span data-stu-id="0c859-171">owner</span></span>|<span data-ttu-id="0c859-172">String</span><span class="sxs-lookup"><span data-stu-id="0c859-172">String</span></span>|<span data-ttu-id="0c859-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="0c859-173">The owner of the app.</span></span> <span data-ttu-id="0c859-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-175">developer</span><span class="sxs-lookup"><span data-stu-id="0c859-175">developer</span></span>|<span data-ttu-id="0c859-176">String</span><span class="sxs-lookup"><span data-stu-id="0c859-176">String</span></span>|<span data-ttu-id="0c859-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="0c859-177">The developer of the app.</span></span> <span data-ttu-id="0c859-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-179">notes</span><span class="sxs-lookup"><span data-stu-id="0c859-179">notes</span></span>|<span data-ttu-id="0c859-180">String</span><span class="sxs-lookup"><span data-stu-id="0c859-180">String</span></span>|<span data-ttu-id="0c859-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="0c859-181">Notes for the app.</span></span> <span data-ttu-id="0c859-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0c859-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="0c859-183">publishingState</span></span>|[<span data-ttu-id="0c859-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="0c859-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0c859-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="0c859-185">The publishing state for the app.</span></span> <span data-ttu-id="0c859-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="0c859-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0c859-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0c859-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0c859-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0c859-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0c859-189">packageId</span><span class="sxs-lookup"><span data-stu-id="0c859-189">packageId</span></span>|<span data-ttu-id="0c859-190">String</span><span class="sxs-lookup"><span data-stu-id="0c859-190">String</span></span>|<span data-ttu-id="0c859-191">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="0c859-191">The package identifier.</span></span>|
|<span data-ttu-id="0c859-192">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0c859-192">appStoreUrl</span></span>|<span data-ttu-id="0c859-193">String</span><span class="sxs-lookup"><span data-stu-id="0c859-193">String</span></span>|<span data-ttu-id="0c859-194">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="0c859-194">The Android app store URL.</span></span>|
|<span data-ttu-id="0c859-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0c859-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0c859-196">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0c859-196">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="0c859-197">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="0c859-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="0c859-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c859-198">Response</span></span>
<span data-ttu-id="0c859-199">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0c859-199">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c859-200">Пример</span><span class="sxs-lookup"><span data-stu-id="0c859-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c859-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c859-201">Request</span></span>
<span data-ttu-id="0c859-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c859-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="0c859-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c859-203">Response</span></span>
<span data-ttu-id="0c859-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0c859-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```









