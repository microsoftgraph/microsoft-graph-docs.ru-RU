---
title: Create managedAndroidStoreApp
description: Создание нового объекта managedAndroidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bdd3e9638aac85e6631597286cb43a4ec5fc4fc0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831173"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="7e414-103">Create managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="7e414-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="7e414-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7e414-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e414-105">Создание нового объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-105">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e414-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7e414-106">Prerequisites</span></span>
<span data-ttu-id="7e414-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e414-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e414-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e414-109">Permission type</span></span>|<span data-ttu-id="7e414-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e414-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e414-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e414-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7e414-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e414-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7e414-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e414-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e414-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e414-114">Not supported.</span></span>|
|<span data-ttu-id="7e414-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e414-115">Application</span></span>|<span data-ttu-id="7e414-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e414-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e414-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e414-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7e414-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e414-118">Request headers</span></span>
|<span data-ttu-id="7e414-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7e414-119">Header</span></span>|<span data-ttu-id="7e414-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7e414-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e414-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e414-121">Authorization</span></span>|<span data-ttu-id="7e414-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7e414-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e414-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7e414-123">Accept</span></span>|<span data-ttu-id="7e414-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7e414-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e414-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e414-125">Request body</span></span>
<span data-ttu-id="7e414-126">В теле запроса добавьте представление объекта managedAndroidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e414-126">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="7e414-127">Ниже показаны свойства, которые необходимо указывать при создании объекта managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="7e414-127">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="7e414-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e414-128">Property</span></span>|<span data-ttu-id="7e414-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7e414-129">Type</span></span>|<span data-ttu-id="7e414-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7e414-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e414-131">id</span><span class="sxs-lookup"><span data-stu-id="7e414-131">id</span></span>|<span data-ttu-id="7e414-132">Строка</span><span class="sxs-lookup"><span data-stu-id="7e414-132">String</span></span>|<span data-ttu-id="7e414-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7e414-133">Key of the entity.</span></span> <span data-ttu-id="7e414-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7e414-135">displayName</span></span>|<span data-ttu-id="7e414-136">String</span><span class="sxs-lookup"><span data-stu-id="7e414-136">String</span></span>|<span data-ttu-id="7e414-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="7e414-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7e414-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-139">описание</span><span class="sxs-lookup"><span data-stu-id="7e414-139">description</span></span>|<span data-ttu-id="7e414-140">String</span><span class="sxs-lookup"><span data-stu-id="7e414-140">String</span></span>|<span data-ttu-id="7e414-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7e414-141">The description of the app.</span></span> <span data-ttu-id="7e414-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-143">publisher</span><span class="sxs-lookup"><span data-stu-id="7e414-143">publisher</span></span>|<span data-ttu-id="7e414-144">String</span><span class="sxs-lookup"><span data-stu-id="7e414-144">String</span></span>|<span data-ttu-id="7e414-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="7e414-145">The publisher of the app.</span></span> <span data-ttu-id="7e414-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7e414-147">largeIcon</span></span>|[<span data-ttu-id="7e414-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7e414-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7e414-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="7e414-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7e414-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e414-151">createdDateTime</span></span>|<span data-ttu-id="7e414-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e414-152">DateTimeOffset</span></span>|<span data-ttu-id="7e414-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="7e414-153">The date and time the app was created.</span></span> <span data-ttu-id="7e414-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e414-155">lastModifiedDateTime</span></span>|<span data-ttu-id="7e414-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e414-156">DateTimeOffset</span></span>|<span data-ttu-id="7e414-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="7e414-157">The date and time the app was last modified.</span></span> <span data-ttu-id="7e414-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7e414-159">isFeatured</span></span>|<span data-ttu-id="7e414-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e414-160">Boolean</span></span>|<span data-ttu-id="7e414-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7e414-162">privacyInformationUrl</span></span>|<span data-ttu-id="7e414-163">String</span><span class="sxs-lookup"><span data-stu-id="7e414-163">String</span></span>|<span data-ttu-id="7e414-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="7e414-164">The privacy statement Url.</span></span> <span data-ttu-id="7e414-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7e414-166">informationUrl</span></span>|<span data-ttu-id="7e414-167">String</span><span class="sxs-lookup"><span data-stu-id="7e414-167">String</span></span>|<span data-ttu-id="7e414-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="7e414-168">The more information Url.</span></span> <span data-ttu-id="7e414-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-170">owner</span><span class="sxs-lookup"><span data-stu-id="7e414-170">owner</span></span>|<span data-ttu-id="7e414-171">String</span><span class="sxs-lookup"><span data-stu-id="7e414-171">String</span></span>|<span data-ttu-id="7e414-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="7e414-172">The owner of the app.</span></span> <span data-ttu-id="7e414-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-174">developer</span><span class="sxs-lookup"><span data-stu-id="7e414-174">developer</span></span>|<span data-ttu-id="7e414-175">String</span><span class="sxs-lookup"><span data-stu-id="7e414-175">String</span></span>|<span data-ttu-id="7e414-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="7e414-176">The developer of the app.</span></span> <span data-ttu-id="7e414-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-178">notes</span><span class="sxs-lookup"><span data-stu-id="7e414-178">notes</span></span>|<span data-ttu-id="7e414-179">String</span><span class="sxs-lookup"><span data-stu-id="7e414-179">String</span></span>|<span data-ttu-id="7e414-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="7e414-180">Notes for the app.</span></span> <span data-ttu-id="7e414-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e414-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="7e414-182">publishingState</span></span>|[<span data-ttu-id="7e414-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7e414-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7e414-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="7e414-184">The publishing state for the app.</span></span> <span data-ttu-id="7e414-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="7e414-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7e414-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7e414-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7e414-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7e414-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="7e414-188">appAvailability</span></span>|[<span data-ttu-id="7e414-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="7e414-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="7e414-190">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="7e414-190">The Application's availability.</span></span> <span data-ttu-id="7e414-191">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="7e414-192">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="7e414-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="7e414-193">version</span><span class="sxs-lookup"><span data-stu-id="7e414-193">version</span></span>|<span data-ttu-id="7e414-194">String</span><span class="sxs-lookup"><span data-stu-id="7e414-194">String</span></span>|<span data-ttu-id="7e414-195">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="7e414-195">The Application's version.</span></span> <span data-ttu-id="7e414-196">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7e414-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="7e414-197">packageId</span><span class="sxs-lookup"><span data-stu-id="7e414-197">packageId</span></span>|<span data-ttu-id="7e414-198">String</span><span class="sxs-lookup"><span data-stu-id="7e414-198">String</span></span>|<span data-ttu-id="7e414-199">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="7e414-199">The app's package ID.</span></span>|
|<span data-ttu-id="7e414-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7e414-200">appStoreUrl</span></span>|<span data-ttu-id="7e414-201">String</span><span class="sxs-lookup"><span data-stu-id="7e414-201">String</span></span>|<span data-ttu-id="7e414-202">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="7e414-202">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="7e414-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7e414-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7e414-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7e414-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="7e414-205">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="7e414-205">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="7e414-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e414-206">Response</span></span>
<span data-ttu-id="7e414-207">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7e414-207">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e414-208">Пример</span><span class="sxs-lookup"><span data-stu-id="7e414-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="7e414-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e414-209">Request</span></span>
<span data-ttu-id="7e414-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e414-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7e414-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e414-211">Response</span></span>
<span data-ttu-id="7e414-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7e414-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



