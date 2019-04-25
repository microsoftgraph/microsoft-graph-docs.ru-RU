---
title: Создание объекта androidStoreApp
description: Создание объекта androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cabceb70911a4de50b26b01ea4856791a747d46
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577520"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="05f01-103">Создание объекта androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="05f01-103">Create androidStoreApp</span></span>

> <span data-ttu-id="05f01-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05f01-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05f01-105">Создание объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-105">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05f01-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="05f01-106">Prerequisites</span></span>
<span data-ttu-id="05f01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05f01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05f01-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05f01-109">Permission type</span></span>|<span data-ttu-id="05f01-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05f01-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05f01-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05f01-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05f01-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05f01-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05f01-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05f01-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05f01-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05f01-114">Not supported.</span></span>|
|<span data-ttu-id="05f01-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05f01-115">Application</span></span>|<span data-ttu-id="05f01-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05f01-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05f01-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05f01-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="05f01-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05f01-118">Request headers</span></span>
|<span data-ttu-id="05f01-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05f01-119">Header</span></span>|<span data-ttu-id="05f01-120">Значение</span><span class="sxs-lookup"><span data-stu-id="05f01-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05f01-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05f01-121">Authorization</span></span>|<span data-ttu-id="05f01-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05f01-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05f01-123">Accept</span><span class="sxs-lookup"><span data-stu-id="05f01-123">Accept</span></span>|<span data-ttu-id="05f01-124">application/json</span><span class="sxs-lookup"><span data-stu-id="05f01-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05f01-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05f01-125">Request body</span></span>
<span data-ttu-id="05f01-126">В тексте запроса добавьте представление объекта androidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05f01-126">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="05f01-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="05f01-127">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="05f01-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="05f01-128">Property</span></span>|<span data-ttu-id="05f01-129">Тип</span><span class="sxs-lookup"><span data-stu-id="05f01-129">Type</span></span>|<span data-ttu-id="05f01-130">Описание</span><span class="sxs-lookup"><span data-stu-id="05f01-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05f01-131">id</span><span class="sxs-lookup"><span data-stu-id="05f01-131">id</span></span>|<span data-ttu-id="05f01-132">Строка</span><span class="sxs-lookup"><span data-stu-id="05f01-132">String</span></span>|<span data-ttu-id="05f01-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="05f01-133">Key of the entity.</span></span> <span data-ttu-id="05f01-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-135">displayName</span><span class="sxs-lookup"><span data-stu-id="05f01-135">displayName</span></span>|<span data-ttu-id="05f01-136">Строка</span><span class="sxs-lookup"><span data-stu-id="05f01-136">String</span></span>|<span data-ttu-id="05f01-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="05f01-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="05f01-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-139">description</span><span class="sxs-lookup"><span data-stu-id="05f01-139">description</span></span>|<span data-ttu-id="05f01-140">String</span><span class="sxs-lookup"><span data-stu-id="05f01-140">String</span></span>|<span data-ttu-id="05f01-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="05f01-141">The description of the app.</span></span> <span data-ttu-id="05f01-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-143">publisher</span><span class="sxs-lookup"><span data-stu-id="05f01-143">publisher</span></span>|<span data-ttu-id="05f01-144">String</span><span class="sxs-lookup"><span data-stu-id="05f01-144">String</span></span>|<span data-ttu-id="05f01-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="05f01-145">The publisher of the app.</span></span> <span data-ttu-id="05f01-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="05f01-147">largeIcon</span></span>|[<span data-ttu-id="05f01-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="05f01-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="05f01-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="05f01-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="05f01-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05f01-151">createdDateTime</span></span>|<span data-ttu-id="05f01-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05f01-152">DateTimeOffset</span></span>|<span data-ttu-id="05f01-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="05f01-153">The date and time the app was created.</span></span> <span data-ttu-id="05f01-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05f01-155">lastModifiedDateTime</span></span>|<span data-ttu-id="05f01-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05f01-156">DateTimeOffset</span></span>|<span data-ttu-id="05f01-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="05f01-157">The date and time the app was last modified.</span></span> <span data-ttu-id="05f01-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="05f01-159">isFeatured</span></span>|<span data-ttu-id="05f01-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="05f01-160">Boolean</span></span>|<span data-ttu-id="05f01-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="05f01-162">privacyInformationUrl</span></span>|<span data-ttu-id="05f01-163">String</span><span class="sxs-lookup"><span data-stu-id="05f01-163">String</span></span>|<span data-ttu-id="05f01-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="05f01-164">The privacy statement Url.</span></span> <span data-ttu-id="05f01-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="05f01-166">informationUrl</span></span>|<span data-ttu-id="05f01-167">String</span><span class="sxs-lookup"><span data-stu-id="05f01-167">String</span></span>|<span data-ttu-id="05f01-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="05f01-168">The more information Url.</span></span> <span data-ttu-id="05f01-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-170">owner</span><span class="sxs-lookup"><span data-stu-id="05f01-170">owner</span></span>|<span data-ttu-id="05f01-171">String</span><span class="sxs-lookup"><span data-stu-id="05f01-171">String</span></span>|<span data-ttu-id="05f01-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="05f01-172">The owner of the app.</span></span> <span data-ttu-id="05f01-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-174">developer</span><span class="sxs-lookup"><span data-stu-id="05f01-174">developer</span></span>|<span data-ttu-id="05f01-175">String</span><span class="sxs-lookup"><span data-stu-id="05f01-175">String</span></span>|<span data-ttu-id="05f01-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="05f01-176">The developer of the app.</span></span> <span data-ttu-id="05f01-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-178">notes</span><span class="sxs-lookup"><span data-stu-id="05f01-178">notes</span></span>|<span data-ttu-id="05f01-179">String</span><span class="sxs-lookup"><span data-stu-id="05f01-179">String</span></span>|<span data-ttu-id="05f01-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="05f01-180">Notes for the app.</span></span> <span data-ttu-id="05f01-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="05f01-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="05f01-182">publishingState</span></span>|[<span data-ttu-id="05f01-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="05f01-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="05f01-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="05f01-184">The publishing state for the app.</span></span> <span data-ttu-id="05f01-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="05f01-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="05f01-186">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="05f01-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="05f01-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="05f01-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="05f01-188">packageId</span><span class="sxs-lookup"><span data-stu-id="05f01-188">packageId</span></span>|<span data-ttu-id="05f01-189">String</span><span class="sxs-lookup"><span data-stu-id="05f01-189">String</span></span>|<span data-ttu-id="05f01-190">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="05f01-190">The package identifier.</span></span>|
|<span data-ttu-id="05f01-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="05f01-191">appStoreUrl</span></span>|<span data-ttu-id="05f01-192">String</span><span class="sxs-lookup"><span data-stu-id="05f01-192">String</span></span>|<span data-ttu-id="05f01-193">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="05f01-193">The Android app store URL.</span></span>|
|<span data-ttu-id="05f01-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="05f01-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="05f01-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="05f01-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="05f01-196">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="05f01-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="05f01-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="05f01-197">Response</span></span>
<span data-ttu-id="05f01-198">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="05f01-198">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05f01-199">Пример</span><span class="sxs-lookup"><span data-stu-id="05f01-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="05f01-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="05f01-200">Request</span></span>
<span data-ttu-id="05f01-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05f01-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05f01-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="05f01-202">Response</span></span>
<span data-ttu-id="05f01-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05f01-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



