---
title: Update androidStoreApp
description: Обновление свойств объекта androidStoreApp.
ms.openlocfilehash: 1332373eadb0623c7bdd9e606d52a2a1c8875403
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024982"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="c527c-103">Update androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="c527c-103">Update androidStoreApp</span></span>

> <span data-ttu-id="c527c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c527c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c527c-105">Обновление свойств объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-105">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c527c-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c527c-106">Prerequisites</span></span>
<span data-ttu-id="c527c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c527c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c527c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c527c-109">Permission type</span></span>|<span data-ttu-id="c527c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c527c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c527c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c527c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c527c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c527c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c527c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c527c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c527c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c527c-114">Not supported.</span></span>|
|<span data-ttu-id="c527c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c527c-115">Application</span></span>|<span data-ttu-id="c527c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c527c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c527c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c527c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="c527c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c527c-118">Request headers</span></span>
|<span data-ttu-id="c527c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c527c-119">Header</span></span>|<span data-ttu-id="c527c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c527c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c527c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c527c-121">Authorization</span></span>|<span data-ttu-id="c527c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c527c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c527c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c527c-123">Accept</span></span>|<span data-ttu-id="c527c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c527c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c527c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c527c-125">Request body</span></span>
<span data-ttu-id="c527c-126">В теле запроса добавьте представление объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c527c-126">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="c527c-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-127">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="c527c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c527c-128">Property</span></span>|<span data-ttu-id="c527c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c527c-129">Type</span></span>|<span data-ttu-id="c527c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c527c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c527c-131">id</span><span class="sxs-lookup"><span data-stu-id="c527c-131">id</span></span>|<span data-ttu-id="c527c-132">String</span><span class="sxs-lookup"><span data-stu-id="c527c-132">String</span></span>|<span data-ttu-id="c527c-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c527c-133">Key of the entity.</span></span> <span data-ttu-id="c527c-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c527c-135">displayName</span></span>|<span data-ttu-id="c527c-136">String</span><span class="sxs-lookup"><span data-stu-id="c527c-136">String</span></span>|<span data-ttu-id="c527c-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c527c-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c527c-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-139">описание</span><span class="sxs-lookup"><span data-stu-id="c527c-139">description</span></span>|<span data-ttu-id="c527c-140">String</span><span class="sxs-lookup"><span data-stu-id="c527c-140">String</span></span>|<span data-ttu-id="c527c-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c527c-141">The description of the app.</span></span> <span data-ttu-id="c527c-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-143">publisher</span><span class="sxs-lookup"><span data-stu-id="c527c-143">publisher</span></span>|<span data-ttu-id="c527c-144">String</span><span class="sxs-lookup"><span data-stu-id="c527c-144">String</span></span>|<span data-ttu-id="c527c-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c527c-145">The publisher of the app.</span></span> <span data-ttu-id="c527c-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c527c-147">largeIcon</span></span>|[<span data-ttu-id="c527c-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c527c-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c527c-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="c527c-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c527c-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c527c-151">createdDateTime</span></span>|<span data-ttu-id="c527c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c527c-152">DateTimeOffset</span></span>|<span data-ttu-id="c527c-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="c527c-153">The date and time the app was created.</span></span> <span data-ttu-id="c527c-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c527c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="c527c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c527c-156">DateTimeOffset</span></span>|<span data-ttu-id="c527c-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="c527c-157">The date and time the app was last modified.</span></span> <span data-ttu-id="c527c-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c527c-159">isFeatured</span></span>|<span data-ttu-id="c527c-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="c527c-160">Boolean</span></span>|<span data-ttu-id="c527c-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c527c-162">privacyInformationUrl</span></span>|<span data-ttu-id="c527c-163">String</span><span class="sxs-lookup"><span data-stu-id="c527c-163">String</span></span>|<span data-ttu-id="c527c-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c527c-164">The privacy statement Url.</span></span> <span data-ttu-id="c527c-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c527c-166">informationUrl</span></span>|<span data-ttu-id="c527c-167">String</span><span class="sxs-lookup"><span data-stu-id="c527c-167">String</span></span>|<span data-ttu-id="c527c-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="c527c-168">The more information Url.</span></span> <span data-ttu-id="c527c-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-170">owner</span><span class="sxs-lookup"><span data-stu-id="c527c-170">owner</span></span>|<span data-ttu-id="c527c-171">String</span><span class="sxs-lookup"><span data-stu-id="c527c-171">String</span></span>|<span data-ttu-id="c527c-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="c527c-172">The owner of the app.</span></span> <span data-ttu-id="c527c-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-174">developer</span><span class="sxs-lookup"><span data-stu-id="c527c-174">developer</span></span>|<span data-ttu-id="c527c-175">String</span><span class="sxs-lookup"><span data-stu-id="c527c-175">String</span></span>|<span data-ttu-id="c527c-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="c527c-176">The developer of the app.</span></span> <span data-ttu-id="c527c-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-178">notes</span><span class="sxs-lookup"><span data-stu-id="c527c-178">notes</span></span>|<span data-ttu-id="c527c-179">String</span><span class="sxs-lookup"><span data-stu-id="c527c-179">String</span></span>|<span data-ttu-id="c527c-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="c527c-180">Notes for the app.</span></span> <span data-ttu-id="c527c-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c527c-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="c527c-182">publishingState</span></span>|[<span data-ttu-id="c527c-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c527c-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c527c-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="c527c-184">The publishing state for the app.</span></span> <span data-ttu-id="c527c-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="c527c-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c527c-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c527c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c527c-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c527c-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c527c-188">packageId</span><span class="sxs-lookup"><span data-stu-id="c527c-188">packageId</span></span>|<span data-ttu-id="c527c-189">String</span><span class="sxs-lookup"><span data-stu-id="c527c-189">String</span></span>|<span data-ttu-id="c527c-190">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="c527c-190">The package identifier.</span></span>|
|<span data-ttu-id="c527c-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c527c-191">appStoreUrl</span></span>|<span data-ttu-id="c527c-192">String</span><span class="sxs-lookup"><span data-stu-id="c527c-192">String</span></span>|<span data-ttu-id="c527c-193">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="c527c-193">The Android app store URL.</span></span>|
|<span data-ttu-id="c527c-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c527c-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c527c-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c527c-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="c527c-196">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="c527c-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="c527c-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="c527c-197">Response</span></span>
<span data-ttu-id="c527c-198">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c527c-198">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c527c-199">Пример</span><span class="sxs-lookup"><span data-stu-id="c527c-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="c527c-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="c527c-200">Request</span></span>
<span data-ttu-id="c527c-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c527c-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c527c-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="c527c-202">Response</span></span>
<span data-ttu-id="c527c-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c527c-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



