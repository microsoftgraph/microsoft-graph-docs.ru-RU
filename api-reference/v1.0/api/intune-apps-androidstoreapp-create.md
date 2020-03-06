---
title: Создание объекта androidStoreApp
description: Создание объекта androidStoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b9c1516f6c3dd5ae0e52982e00bcdf1194f019d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516660"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="11249-103">Создание объекта androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="11249-103">Create androidStoreApp</span></span>

<span data-ttu-id="11249-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11249-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11249-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11249-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11249-106">Создание объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-106">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11249-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="11249-107">Prerequisites</span></span>
<span data-ttu-id="11249-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11249-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11249-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11249-110">Permission type</span></span>|<span data-ttu-id="11249-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11249-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11249-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11249-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11249-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11249-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="11249-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11249-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11249-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11249-115">Not supported.</span></span>|
|<span data-ttu-id="11249-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11249-116">Application</span></span>|<span data-ttu-id="11249-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11249-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11249-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11249-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="11249-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="11249-119">Request headers</span></span>
|<span data-ttu-id="11249-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11249-120">Header</span></span>|<span data-ttu-id="11249-121">Значение</span><span class="sxs-lookup"><span data-stu-id="11249-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11249-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11249-122">Authorization</span></span>|<span data-ttu-id="11249-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11249-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11249-124">Accept</span><span class="sxs-lookup"><span data-stu-id="11249-124">Accept</span></span>|<span data-ttu-id="11249-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11249-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11249-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11249-126">Request body</span></span>
<span data-ttu-id="11249-127">В тексте запроса добавьте представление объекта androidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11249-127">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="11249-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="11249-128">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="11249-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="11249-129">Property</span></span>|<span data-ttu-id="11249-130">Тип</span><span class="sxs-lookup"><span data-stu-id="11249-130">Type</span></span>|<span data-ttu-id="11249-131">Описание</span><span class="sxs-lookup"><span data-stu-id="11249-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11249-132">id</span><span class="sxs-lookup"><span data-stu-id="11249-132">id</span></span>|<span data-ttu-id="11249-133">Строка</span><span class="sxs-lookup"><span data-stu-id="11249-133">String</span></span>|<span data-ttu-id="11249-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="11249-134">Key of the entity.</span></span> <span data-ttu-id="11249-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-136">displayName</span><span class="sxs-lookup"><span data-stu-id="11249-136">displayName</span></span>|<span data-ttu-id="11249-137">Строка</span><span class="sxs-lookup"><span data-stu-id="11249-137">String</span></span>|<span data-ttu-id="11249-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="11249-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="11249-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-140">description</span><span class="sxs-lookup"><span data-stu-id="11249-140">description</span></span>|<span data-ttu-id="11249-141">Строка</span><span class="sxs-lookup"><span data-stu-id="11249-141">String</span></span>|<span data-ttu-id="11249-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="11249-142">The description of the app.</span></span> <span data-ttu-id="11249-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-144">publisher</span><span class="sxs-lookup"><span data-stu-id="11249-144">publisher</span></span>|<span data-ttu-id="11249-145">Строка</span><span class="sxs-lookup"><span data-stu-id="11249-145">String</span></span>|<span data-ttu-id="11249-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="11249-146">The publisher of the app.</span></span> <span data-ttu-id="11249-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="11249-148">largeIcon</span></span>|[<span data-ttu-id="11249-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="11249-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="11249-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="11249-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="11249-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11249-152">createdDateTime</span></span>|<span data-ttu-id="11249-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11249-153">DateTimeOffset</span></span>|<span data-ttu-id="11249-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="11249-154">The date and time the app was created.</span></span> <span data-ttu-id="11249-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11249-156">lastModifiedDateTime</span></span>|<span data-ttu-id="11249-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11249-157">DateTimeOffset</span></span>|<span data-ttu-id="11249-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="11249-158">The date and time the app was last modified.</span></span> <span data-ttu-id="11249-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="11249-160">isFeatured</span></span>|<span data-ttu-id="11249-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="11249-161">Boolean</span></span>|<span data-ttu-id="11249-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="11249-163">privacyInformationUrl</span></span>|<span data-ttu-id="11249-164">Строка</span><span class="sxs-lookup"><span data-stu-id="11249-164">String</span></span>|<span data-ttu-id="11249-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="11249-165">The privacy statement Url.</span></span> <span data-ttu-id="11249-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="11249-167">informationUrl</span></span>|<span data-ttu-id="11249-168">Строка</span><span class="sxs-lookup"><span data-stu-id="11249-168">String</span></span>|<span data-ttu-id="11249-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="11249-169">The more information Url.</span></span> <span data-ttu-id="11249-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-171">owner</span><span class="sxs-lookup"><span data-stu-id="11249-171">owner</span></span>|<span data-ttu-id="11249-172">String</span><span class="sxs-lookup"><span data-stu-id="11249-172">String</span></span>|<span data-ttu-id="11249-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="11249-173">The owner of the app.</span></span> <span data-ttu-id="11249-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-175">developer</span><span class="sxs-lookup"><span data-stu-id="11249-175">developer</span></span>|<span data-ttu-id="11249-176">Строка</span><span class="sxs-lookup"><span data-stu-id="11249-176">String</span></span>|<span data-ttu-id="11249-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="11249-177">The developer of the app.</span></span> <span data-ttu-id="11249-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-179">notes</span><span class="sxs-lookup"><span data-stu-id="11249-179">notes</span></span>|<span data-ttu-id="11249-180">Строка</span><span class="sxs-lookup"><span data-stu-id="11249-180">String</span></span>|<span data-ttu-id="11249-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="11249-181">Notes for the app.</span></span> <span data-ttu-id="11249-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11249-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="11249-183">publishingState</span></span>|[<span data-ttu-id="11249-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="11249-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="11249-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="11249-185">The publishing state for the app.</span></span> <span data-ttu-id="11249-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="11249-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="11249-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11249-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="11249-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="11249-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="11249-189">packageId</span><span class="sxs-lookup"><span data-stu-id="11249-189">packageId</span></span>|<span data-ttu-id="11249-190">Строка</span><span class="sxs-lookup"><span data-stu-id="11249-190">String</span></span>|<span data-ttu-id="11249-191">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="11249-191">The package identifier.</span></span>|
|<span data-ttu-id="11249-192">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="11249-192">appStoreUrl</span></span>|<span data-ttu-id="11249-193">String</span><span class="sxs-lookup"><span data-stu-id="11249-193">String</span></span>|<span data-ttu-id="11249-194">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="11249-194">The Android app store URL.</span></span>|
|<span data-ttu-id="11249-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="11249-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="11249-196">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="11249-196">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="11249-197">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="11249-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="11249-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="11249-198">Response</span></span>
<span data-ttu-id="11249-199">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="11249-199">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11249-200">Пример</span><span class="sxs-lookup"><span data-stu-id="11249-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="11249-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="11249-201">Request</span></span>
<span data-ttu-id="11249-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11249-202">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11249-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="11249-203">Response</span></span>
<span data-ttu-id="11249-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11249-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




