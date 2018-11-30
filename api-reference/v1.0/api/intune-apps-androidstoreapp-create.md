---
title: Создание объекта androidStoreApp
description: Создание объекта androidStoreApp.
ms.openlocfilehash: d77aae9acf30d60119d6c00a45530e5a857c0ac1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024981"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="5cf69-103">Создание объекта androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="5cf69-103">Create androidStoreApp</span></span>

> <span data-ttu-id="5cf69-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5cf69-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cf69-105">Создание объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-105">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5cf69-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5cf69-106">Prerequisites</span></span>
<span data-ttu-id="5cf69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cf69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cf69-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5cf69-109">Permission type</span></span>|<span data-ttu-id="5cf69-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5cf69-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cf69-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5cf69-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5cf69-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cf69-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5cf69-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5cf69-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cf69-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cf69-114">Not supported.</span></span>|
|<span data-ttu-id="5cf69-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5cf69-115">Application</span></span>|<span data-ttu-id="5cf69-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cf69-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cf69-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5cf69-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5cf69-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5cf69-118">Request headers</span></span>
|<span data-ttu-id="5cf69-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5cf69-119">Header</span></span>|<span data-ttu-id="5cf69-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5cf69-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cf69-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cf69-121">Authorization</span></span>|<span data-ttu-id="5cf69-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5cf69-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cf69-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5cf69-123">Accept</span></span>|<span data-ttu-id="5cf69-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5cf69-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cf69-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5cf69-125">Request body</span></span>
<span data-ttu-id="5cf69-126">В тексте запроса добавьте представление объекта androidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cf69-126">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="5cf69-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="5cf69-127">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="5cf69-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cf69-128">Property</span></span>|<span data-ttu-id="5cf69-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5cf69-129">Type</span></span>|<span data-ttu-id="5cf69-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5cf69-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cf69-131">id</span><span class="sxs-lookup"><span data-stu-id="5cf69-131">id</span></span>|<span data-ttu-id="5cf69-132">String</span><span class="sxs-lookup"><span data-stu-id="5cf69-132">String</span></span>|<span data-ttu-id="5cf69-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5cf69-133">Key of the entity.</span></span> <span data-ttu-id="5cf69-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5cf69-135">displayName</span></span>|<span data-ttu-id="5cf69-136">String</span><span class="sxs-lookup"><span data-stu-id="5cf69-136">String</span></span>|<span data-ttu-id="5cf69-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="5cf69-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5cf69-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-139">описание</span><span class="sxs-lookup"><span data-stu-id="5cf69-139">description</span></span>|<span data-ttu-id="5cf69-140">String</span><span class="sxs-lookup"><span data-stu-id="5cf69-140">String</span></span>|<span data-ttu-id="5cf69-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="5cf69-141">The description of the app.</span></span> <span data-ttu-id="5cf69-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-143">publisher</span><span class="sxs-lookup"><span data-stu-id="5cf69-143">publisher</span></span>|<span data-ttu-id="5cf69-144">String</span><span class="sxs-lookup"><span data-stu-id="5cf69-144">String</span></span>|<span data-ttu-id="5cf69-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="5cf69-145">The publisher of the app.</span></span> <span data-ttu-id="5cf69-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5cf69-147">largeIcon</span></span>|[<span data-ttu-id="5cf69-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5cf69-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5cf69-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="5cf69-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5cf69-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5cf69-151">createdDateTime</span></span>|<span data-ttu-id="5cf69-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cf69-152">DateTimeOffset</span></span>|<span data-ttu-id="5cf69-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="5cf69-153">The date and time the app was created.</span></span> <span data-ttu-id="5cf69-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cf69-155">lastModifiedDateTime</span></span>|<span data-ttu-id="5cf69-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cf69-156">DateTimeOffset</span></span>|<span data-ttu-id="5cf69-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="5cf69-157">The date and time the app was last modified.</span></span> <span data-ttu-id="5cf69-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5cf69-159">isFeatured</span></span>|<span data-ttu-id="5cf69-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cf69-160">Boolean</span></span>|<span data-ttu-id="5cf69-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5cf69-162">privacyInformationUrl</span></span>|<span data-ttu-id="5cf69-163">String</span><span class="sxs-lookup"><span data-stu-id="5cf69-163">String</span></span>|<span data-ttu-id="5cf69-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5cf69-164">The privacy statement Url.</span></span> <span data-ttu-id="5cf69-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5cf69-166">informationUrl</span></span>|<span data-ttu-id="5cf69-167">String</span><span class="sxs-lookup"><span data-stu-id="5cf69-167">String</span></span>|<span data-ttu-id="5cf69-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5cf69-168">The more information Url.</span></span> <span data-ttu-id="5cf69-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-170">owner</span><span class="sxs-lookup"><span data-stu-id="5cf69-170">owner</span></span>|<span data-ttu-id="5cf69-171">String</span><span class="sxs-lookup"><span data-stu-id="5cf69-171">String</span></span>|<span data-ttu-id="5cf69-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="5cf69-172">The owner of the app.</span></span> <span data-ttu-id="5cf69-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-174">developer</span><span class="sxs-lookup"><span data-stu-id="5cf69-174">developer</span></span>|<span data-ttu-id="5cf69-175">String</span><span class="sxs-lookup"><span data-stu-id="5cf69-175">String</span></span>|<span data-ttu-id="5cf69-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="5cf69-176">The developer of the app.</span></span> <span data-ttu-id="5cf69-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-178">notes</span><span class="sxs-lookup"><span data-stu-id="5cf69-178">notes</span></span>|<span data-ttu-id="5cf69-179">String</span><span class="sxs-lookup"><span data-stu-id="5cf69-179">String</span></span>|<span data-ttu-id="5cf69-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="5cf69-180">Notes for the app.</span></span> <span data-ttu-id="5cf69-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cf69-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="5cf69-182">publishingState</span></span>|[<span data-ttu-id="5cf69-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5cf69-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5cf69-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="5cf69-184">The publishing state for the app.</span></span> <span data-ttu-id="5cf69-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="5cf69-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5cf69-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5cf69-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5cf69-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5cf69-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5cf69-188">packageId</span><span class="sxs-lookup"><span data-stu-id="5cf69-188">packageId</span></span>|<span data-ttu-id="5cf69-189">String</span><span class="sxs-lookup"><span data-stu-id="5cf69-189">String</span></span>|<span data-ttu-id="5cf69-190">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="5cf69-190">The package identifier.</span></span>|
|<span data-ttu-id="5cf69-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5cf69-191">appStoreUrl</span></span>|<span data-ttu-id="5cf69-192">String</span><span class="sxs-lookup"><span data-stu-id="5cf69-192">String</span></span>|<span data-ttu-id="5cf69-193">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="5cf69-193">The Android app store URL.</span></span>|
|<span data-ttu-id="5cf69-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5cf69-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5cf69-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5cf69-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="5cf69-196">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="5cf69-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="5cf69-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="5cf69-197">Response</span></span>
<span data-ttu-id="5cf69-198">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5cf69-198">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cf69-199">Пример</span><span class="sxs-lookup"><span data-stu-id="5cf69-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="5cf69-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="5cf69-200">Request</span></span>
<span data-ttu-id="5cf69-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5cf69-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="5cf69-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="5cf69-202">Response</span></span>
<span data-ttu-id="5cf69-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5cf69-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



