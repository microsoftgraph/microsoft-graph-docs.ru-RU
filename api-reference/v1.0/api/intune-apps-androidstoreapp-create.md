---
title: Создание объекта androidStoreApp
description: Создание объекта androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 402d046204573e531b9934cc389fd103c0aabd52
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446556"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="4c5e2-103">Создание объекта androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="4c5e2-103">Create androidStoreApp</span></span>

<span data-ttu-id="4c5e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c5e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c5e2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c5e2-106">Создание объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-106">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c5e2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4c5e2-107">Prerequisites</span></span>
<span data-ttu-id="4c5e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c5e2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c5e2-110">Permission type</span></span>|<span data-ttu-id="4c5e2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c5e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c5e2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c5e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c5e2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c5e2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c5e2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c5e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c5e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-115">Not supported.</span></span>|
|<span data-ttu-id="4c5e2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c5e2-116">Application</span></span>|<span data-ttu-id="4c5e2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c5e2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c5e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4c5e2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4c5e2-119">Request headers</span></span>
|<span data-ttu-id="4c5e2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c5e2-120">Header</span></span>|<span data-ttu-id="4c5e2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4c5e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c5e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c5e2-122">Authorization</span></span>|<span data-ttu-id="4c5e2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c5e2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4c5e2-124">Accept</span></span>|<span data-ttu-id="4c5e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c5e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c5e2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c5e2-126">Request body</span></span>
<span data-ttu-id="4c5e2-127">В тексте запроса добавьте представление объекта androidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-127">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="4c5e2-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-128">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="4c5e2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c5e2-129">Property</span></span>|<span data-ttu-id="4c5e2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4c5e2-130">Type</span></span>|<span data-ttu-id="4c5e2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4c5e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c5e2-132">id</span><span class="sxs-lookup"><span data-stu-id="4c5e2-132">id</span></span>|<span data-ttu-id="4c5e2-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4c5e2-133">String</span></span>|<span data-ttu-id="4c5e2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-134">Key of the entity.</span></span> <span data-ttu-id="4c5e2-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4c5e2-136">displayName</span></span>|<span data-ttu-id="4c5e2-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4c5e2-137">String</span></span>|<span data-ttu-id="4c5e2-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4c5e2-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-140">description</span><span class="sxs-lookup"><span data-stu-id="4c5e2-140">description</span></span>|<span data-ttu-id="4c5e2-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4c5e2-141">String</span></span>|<span data-ttu-id="4c5e2-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-142">The description of the app.</span></span> <span data-ttu-id="4c5e2-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4c5e2-144">publisher</span></span>|<span data-ttu-id="4c5e2-145">String</span><span class="sxs-lookup"><span data-stu-id="4c5e2-145">String</span></span>|<span data-ttu-id="4c5e2-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-146">The publisher of the app.</span></span> <span data-ttu-id="4c5e2-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4c5e2-148">largeIcon</span></span>|[<span data-ttu-id="4c5e2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4c5e2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4c5e2-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4c5e2-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c5e2-152">createdDateTime</span></span>|<span data-ttu-id="4c5e2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c5e2-153">DateTimeOffset</span></span>|<span data-ttu-id="4c5e2-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-154">The date and time the app was created.</span></span> <span data-ttu-id="4c5e2-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c5e2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4c5e2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c5e2-157">DateTimeOffset</span></span>|<span data-ttu-id="4c5e2-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4c5e2-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4c5e2-160">isFeatured</span></span>|<span data-ttu-id="4c5e2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c5e2-161">Boolean</span></span>|<span data-ttu-id="4c5e2-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4c5e2-163">privacyInformationUrl</span></span>|<span data-ttu-id="4c5e2-164">String</span><span class="sxs-lookup"><span data-stu-id="4c5e2-164">String</span></span>|<span data-ttu-id="4c5e2-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-165">The privacy statement Url.</span></span> <span data-ttu-id="4c5e2-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4c5e2-167">informationUrl</span></span>|<span data-ttu-id="4c5e2-168">String</span><span class="sxs-lookup"><span data-stu-id="4c5e2-168">String</span></span>|<span data-ttu-id="4c5e2-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-169">The more information Url.</span></span> <span data-ttu-id="4c5e2-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-171">owner</span><span class="sxs-lookup"><span data-stu-id="4c5e2-171">owner</span></span>|<span data-ttu-id="4c5e2-172">String</span><span class="sxs-lookup"><span data-stu-id="4c5e2-172">String</span></span>|<span data-ttu-id="4c5e2-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-173">The owner of the app.</span></span> <span data-ttu-id="4c5e2-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-175">developer</span><span class="sxs-lookup"><span data-stu-id="4c5e2-175">developer</span></span>|<span data-ttu-id="4c5e2-176">String</span><span class="sxs-lookup"><span data-stu-id="4c5e2-176">String</span></span>|<span data-ttu-id="4c5e2-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-177">The developer of the app.</span></span> <span data-ttu-id="4c5e2-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-179">notes</span><span class="sxs-lookup"><span data-stu-id="4c5e2-179">notes</span></span>|<span data-ttu-id="4c5e2-180">String</span><span class="sxs-lookup"><span data-stu-id="4c5e2-180">String</span></span>|<span data-ttu-id="4c5e2-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-181">Notes for the app.</span></span> <span data-ttu-id="4c5e2-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c5e2-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="4c5e2-183">publishingState</span></span>|[<span data-ttu-id="4c5e2-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="4c5e2-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4c5e2-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-185">The publishing state for the app.</span></span> <span data-ttu-id="4c5e2-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4c5e2-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c5e2-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4c5e2-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4c5e2-189">packageId</span><span class="sxs-lookup"><span data-stu-id="4c5e2-189">packageId</span></span>|<span data-ttu-id="4c5e2-190">String</span><span class="sxs-lookup"><span data-stu-id="4c5e2-190">String</span></span>|<span data-ttu-id="4c5e2-191">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-191">The package identifier.</span></span>|
|<span data-ttu-id="4c5e2-192">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4c5e2-192">appStoreUrl</span></span>|<span data-ttu-id="4c5e2-193">String</span><span class="sxs-lookup"><span data-stu-id="4c5e2-193">String</span></span>|<span data-ttu-id="4c5e2-194">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-194">The Android app store URL.</span></span>|
|<span data-ttu-id="4c5e2-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4c5e2-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4c5e2-196">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4c5e2-196">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="4c5e2-197">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="4c5e2-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c5e2-198">Response</span></span>
<span data-ttu-id="4c5e2-199">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-199">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c5e2-200">Пример</span><span class="sxs-lookup"><span data-stu-id="4c5e2-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c5e2-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c5e2-201">Request</span></span>
<span data-ttu-id="4c5e2-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-202">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c5e2-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c5e2-203">Response</span></span>
<span data-ttu-id="4c5e2-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c5e2-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






