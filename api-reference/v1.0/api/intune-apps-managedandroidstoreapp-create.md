---
title: Create managedAndroidStoreApp
description: Создание нового объекта managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8104dbc8259352d917f8b05761d06aa3f3dea805
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754310"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="667a7-103">Create managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="667a7-103">Create managedAndroidStoreApp</span></span>

<span data-ttu-id="667a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="667a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="667a7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="667a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="667a7-106">Создание нового объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-106">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="667a7-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="667a7-107">Prerequisites</span></span>
<span data-ttu-id="667a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="667a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="667a7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="667a7-110">Permission type</span></span>|<span data-ttu-id="667a7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="667a7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="667a7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="667a7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="667a7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="667a7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="667a7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="667a7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="667a7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="667a7-115">Not supported.</span></span>|
|<span data-ttu-id="667a7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="667a7-116">Application</span></span>|<span data-ttu-id="667a7-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="667a7-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="667a7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="667a7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="667a7-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="667a7-119">Request headers</span></span>
|<span data-ttu-id="667a7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="667a7-120">Header</span></span>|<span data-ttu-id="667a7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="667a7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="667a7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="667a7-122">Authorization</span></span>|<span data-ttu-id="667a7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="667a7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="667a7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="667a7-124">Accept</span></span>|<span data-ttu-id="667a7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="667a7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="667a7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="667a7-126">Request body</span></span>
<span data-ttu-id="667a7-127">В теле запроса добавьте представление объекта managedAndroidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="667a7-127">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="667a7-128">Ниже показаны свойства, которые необходимо указывать при создании объекта managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="667a7-128">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="667a7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="667a7-129">Property</span></span>|<span data-ttu-id="667a7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="667a7-130">Type</span></span>|<span data-ttu-id="667a7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="667a7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="667a7-132">id</span><span class="sxs-lookup"><span data-stu-id="667a7-132">id</span></span>|<span data-ttu-id="667a7-133">String</span><span class="sxs-lookup"><span data-stu-id="667a7-133">String</span></span>|<span data-ttu-id="667a7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="667a7-134">Key of the entity.</span></span> <span data-ttu-id="667a7-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="667a7-136">displayName</span></span>|<span data-ttu-id="667a7-137">String</span><span class="sxs-lookup"><span data-stu-id="667a7-137">String</span></span>|<span data-ttu-id="667a7-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="667a7-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="667a7-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-140">description</span><span class="sxs-lookup"><span data-stu-id="667a7-140">description</span></span>|<span data-ttu-id="667a7-141">String</span><span class="sxs-lookup"><span data-stu-id="667a7-141">String</span></span>|<span data-ttu-id="667a7-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="667a7-142">The description of the app.</span></span> <span data-ttu-id="667a7-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-144">publisher</span><span class="sxs-lookup"><span data-stu-id="667a7-144">publisher</span></span>|<span data-ttu-id="667a7-145">String</span><span class="sxs-lookup"><span data-stu-id="667a7-145">String</span></span>|<span data-ttu-id="667a7-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="667a7-146">The publisher of the app.</span></span> <span data-ttu-id="667a7-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="667a7-148">largeIcon</span></span>|[<span data-ttu-id="667a7-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="667a7-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="667a7-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="667a7-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="667a7-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="667a7-152">createdDateTime</span></span>|<span data-ttu-id="667a7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="667a7-153">DateTimeOffset</span></span>|<span data-ttu-id="667a7-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="667a7-154">The date and time the app was created.</span></span> <span data-ttu-id="667a7-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="667a7-156">lastModifiedDateTime</span></span>|<span data-ttu-id="667a7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="667a7-157">DateTimeOffset</span></span>|<span data-ttu-id="667a7-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="667a7-158">The date and time the app was last modified.</span></span> <span data-ttu-id="667a7-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="667a7-160">isFeatured</span></span>|<span data-ttu-id="667a7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="667a7-161">Boolean</span></span>|<span data-ttu-id="667a7-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="667a7-163">privacyInformationUrl</span></span>|<span data-ttu-id="667a7-164">String</span><span class="sxs-lookup"><span data-stu-id="667a7-164">String</span></span>|<span data-ttu-id="667a7-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="667a7-165">The privacy statement Url.</span></span> <span data-ttu-id="667a7-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="667a7-167">informationUrl</span></span>|<span data-ttu-id="667a7-168">String</span><span class="sxs-lookup"><span data-stu-id="667a7-168">String</span></span>|<span data-ttu-id="667a7-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="667a7-169">The more information Url.</span></span> <span data-ttu-id="667a7-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-171">owner</span><span class="sxs-lookup"><span data-stu-id="667a7-171">owner</span></span>|<span data-ttu-id="667a7-172">String</span><span class="sxs-lookup"><span data-stu-id="667a7-172">String</span></span>|<span data-ttu-id="667a7-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="667a7-173">The owner of the app.</span></span> <span data-ttu-id="667a7-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-175">developer</span><span class="sxs-lookup"><span data-stu-id="667a7-175">developer</span></span>|<span data-ttu-id="667a7-176">String</span><span class="sxs-lookup"><span data-stu-id="667a7-176">String</span></span>|<span data-ttu-id="667a7-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="667a7-177">The developer of the app.</span></span> <span data-ttu-id="667a7-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-179">notes</span><span class="sxs-lookup"><span data-stu-id="667a7-179">notes</span></span>|<span data-ttu-id="667a7-180">String</span><span class="sxs-lookup"><span data-stu-id="667a7-180">String</span></span>|<span data-ttu-id="667a7-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="667a7-181">Notes for the app.</span></span> <span data-ttu-id="667a7-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="667a7-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="667a7-183">publishingState</span></span>|[<span data-ttu-id="667a7-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="667a7-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="667a7-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="667a7-185">The publishing state for the app.</span></span> <span data-ttu-id="667a7-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="667a7-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="667a7-187">Унаследованный от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="667a7-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="667a7-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="667a7-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="667a7-189">appAvailability</span></span>|[<span data-ttu-id="667a7-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="667a7-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="667a7-191">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="667a7-191">The Application's availability.</span></span> <span data-ttu-id="667a7-192">Унаследованный от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="667a7-193">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="667a7-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="667a7-194">version</span><span class="sxs-lookup"><span data-stu-id="667a7-194">version</span></span>|<span data-ttu-id="667a7-195">String</span><span class="sxs-lookup"><span data-stu-id="667a7-195">String</span></span>|<span data-ttu-id="667a7-196">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="667a7-196">The Application's version.</span></span> <span data-ttu-id="667a7-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="667a7-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="667a7-198">packageId</span><span class="sxs-lookup"><span data-stu-id="667a7-198">packageId</span></span>|<span data-ttu-id="667a7-199">String</span><span class="sxs-lookup"><span data-stu-id="667a7-199">String</span></span>|<span data-ttu-id="667a7-200">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="667a7-200">The app's package ID.</span></span>|
|<span data-ttu-id="667a7-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="667a7-201">appStoreUrl</span></span>|<span data-ttu-id="667a7-202">String</span><span class="sxs-lookup"><span data-stu-id="667a7-202">String</span></span>|<span data-ttu-id="667a7-203">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="667a7-203">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="667a7-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="667a7-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="667a7-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="667a7-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="667a7-206">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="667a7-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="667a7-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="667a7-207">Response</span></span>
<span data-ttu-id="667a7-208">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="667a7-208">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="667a7-209">Пример</span><span class="sxs-lookup"><span data-stu-id="667a7-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="667a7-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="667a7-210">Request</span></span>
<span data-ttu-id="667a7-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="667a7-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1056

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="667a7-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="667a7-212">Response</span></span>
<span data-ttu-id="667a7-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="667a7-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1228

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  }
}
```




