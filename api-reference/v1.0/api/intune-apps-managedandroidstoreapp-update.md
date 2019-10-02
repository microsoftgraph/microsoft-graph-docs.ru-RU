---
title: Update managedAndroidStoreApp
description: Обновление свойств объекта managedAndroidStoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5f8fb536da2b8b2898322edd0adfa711be4b655
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358685"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="b7eed-103">Update managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="b7eed-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="b7eed-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7eed-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7eed-105">Обновление свойств объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-105">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7eed-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b7eed-106">Prerequisites</span></span>
<span data-ttu-id="b7eed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7eed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7eed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7eed-109">Permission type</span></span>|<span data-ttu-id="b7eed-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7eed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7eed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7eed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b7eed-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7eed-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b7eed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7eed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7eed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7eed-114">Not supported.</span></span>|
|<span data-ttu-id="b7eed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7eed-115">Application</span></span>|<span data-ttu-id="b7eed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7eed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7eed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7eed-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b7eed-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7eed-118">Request headers</span></span>
|<span data-ttu-id="b7eed-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7eed-119">Header</span></span>|<span data-ttu-id="b7eed-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b7eed-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7eed-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7eed-121">Authorization</span></span>|<span data-ttu-id="b7eed-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7eed-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7eed-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b7eed-123">Accept</span></span>|<span data-ttu-id="b7eed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b7eed-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7eed-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7eed-125">Request body</span></span>
<span data-ttu-id="b7eed-126">В теле запроса добавьте представление объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7eed-126">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="b7eed-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-127">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="b7eed-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7eed-128">Property</span></span>|<span data-ttu-id="b7eed-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b7eed-129">Type</span></span>|<span data-ttu-id="b7eed-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b7eed-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7eed-131">id</span><span class="sxs-lookup"><span data-stu-id="b7eed-131">id</span></span>|<span data-ttu-id="b7eed-132">Строка</span><span class="sxs-lookup"><span data-stu-id="b7eed-132">String</span></span>|<span data-ttu-id="b7eed-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b7eed-133">Key of the entity.</span></span> <span data-ttu-id="b7eed-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b7eed-135">displayName</span></span>|<span data-ttu-id="b7eed-136">Строка</span><span class="sxs-lookup"><span data-stu-id="b7eed-136">String</span></span>|<span data-ttu-id="b7eed-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b7eed-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b7eed-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-139">description</span><span class="sxs-lookup"><span data-stu-id="b7eed-139">description</span></span>|<span data-ttu-id="b7eed-140">String</span><span class="sxs-lookup"><span data-stu-id="b7eed-140">String</span></span>|<span data-ttu-id="b7eed-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b7eed-141">The description of the app.</span></span> <span data-ttu-id="b7eed-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-143">publisher</span><span class="sxs-lookup"><span data-stu-id="b7eed-143">publisher</span></span>|<span data-ttu-id="b7eed-144">String</span><span class="sxs-lookup"><span data-stu-id="b7eed-144">String</span></span>|<span data-ttu-id="b7eed-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b7eed-145">The publisher of the app.</span></span> <span data-ttu-id="b7eed-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b7eed-147">largeIcon</span></span>|[<span data-ttu-id="b7eed-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b7eed-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b7eed-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b7eed-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b7eed-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7eed-151">createdDateTime</span></span>|<span data-ttu-id="b7eed-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7eed-152">DateTimeOffset</span></span>|<span data-ttu-id="b7eed-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b7eed-153">The date and time the app was created.</span></span> <span data-ttu-id="b7eed-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7eed-155">lastModifiedDateTime</span></span>|<span data-ttu-id="b7eed-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7eed-156">DateTimeOffset</span></span>|<span data-ttu-id="b7eed-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b7eed-157">The date and time the app was last modified.</span></span> <span data-ttu-id="b7eed-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b7eed-159">isFeatured</span></span>|<span data-ttu-id="b7eed-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7eed-160">Boolean</span></span>|<span data-ttu-id="b7eed-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b7eed-162">privacyInformationUrl</span></span>|<span data-ttu-id="b7eed-163">String</span><span class="sxs-lookup"><span data-stu-id="b7eed-163">String</span></span>|<span data-ttu-id="b7eed-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b7eed-164">The privacy statement Url.</span></span> <span data-ttu-id="b7eed-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b7eed-166">informationUrl</span></span>|<span data-ttu-id="b7eed-167">String</span><span class="sxs-lookup"><span data-stu-id="b7eed-167">String</span></span>|<span data-ttu-id="b7eed-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b7eed-168">The more information Url.</span></span> <span data-ttu-id="b7eed-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-170">owner</span><span class="sxs-lookup"><span data-stu-id="b7eed-170">owner</span></span>|<span data-ttu-id="b7eed-171">String</span><span class="sxs-lookup"><span data-stu-id="b7eed-171">String</span></span>|<span data-ttu-id="b7eed-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b7eed-172">The owner of the app.</span></span> <span data-ttu-id="b7eed-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-174">developer</span><span class="sxs-lookup"><span data-stu-id="b7eed-174">developer</span></span>|<span data-ttu-id="b7eed-175">String</span><span class="sxs-lookup"><span data-stu-id="b7eed-175">String</span></span>|<span data-ttu-id="b7eed-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b7eed-176">The developer of the app.</span></span> <span data-ttu-id="b7eed-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-178">notes</span><span class="sxs-lookup"><span data-stu-id="b7eed-178">notes</span></span>|<span data-ttu-id="b7eed-179">String</span><span class="sxs-lookup"><span data-stu-id="b7eed-179">String</span></span>|<span data-ttu-id="b7eed-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="b7eed-180">Notes for the app.</span></span> <span data-ttu-id="b7eed-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7eed-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="b7eed-182">publishingState</span></span>|[<span data-ttu-id="b7eed-183">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="b7eed-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b7eed-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="b7eed-184">The publishing state for the app.</span></span> <span data-ttu-id="b7eed-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b7eed-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b7eed-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b7eed-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b7eed-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b7eed-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="b7eed-188">appAvailability</span></span>|[<span data-ttu-id="b7eed-189">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="b7eed-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="b7eed-190">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="b7eed-190">The Application's availability.</span></span> <span data-ttu-id="b7eed-191">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="b7eed-192">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="b7eed-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="b7eed-193">version</span><span class="sxs-lookup"><span data-stu-id="b7eed-193">version</span></span>|<span data-ttu-id="b7eed-194">String</span><span class="sxs-lookup"><span data-stu-id="b7eed-194">String</span></span>|<span data-ttu-id="b7eed-195">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="b7eed-195">The Application's version.</span></span> <span data-ttu-id="b7eed-196">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b7eed-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="b7eed-197">packageId</span><span class="sxs-lookup"><span data-stu-id="b7eed-197">packageId</span></span>|<span data-ttu-id="b7eed-198">String</span><span class="sxs-lookup"><span data-stu-id="b7eed-198">String</span></span>|<span data-ttu-id="b7eed-199">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="b7eed-199">The app's package ID.</span></span>|
|<span data-ttu-id="b7eed-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b7eed-200">appStoreUrl</span></span>|<span data-ttu-id="b7eed-201">String</span><span class="sxs-lookup"><span data-stu-id="b7eed-201">String</span></span>|<span data-ttu-id="b7eed-202">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="b7eed-202">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="b7eed-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b7eed-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b7eed-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b7eed-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="b7eed-205">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="b7eed-205">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="b7eed-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7eed-206">Response</span></span>
<span data-ttu-id="b7eed-207">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b7eed-207">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7eed-208">Пример</span><span class="sxs-lookup"><span data-stu-id="b7eed-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7eed-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7eed-209">Request</span></span>
<span data-ttu-id="b7eed-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7eed-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b7eed-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7eed-211">Response</span></span>
<span data-ttu-id="b7eed-p117">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7eed-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




