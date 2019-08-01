---
title: Update androidStoreApp
description: Обновление свойств объекта androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 76ae9d4b1bcf06bde926ecebeadb7095f4bfd8df
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014293"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="77cb5-103">Update androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="77cb5-103">Update androidStoreApp</span></span>

> <span data-ttu-id="77cb5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77cb5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77cb5-105">Обновление свойств объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-105">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77cb5-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="77cb5-106">Prerequisites</span></span>
<span data-ttu-id="77cb5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77cb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77cb5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77cb5-109">Permission type</span></span>|<span data-ttu-id="77cb5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77cb5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77cb5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77cb5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="77cb5-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77cb5-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="77cb5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77cb5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77cb5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77cb5-114">Not supported.</span></span>|
|<span data-ttu-id="77cb5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77cb5-115">Application</span></span>|<span data-ttu-id="77cb5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77cb5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77cb5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77cb5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="77cb5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77cb5-118">Request headers</span></span>
|<span data-ttu-id="77cb5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77cb5-119">Header</span></span>|<span data-ttu-id="77cb5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="77cb5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77cb5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77cb5-121">Authorization</span></span>|<span data-ttu-id="77cb5-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77cb5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77cb5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="77cb5-123">Accept</span></span>|<span data-ttu-id="77cb5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="77cb5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77cb5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="77cb5-125">Request body</span></span>
<span data-ttu-id="77cb5-126">В теле запроса добавьте представление объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77cb5-126">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="77cb5-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-127">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="77cb5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="77cb5-128">Property</span></span>|<span data-ttu-id="77cb5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="77cb5-129">Type</span></span>|<span data-ttu-id="77cb5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="77cb5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77cb5-131">id</span><span class="sxs-lookup"><span data-stu-id="77cb5-131">id</span></span>|<span data-ttu-id="77cb5-132">Строка</span><span class="sxs-lookup"><span data-stu-id="77cb5-132">String</span></span>|<span data-ttu-id="77cb5-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="77cb5-133">Key of the entity.</span></span> <span data-ttu-id="77cb5-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="77cb5-135">displayName</span></span>|<span data-ttu-id="77cb5-136">Строка</span><span class="sxs-lookup"><span data-stu-id="77cb5-136">String</span></span>|<span data-ttu-id="77cb5-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="77cb5-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="77cb5-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-139">description</span><span class="sxs-lookup"><span data-stu-id="77cb5-139">description</span></span>|<span data-ttu-id="77cb5-140">Строка</span><span class="sxs-lookup"><span data-stu-id="77cb5-140">String</span></span>|<span data-ttu-id="77cb5-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="77cb5-141">The description of the app.</span></span> <span data-ttu-id="77cb5-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-143">publisher</span><span class="sxs-lookup"><span data-stu-id="77cb5-143">publisher</span></span>|<span data-ttu-id="77cb5-144">String</span><span class="sxs-lookup"><span data-stu-id="77cb5-144">String</span></span>|<span data-ttu-id="77cb5-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="77cb5-145">The publisher of the app.</span></span> <span data-ttu-id="77cb5-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="77cb5-147">largeIcon</span></span>|[<span data-ttu-id="77cb5-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="77cb5-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="77cb5-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="77cb5-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="77cb5-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77cb5-151">createdDateTime</span></span>|<span data-ttu-id="77cb5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77cb5-152">DateTimeOffset</span></span>|<span data-ttu-id="77cb5-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="77cb5-153">The date and time the app was created.</span></span> <span data-ttu-id="77cb5-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77cb5-155">lastModifiedDateTime</span></span>|<span data-ttu-id="77cb5-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77cb5-156">DateTimeOffset</span></span>|<span data-ttu-id="77cb5-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="77cb5-157">The date and time the app was last modified.</span></span> <span data-ttu-id="77cb5-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="77cb5-159">isFeatured</span></span>|<span data-ttu-id="77cb5-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="77cb5-160">Boolean</span></span>|<span data-ttu-id="77cb5-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="77cb5-162">privacyInformationUrl</span></span>|<span data-ttu-id="77cb5-163">String</span><span class="sxs-lookup"><span data-stu-id="77cb5-163">String</span></span>|<span data-ttu-id="77cb5-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="77cb5-164">The privacy statement Url.</span></span> <span data-ttu-id="77cb5-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="77cb5-166">informationUrl</span></span>|<span data-ttu-id="77cb5-167">String</span><span class="sxs-lookup"><span data-stu-id="77cb5-167">String</span></span>|<span data-ttu-id="77cb5-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="77cb5-168">The more information Url.</span></span> <span data-ttu-id="77cb5-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-170">owner</span><span class="sxs-lookup"><span data-stu-id="77cb5-170">owner</span></span>|<span data-ttu-id="77cb5-171">String</span><span class="sxs-lookup"><span data-stu-id="77cb5-171">String</span></span>|<span data-ttu-id="77cb5-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="77cb5-172">The owner of the app.</span></span> <span data-ttu-id="77cb5-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-174">developer</span><span class="sxs-lookup"><span data-stu-id="77cb5-174">developer</span></span>|<span data-ttu-id="77cb5-175">String</span><span class="sxs-lookup"><span data-stu-id="77cb5-175">String</span></span>|<span data-ttu-id="77cb5-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="77cb5-176">The developer of the app.</span></span> <span data-ttu-id="77cb5-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-178">notes</span><span class="sxs-lookup"><span data-stu-id="77cb5-178">notes</span></span>|<span data-ttu-id="77cb5-179">String</span><span class="sxs-lookup"><span data-stu-id="77cb5-179">String</span></span>|<span data-ttu-id="77cb5-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="77cb5-180">Notes for the app.</span></span> <span data-ttu-id="77cb5-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77cb5-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="77cb5-182">publishingState</span></span>|[<span data-ttu-id="77cb5-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="77cb5-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="77cb5-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="77cb5-184">The publishing state for the app.</span></span> <span data-ttu-id="77cb5-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="77cb5-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="77cb5-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="77cb5-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="77cb5-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="77cb5-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="77cb5-188">packageId</span><span class="sxs-lookup"><span data-stu-id="77cb5-188">packageId</span></span>|<span data-ttu-id="77cb5-189">String</span><span class="sxs-lookup"><span data-stu-id="77cb5-189">String</span></span>|<span data-ttu-id="77cb5-190">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="77cb5-190">The package identifier.</span></span>|
|<span data-ttu-id="77cb5-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="77cb5-191">appStoreUrl</span></span>|<span data-ttu-id="77cb5-192">String</span><span class="sxs-lookup"><span data-stu-id="77cb5-192">String</span></span>|<span data-ttu-id="77cb5-193">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="77cb5-193">The Android app store URL.</span></span>|
|<span data-ttu-id="77cb5-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="77cb5-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="77cb5-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="77cb5-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="77cb5-196">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="77cb5-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="77cb5-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="77cb5-197">Response</span></span>
<span data-ttu-id="77cb5-198">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="77cb5-198">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77cb5-199">Пример</span><span class="sxs-lookup"><span data-stu-id="77cb5-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="77cb5-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="77cb5-200">Request</span></span>
<span data-ttu-id="77cb5-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77cb5-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="77cb5-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="77cb5-202">Response</span></span>
<span data-ttu-id="77cb5-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77cb5-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



