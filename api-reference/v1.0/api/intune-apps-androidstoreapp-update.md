---
title: Update androidStoreApp
description: Обновление свойств объекта androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 38954ac2ea4aad05e66405aa393e52aba14bb0d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463190"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="2a8c9-103">Update androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="2a8c9-103">Update androidStoreApp</span></span>

<span data-ttu-id="2a8c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a8c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a8c9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a8c9-106">Обновление свойств объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-106">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a8c9-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2a8c9-107">Prerequisites</span></span>
<span data-ttu-id="2a8c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a8c9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a8c9-110">Permission type</span></span>|<span data-ttu-id="2a8c9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a8c9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a8c9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a8c9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a8c9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a8c9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2a8c9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a8c9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a8c9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-115">Not supported.</span></span>|
|<span data-ttu-id="2a8c9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a8c9-116">Application</span></span>|<span data-ttu-id="2a8c9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a8c9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a8c9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="2a8c9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2a8c9-119">Request headers</span></span>
|<span data-ttu-id="2a8c9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a8c9-120">Header</span></span>|<span data-ttu-id="2a8c9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2a8c9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a8c9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a8c9-122">Authorization</span></span>|<span data-ttu-id="2a8c9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a8c9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2a8c9-124">Accept</span></span>|<span data-ttu-id="2a8c9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a8c9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a8c9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a8c9-126">Request body</span></span>
<span data-ttu-id="2a8c9-127">В теле запроса добавьте представление объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-127">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="2a8c9-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-128">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="2a8c9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a8c9-129">Property</span></span>|<span data-ttu-id="2a8c9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2a8c9-130">Type</span></span>|<span data-ttu-id="2a8c9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2a8c9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a8c9-132">id</span><span class="sxs-lookup"><span data-stu-id="2a8c9-132">id</span></span>|<span data-ttu-id="2a8c9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2a8c9-133">String</span></span>|<span data-ttu-id="2a8c9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-134">Key of the entity.</span></span> <span data-ttu-id="2a8c9-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2a8c9-136">displayName</span></span>|<span data-ttu-id="2a8c9-137">Строка</span><span class="sxs-lookup"><span data-stu-id="2a8c9-137">String</span></span>|<span data-ttu-id="2a8c9-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2a8c9-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-140">description</span><span class="sxs-lookup"><span data-stu-id="2a8c9-140">description</span></span>|<span data-ttu-id="2a8c9-141">Строка</span><span class="sxs-lookup"><span data-stu-id="2a8c9-141">String</span></span>|<span data-ttu-id="2a8c9-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-142">The description of the app.</span></span> <span data-ttu-id="2a8c9-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-144">publisher</span><span class="sxs-lookup"><span data-stu-id="2a8c9-144">publisher</span></span>|<span data-ttu-id="2a8c9-145">String</span><span class="sxs-lookup"><span data-stu-id="2a8c9-145">String</span></span>|<span data-ttu-id="2a8c9-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-146">The publisher of the app.</span></span> <span data-ttu-id="2a8c9-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2a8c9-148">largeIcon</span></span>|[<span data-ttu-id="2a8c9-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2a8c9-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2a8c9-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2a8c9-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a8c9-152">createdDateTime</span></span>|<span data-ttu-id="2a8c9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a8c9-153">DateTimeOffset</span></span>|<span data-ttu-id="2a8c9-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-154">The date and time the app was created.</span></span> <span data-ttu-id="2a8c9-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a8c9-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2a8c9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a8c9-157">DateTimeOffset</span></span>|<span data-ttu-id="2a8c9-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2a8c9-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2a8c9-160">isFeatured</span></span>|<span data-ttu-id="2a8c9-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a8c9-161">Boolean</span></span>|<span data-ttu-id="2a8c9-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2a8c9-163">privacyInformationUrl</span></span>|<span data-ttu-id="2a8c9-164">String</span><span class="sxs-lookup"><span data-stu-id="2a8c9-164">String</span></span>|<span data-ttu-id="2a8c9-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-165">The privacy statement Url.</span></span> <span data-ttu-id="2a8c9-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2a8c9-167">informationUrl</span></span>|<span data-ttu-id="2a8c9-168">String</span><span class="sxs-lookup"><span data-stu-id="2a8c9-168">String</span></span>|<span data-ttu-id="2a8c9-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-169">The more information Url.</span></span> <span data-ttu-id="2a8c9-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-171">owner</span><span class="sxs-lookup"><span data-stu-id="2a8c9-171">owner</span></span>|<span data-ttu-id="2a8c9-172">String</span><span class="sxs-lookup"><span data-stu-id="2a8c9-172">String</span></span>|<span data-ttu-id="2a8c9-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-173">The owner of the app.</span></span> <span data-ttu-id="2a8c9-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-175">developer</span><span class="sxs-lookup"><span data-stu-id="2a8c9-175">developer</span></span>|<span data-ttu-id="2a8c9-176">String</span><span class="sxs-lookup"><span data-stu-id="2a8c9-176">String</span></span>|<span data-ttu-id="2a8c9-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-177">The developer of the app.</span></span> <span data-ttu-id="2a8c9-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-179">notes</span><span class="sxs-lookup"><span data-stu-id="2a8c9-179">notes</span></span>|<span data-ttu-id="2a8c9-180">String</span><span class="sxs-lookup"><span data-stu-id="2a8c9-180">String</span></span>|<span data-ttu-id="2a8c9-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-181">Notes for the app.</span></span> <span data-ttu-id="2a8c9-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a8c9-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="2a8c9-183">publishingState</span></span>|[<span data-ttu-id="2a8c9-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="2a8c9-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2a8c9-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-185">The publishing state for the app.</span></span> <span data-ttu-id="2a8c9-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2a8c9-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a8c9-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2a8c9-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2a8c9-189">packageId</span><span class="sxs-lookup"><span data-stu-id="2a8c9-189">packageId</span></span>|<span data-ttu-id="2a8c9-190">String</span><span class="sxs-lookup"><span data-stu-id="2a8c9-190">String</span></span>|<span data-ttu-id="2a8c9-191">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-191">The package identifier.</span></span>|
|<span data-ttu-id="2a8c9-192">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2a8c9-192">appStoreUrl</span></span>|<span data-ttu-id="2a8c9-193">String</span><span class="sxs-lookup"><span data-stu-id="2a8c9-193">String</span></span>|<span data-ttu-id="2a8c9-194">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-194">The Android app store URL.</span></span>|
|<span data-ttu-id="2a8c9-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2a8c9-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2a8c9-196">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2a8c9-196">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="2a8c9-197">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="2a8c9-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a8c9-198">Response</span></span>
<span data-ttu-id="2a8c9-199">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-199">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a8c9-200">Пример</span><span class="sxs-lookup"><span data-stu-id="2a8c9-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a8c9-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a8c9-201">Request</span></span>
<span data-ttu-id="2a8c9-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-202">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2a8c9-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a8c9-203">Response</span></span>
<span data-ttu-id="2a8c9-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a8c9-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






