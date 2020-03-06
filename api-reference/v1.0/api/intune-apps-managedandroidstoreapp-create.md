---
title: Create managedAndroidStoreApp
description: Создание нового объекта managedAndroidStoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 268e657857734be9fc8a137c3c50de7b2dc6dd35
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516414"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="670f2-103">Create managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="670f2-103">Create managedAndroidStoreApp</span></span>

<span data-ttu-id="670f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="670f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="670f2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="670f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="670f2-106">Создание нового объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-106">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="670f2-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="670f2-107">Prerequisites</span></span>
<span data-ttu-id="670f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="670f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="670f2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="670f2-110">Permission type</span></span>|<span data-ttu-id="670f2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="670f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="670f2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="670f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="670f2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="670f2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="670f2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="670f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="670f2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="670f2-115">Not supported.</span></span>|
|<span data-ttu-id="670f2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="670f2-116">Application</span></span>|<span data-ttu-id="670f2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="670f2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="670f2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="670f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="670f2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="670f2-119">Request headers</span></span>
|<span data-ttu-id="670f2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="670f2-120">Header</span></span>|<span data-ttu-id="670f2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="670f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="670f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="670f2-122">Authorization</span></span>|<span data-ttu-id="670f2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="670f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="670f2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="670f2-124">Accept</span></span>|<span data-ttu-id="670f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="670f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="670f2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="670f2-126">Request body</span></span>
<span data-ttu-id="670f2-127">В теле запроса добавьте представление объекта managedAndroidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="670f2-127">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="670f2-128">Ниже показаны свойства, которые необходимо указывать при создании объекта managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="670f2-128">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="670f2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="670f2-129">Property</span></span>|<span data-ttu-id="670f2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="670f2-130">Type</span></span>|<span data-ttu-id="670f2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="670f2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="670f2-132">id</span><span class="sxs-lookup"><span data-stu-id="670f2-132">id</span></span>|<span data-ttu-id="670f2-133">Строка</span><span class="sxs-lookup"><span data-stu-id="670f2-133">String</span></span>|<span data-ttu-id="670f2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="670f2-134">Key of the entity.</span></span> <span data-ttu-id="670f2-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="670f2-136">displayName</span></span>|<span data-ttu-id="670f2-137">Строка</span><span class="sxs-lookup"><span data-stu-id="670f2-137">String</span></span>|<span data-ttu-id="670f2-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="670f2-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="670f2-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-140">description</span><span class="sxs-lookup"><span data-stu-id="670f2-140">description</span></span>|<span data-ttu-id="670f2-141">Строка</span><span class="sxs-lookup"><span data-stu-id="670f2-141">String</span></span>|<span data-ttu-id="670f2-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="670f2-142">The description of the app.</span></span> <span data-ttu-id="670f2-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-144">publisher</span><span class="sxs-lookup"><span data-stu-id="670f2-144">publisher</span></span>|<span data-ttu-id="670f2-145">Строка</span><span class="sxs-lookup"><span data-stu-id="670f2-145">String</span></span>|<span data-ttu-id="670f2-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="670f2-146">The publisher of the app.</span></span> <span data-ttu-id="670f2-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="670f2-148">largeIcon</span></span>|[<span data-ttu-id="670f2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="670f2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="670f2-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="670f2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="670f2-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="670f2-152">createdDateTime</span></span>|<span data-ttu-id="670f2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="670f2-153">DateTimeOffset</span></span>|<span data-ttu-id="670f2-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="670f2-154">The date and time the app was created.</span></span> <span data-ttu-id="670f2-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="670f2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="670f2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="670f2-157">DateTimeOffset</span></span>|<span data-ttu-id="670f2-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="670f2-158">The date and time the app was last modified.</span></span> <span data-ttu-id="670f2-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="670f2-160">isFeatured</span></span>|<span data-ttu-id="670f2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="670f2-161">Boolean</span></span>|<span data-ttu-id="670f2-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="670f2-163">privacyInformationUrl</span></span>|<span data-ttu-id="670f2-164">Строка</span><span class="sxs-lookup"><span data-stu-id="670f2-164">String</span></span>|<span data-ttu-id="670f2-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="670f2-165">The privacy statement Url.</span></span> <span data-ttu-id="670f2-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="670f2-167">informationUrl</span></span>|<span data-ttu-id="670f2-168">Строка</span><span class="sxs-lookup"><span data-stu-id="670f2-168">String</span></span>|<span data-ttu-id="670f2-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="670f2-169">The more information Url.</span></span> <span data-ttu-id="670f2-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-171">owner</span><span class="sxs-lookup"><span data-stu-id="670f2-171">owner</span></span>|<span data-ttu-id="670f2-172">String</span><span class="sxs-lookup"><span data-stu-id="670f2-172">String</span></span>|<span data-ttu-id="670f2-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="670f2-173">The owner of the app.</span></span> <span data-ttu-id="670f2-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-175">developer</span><span class="sxs-lookup"><span data-stu-id="670f2-175">developer</span></span>|<span data-ttu-id="670f2-176">Строка</span><span class="sxs-lookup"><span data-stu-id="670f2-176">String</span></span>|<span data-ttu-id="670f2-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="670f2-177">The developer of the app.</span></span> <span data-ttu-id="670f2-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-179">notes</span><span class="sxs-lookup"><span data-stu-id="670f2-179">notes</span></span>|<span data-ttu-id="670f2-180">Строка</span><span class="sxs-lookup"><span data-stu-id="670f2-180">String</span></span>|<span data-ttu-id="670f2-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="670f2-181">Notes for the app.</span></span> <span data-ttu-id="670f2-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="670f2-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="670f2-183">publishingState</span></span>|[<span data-ttu-id="670f2-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="670f2-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="670f2-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="670f2-185">The publishing state for the app.</span></span> <span data-ttu-id="670f2-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="670f2-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="670f2-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="670f2-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="670f2-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="670f2-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="670f2-189">appAvailability</span></span>|[<span data-ttu-id="670f2-190">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="670f2-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="670f2-191">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="670f2-191">The Application's availability.</span></span> <span data-ttu-id="670f2-192">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="670f2-193">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="670f2-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="670f2-194">version</span><span class="sxs-lookup"><span data-stu-id="670f2-194">version</span></span>|<span data-ttu-id="670f2-195">String</span><span class="sxs-lookup"><span data-stu-id="670f2-195">String</span></span>|<span data-ttu-id="670f2-196">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="670f2-196">The Application's version.</span></span> <span data-ttu-id="670f2-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="670f2-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="670f2-198">packageId</span><span class="sxs-lookup"><span data-stu-id="670f2-198">packageId</span></span>|<span data-ttu-id="670f2-199">Строка</span><span class="sxs-lookup"><span data-stu-id="670f2-199">String</span></span>|<span data-ttu-id="670f2-200">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="670f2-200">The app's package ID.</span></span>|
|<span data-ttu-id="670f2-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="670f2-201">appStoreUrl</span></span>|<span data-ttu-id="670f2-202">String</span><span class="sxs-lookup"><span data-stu-id="670f2-202">String</span></span>|<span data-ttu-id="670f2-203">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="670f2-203">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="670f2-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="670f2-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="670f2-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="670f2-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="670f2-206">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="670f2-206">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="670f2-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="670f2-207">Response</span></span>
<span data-ttu-id="670f2-208">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="670f2-208">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="670f2-209">Пример</span><span class="sxs-lookup"><span data-stu-id="670f2-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="670f2-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="670f2-210">Request</span></span>
<span data-ttu-id="670f2-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="670f2-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1016

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
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="670f2-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="670f2-212">Response</span></span>
<span data-ttu-id="670f2-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="670f2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1188

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
    "v5_1": true
  }
}
```




