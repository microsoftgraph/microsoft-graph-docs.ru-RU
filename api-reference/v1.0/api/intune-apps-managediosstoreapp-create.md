---
title: Create managedIOSStoreApp
description: Создание объекта managedIOSStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ee9399e604c2a380b8224cd68db1a406bf62908
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548469"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="9a703-103">Create managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="9a703-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="9a703-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a703-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a703-105">Создание объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-105">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a703-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9a703-106">Prerequisites</span></span>
<span data-ttu-id="9a703-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a703-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a703-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a703-109">Permission type</span></span>|<span data-ttu-id="9a703-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a703-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a703-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a703-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9a703-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a703-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9a703-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a703-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a703-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a703-114">Not supported.</span></span>|
|<span data-ttu-id="9a703-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a703-115">Application</span></span>|<span data-ttu-id="9a703-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a703-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a703-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a703-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9a703-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a703-118">Request headers</span></span>
|<span data-ttu-id="9a703-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a703-119">Header</span></span>|<span data-ttu-id="9a703-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9a703-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a703-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a703-121">Authorization</span></span>|<span data-ttu-id="9a703-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a703-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a703-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9a703-123">Accept</span></span>|<span data-ttu-id="9a703-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9a703-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a703-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a703-125">Request body</span></span>
<span data-ttu-id="9a703-126">В теле запроса добавьте представление объекта managedIOSStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a703-126">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="9a703-127">Ниже показаны свойства, которые необходимо указывать при создании объекта managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="9a703-127">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="9a703-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a703-128">Property</span></span>|<span data-ttu-id="9a703-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9a703-129">Type</span></span>|<span data-ttu-id="9a703-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9a703-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a703-131">id</span><span class="sxs-lookup"><span data-stu-id="9a703-131">id</span></span>|<span data-ttu-id="9a703-132">Строка</span><span class="sxs-lookup"><span data-stu-id="9a703-132">String</span></span>|<span data-ttu-id="9a703-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9a703-133">Key of the entity.</span></span> <span data-ttu-id="9a703-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9a703-135">displayName</span></span>|<span data-ttu-id="9a703-136">String</span><span class="sxs-lookup"><span data-stu-id="9a703-136">String</span></span>|<span data-ttu-id="9a703-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9a703-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9a703-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-139">description</span><span class="sxs-lookup"><span data-stu-id="9a703-139">description</span></span>|<span data-ttu-id="9a703-140">String</span><span class="sxs-lookup"><span data-stu-id="9a703-140">String</span></span>|<span data-ttu-id="9a703-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9a703-141">The description of the app.</span></span> <span data-ttu-id="9a703-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-143">publisher</span><span class="sxs-lookup"><span data-stu-id="9a703-143">publisher</span></span>|<span data-ttu-id="9a703-144">String</span><span class="sxs-lookup"><span data-stu-id="9a703-144">String</span></span>|<span data-ttu-id="9a703-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9a703-145">The publisher of the app.</span></span> <span data-ttu-id="9a703-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9a703-147">largeIcon</span></span>|[<span data-ttu-id="9a703-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9a703-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9a703-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9a703-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9a703-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a703-151">createdDateTime</span></span>|<span data-ttu-id="9a703-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a703-152">DateTimeOffset</span></span>|<span data-ttu-id="9a703-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9a703-153">The date and time the app was created.</span></span> <span data-ttu-id="9a703-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a703-155">lastModifiedDateTime</span></span>|<span data-ttu-id="9a703-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a703-156">DateTimeOffset</span></span>|<span data-ttu-id="9a703-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9a703-157">The date and time the app was last modified.</span></span> <span data-ttu-id="9a703-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9a703-159">isFeatured</span></span>|<span data-ttu-id="9a703-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a703-160">Boolean</span></span>|<span data-ttu-id="9a703-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9a703-162">privacyInformationUrl</span></span>|<span data-ttu-id="9a703-163">String</span><span class="sxs-lookup"><span data-stu-id="9a703-163">String</span></span>|<span data-ttu-id="9a703-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9a703-164">The privacy statement Url.</span></span> <span data-ttu-id="9a703-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9a703-166">informationUrl</span></span>|<span data-ttu-id="9a703-167">String</span><span class="sxs-lookup"><span data-stu-id="9a703-167">String</span></span>|<span data-ttu-id="9a703-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9a703-168">The more information Url.</span></span> <span data-ttu-id="9a703-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-170">owner</span><span class="sxs-lookup"><span data-stu-id="9a703-170">owner</span></span>|<span data-ttu-id="9a703-171">String</span><span class="sxs-lookup"><span data-stu-id="9a703-171">String</span></span>|<span data-ttu-id="9a703-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9a703-172">The owner of the app.</span></span> <span data-ttu-id="9a703-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-174">developer</span><span class="sxs-lookup"><span data-stu-id="9a703-174">developer</span></span>|<span data-ttu-id="9a703-175">String</span><span class="sxs-lookup"><span data-stu-id="9a703-175">String</span></span>|<span data-ttu-id="9a703-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9a703-176">The developer of the app.</span></span> <span data-ttu-id="9a703-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-178">notes</span><span class="sxs-lookup"><span data-stu-id="9a703-178">notes</span></span>|<span data-ttu-id="9a703-179">String</span><span class="sxs-lookup"><span data-stu-id="9a703-179">String</span></span>|<span data-ttu-id="9a703-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9a703-180">Notes for the app.</span></span> <span data-ttu-id="9a703-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9a703-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="9a703-182">publishingState</span></span>|[<span data-ttu-id="9a703-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9a703-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9a703-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="9a703-184">The publishing state for the app.</span></span> <span data-ttu-id="9a703-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9a703-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9a703-186">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9a703-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9a703-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9a703-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="9a703-188">appAvailability</span></span>|[<span data-ttu-id="9a703-189">Манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="9a703-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="9a703-190">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="9a703-190">The Application's availability.</span></span> <span data-ttu-id="9a703-191">НаСледуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9a703-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="9a703-192">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="9a703-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="9a703-193">version</span><span class="sxs-lookup"><span data-stu-id="9a703-193">version</span></span>|<span data-ttu-id="9a703-194">String</span><span class="sxs-lookup"><span data-stu-id="9a703-194">String</span></span>|<span data-ttu-id="9a703-195">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="9a703-195">The Application's version.</span></span> <span data-ttu-id="9a703-196">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="9a703-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="9a703-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="9a703-197">bundleId</span></span>|<span data-ttu-id="9a703-198">String</span><span class="sxs-lookup"><span data-stu-id="9a703-198">String</span></span>|<span data-ttu-id="9a703-199">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="9a703-199">The app's Bundle ID.</span></span>|
|<span data-ttu-id="9a703-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9a703-200">appStoreUrl</span></span>|<span data-ttu-id="9a703-201">String</span><span class="sxs-lookup"><span data-stu-id="9a703-201">String</span></span>|<span data-ttu-id="9a703-202">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="9a703-202">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="9a703-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9a703-203">applicableDeviceType</span></span>|[<span data-ttu-id="9a703-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9a703-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="9a703-205">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="9a703-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="9a703-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9a703-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9a703-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9a703-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="9a703-208">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="9a703-208">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="9a703-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a703-209">Response</span></span>
<span data-ttu-id="9a703-210">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9a703-210">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a703-211">Пример</span><span class="sxs-lookup"><span data-stu-id="9a703-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a703-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a703-212">Request</span></span>
<span data-ttu-id="9a703-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a703-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1084

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="9a703-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a703-214">Response</span></span>
<span data-ttu-id="9a703-p117">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a703-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1256

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```



