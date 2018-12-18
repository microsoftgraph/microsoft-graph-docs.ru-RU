---
title: Update managedAndroidStoreApp
description: Обновление свойств объекта managedAndroidStoreApp.
author: tfitzmac
ms.openlocfilehash: c592238c7c48939b47dfc772a93dea4f07f7bf06
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327645"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="0e631-103">Update managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="0e631-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="0e631-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0e631-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e631-105">Обновление свойств объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-105">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e631-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0e631-106">Prerequisites</span></span>
<span data-ttu-id="0e631-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e631-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e631-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e631-109">Permission type</span></span>|<span data-ttu-id="0e631-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e631-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e631-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e631-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e631-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e631-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0e631-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e631-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e631-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e631-114">Not supported.</span></span>|
|<span data-ttu-id="0e631-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e631-115">Application</span></span>|<span data-ttu-id="0e631-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e631-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e631-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e631-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="0e631-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e631-118">Request headers</span></span>
|<span data-ttu-id="0e631-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e631-119">Header</span></span>|<span data-ttu-id="0e631-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0e631-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e631-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e631-121">Authorization</span></span>|<span data-ttu-id="0e631-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0e631-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e631-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0e631-123">Accept</span></span>|<span data-ttu-id="0e631-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0e631-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e631-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0e631-125">Request body</span></span>
<span data-ttu-id="0e631-126">В теле запроса добавьте представление объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e631-126">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="0e631-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-127">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="0e631-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e631-128">Property</span></span>|<span data-ttu-id="0e631-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0e631-129">Type</span></span>|<span data-ttu-id="0e631-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0e631-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e631-131">id</span><span class="sxs-lookup"><span data-stu-id="0e631-131">id</span></span>|<span data-ttu-id="0e631-132">Строка</span><span class="sxs-lookup"><span data-stu-id="0e631-132">String</span></span>|<span data-ttu-id="0e631-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0e631-133">Key of the entity.</span></span> <span data-ttu-id="0e631-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0e631-135">displayName</span></span>|<span data-ttu-id="0e631-136">String</span><span class="sxs-lookup"><span data-stu-id="0e631-136">String</span></span>|<span data-ttu-id="0e631-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="0e631-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0e631-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-139">описание</span><span class="sxs-lookup"><span data-stu-id="0e631-139">description</span></span>|<span data-ttu-id="0e631-140">String</span><span class="sxs-lookup"><span data-stu-id="0e631-140">String</span></span>|<span data-ttu-id="0e631-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="0e631-141">The description of the app.</span></span> <span data-ttu-id="0e631-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-143">publisher</span><span class="sxs-lookup"><span data-stu-id="0e631-143">publisher</span></span>|<span data-ttu-id="0e631-144">String</span><span class="sxs-lookup"><span data-stu-id="0e631-144">String</span></span>|<span data-ttu-id="0e631-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="0e631-145">The publisher of the app.</span></span> <span data-ttu-id="0e631-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0e631-147">largeIcon</span></span>|[<span data-ttu-id="0e631-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0e631-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0e631-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="0e631-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0e631-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e631-151">createdDateTime</span></span>|<span data-ttu-id="0e631-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e631-152">DateTimeOffset</span></span>|<span data-ttu-id="0e631-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="0e631-153">The date and time the app was created.</span></span> <span data-ttu-id="0e631-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e631-155">lastModifiedDateTime</span></span>|<span data-ttu-id="0e631-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e631-156">DateTimeOffset</span></span>|<span data-ttu-id="0e631-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="0e631-157">The date and time the app was last modified.</span></span> <span data-ttu-id="0e631-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0e631-159">isFeatured</span></span>|<span data-ttu-id="0e631-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e631-160">Boolean</span></span>|<span data-ttu-id="0e631-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0e631-162">privacyInformationUrl</span></span>|<span data-ttu-id="0e631-163">String</span><span class="sxs-lookup"><span data-stu-id="0e631-163">String</span></span>|<span data-ttu-id="0e631-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="0e631-164">The privacy statement Url.</span></span> <span data-ttu-id="0e631-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0e631-166">informationUrl</span></span>|<span data-ttu-id="0e631-167">String</span><span class="sxs-lookup"><span data-stu-id="0e631-167">String</span></span>|<span data-ttu-id="0e631-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="0e631-168">The more information Url.</span></span> <span data-ttu-id="0e631-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-170">owner</span><span class="sxs-lookup"><span data-stu-id="0e631-170">owner</span></span>|<span data-ttu-id="0e631-171">String</span><span class="sxs-lookup"><span data-stu-id="0e631-171">String</span></span>|<span data-ttu-id="0e631-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="0e631-172">The owner of the app.</span></span> <span data-ttu-id="0e631-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-174">developer</span><span class="sxs-lookup"><span data-stu-id="0e631-174">developer</span></span>|<span data-ttu-id="0e631-175">String</span><span class="sxs-lookup"><span data-stu-id="0e631-175">String</span></span>|<span data-ttu-id="0e631-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="0e631-176">The developer of the app.</span></span> <span data-ttu-id="0e631-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-178">notes</span><span class="sxs-lookup"><span data-stu-id="0e631-178">notes</span></span>|<span data-ttu-id="0e631-179">String</span><span class="sxs-lookup"><span data-stu-id="0e631-179">String</span></span>|<span data-ttu-id="0e631-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="0e631-180">Notes for the app.</span></span> <span data-ttu-id="0e631-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e631-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="0e631-182">publishingState</span></span>|[<span data-ttu-id="0e631-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0e631-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0e631-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="0e631-184">The publishing state for the app.</span></span> <span data-ttu-id="0e631-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="0e631-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0e631-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0e631-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0e631-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0e631-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="0e631-188">appAvailability</span></span>|[<span data-ttu-id="0e631-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="0e631-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="0e631-190">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="0e631-190">The Application's availability.</span></span> <span data-ttu-id="0e631-191">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="0e631-192">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="0e631-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="0e631-193">version</span><span class="sxs-lookup"><span data-stu-id="0e631-193">version</span></span>|<span data-ttu-id="0e631-194">String</span><span class="sxs-lookup"><span data-stu-id="0e631-194">String</span></span>|<span data-ttu-id="0e631-195">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="0e631-195">The Application's version.</span></span> <span data-ttu-id="0e631-196">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e631-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="0e631-197">packageId</span><span class="sxs-lookup"><span data-stu-id="0e631-197">packageId</span></span>|<span data-ttu-id="0e631-198">String</span><span class="sxs-lookup"><span data-stu-id="0e631-198">String</span></span>|<span data-ttu-id="0e631-199">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="0e631-199">The app's package ID.</span></span>|
|<span data-ttu-id="0e631-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0e631-200">appStoreUrl</span></span>|<span data-ttu-id="0e631-201">String</span><span class="sxs-lookup"><span data-stu-id="0e631-201">String</span></span>|<span data-ttu-id="0e631-202">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="0e631-202">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="0e631-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0e631-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0e631-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0e631-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="0e631-205">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="0e631-205">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="0e631-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e631-206">Response</span></span>
<span data-ttu-id="0e631-207">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0e631-207">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e631-208">Пример</span><span class="sxs-lookup"><span data-stu-id="0e631-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e631-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e631-209">Request</span></span>
<span data-ttu-id="0e631-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e631-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="0e631-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e631-211">Response</span></span>
<span data-ttu-id="0e631-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0e631-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



