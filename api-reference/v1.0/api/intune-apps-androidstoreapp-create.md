---
title: Создание объекта androidStoreApp
description: Создание объекта androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ceabaceec42dd6a4ca884af2c7e2b37c044f16a0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263835"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="a23f3-103">Создание объекта androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="a23f3-103">Create androidStoreApp</span></span>

> <span data-ttu-id="a23f3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a23f3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a23f3-105">Создание объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-105">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a23f3-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a23f3-106">Prerequisites</span></span>
<span data-ttu-id="a23f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a23f3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a23f3-109">Permission type</span></span>|<span data-ttu-id="a23f3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a23f3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a23f3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a23f3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a23f3-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a23f3-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a23f3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a23f3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a23f3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a23f3-114">Not supported.</span></span>|
|<span data-ttu-id="a23f3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a23f3-115">Application</span></span>|<span data-ttu-id="a23f3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a23f3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a23f3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a23f3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a23f3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a23f3-118">Request headers</span></span>
|<span data-ttu-id="a23f3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a23f3-119">Header</span></span>|<span data-ttu-id="a23f3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a23f3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a23f3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a23f3-121">Authorization</span></span>|<span data-ttu-id="a23f3-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a23f3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a23f3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a23f3-123">Accept</span></span>|<span data-ttu-id="a23f3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a23f3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a23f3-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a23f3-125">Request body</span></span>
<span data-ttu-id="a23f3-126">В тексте запроса добавьте представление объекта androidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a23f3-126">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="a23f3-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="a23f3-127">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="a23f3-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a23f3-128">Property</span></span>|<span data-ttu-id="a23f3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a23f3-129">Type</span></span>|<span data-ttu-id="a23f3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a23f3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a23f3-131">id</span><span class="sxs-lookup"><span data-stu-id="a23f3-131">id</span></span>|<span data-ttu-id="a23f3-132">Строка</span><span class="sxs-lookup"><span data-stu-id="a23f3-132">String</span></span>|<span data-ttu-id="a23f3-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a23f3-133">Key of the entity.</span></span> <span data-ttu-id="a23f3-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a23f3-135">displayName</span></span>|<span data-ttu-id="a23f3-136">String</span><span class="sxs-lookup"><span data-stu-id="a23f3-136">String</span></span>|<span data-ttu-id="a23f3-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a23f3-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a23f3-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-139">description</span><span class="sxs-lookup"><span data-stu-id="a23f3-139">description</span></span>|<span data-ttu-id="a23f3-140">Строка</span><span class="sxs-lookup"><span data-stu-id="a23f3-140">String</span></span>|<span data-ttu-id="a23f3-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a23f3-141">The description of the app.</span></span> <span data-ttu-id="a23f3-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-143">publisher</span><span class="sxs-lookup"><span data-stu-id="a23f3-143">publisher</span></span>|<span data-ttu-id="a23f3-144">String</span><span class="sxs-lookup"><span data-stu-id="a23f3-144">String</span></span>|<span data-ttu-id="a23f3-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a23f3-145">The publisher of the app.</span></span> <span data-ttu-id="a23f3-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a23f3-147">largeIcon</span></span>|[<span data-ttu-id="a23f3-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a23f3-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a23f3-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a23f3-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a23f3-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a23f3-151">createdDateTime</span></span>|<span data-ttu-id="a23f3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a23f3-152">DateTimeOffset</span></span>|<span data-ttu-id="a23f3-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a23f3-153">The date and time the app was created.</span></span> <span data-ttu-id="a23f3-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a23f3-155">lastModifiedDateTime</span></span>|<span data-ttu-id="a23f3-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a23f3-156">DateTimeOffset</span></span>|<span data-ttu-id="a23f3-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a23f3-157">The date and time the app was last modified.</span></span> <span data-ttu-id="a23f3-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a23f3-159">isFeatured</span></span>|<span data-ttu-id="a23f3-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="a23f3-160">Boolean</span></span>|<span data-ttu-id="a23f3-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a23f3-162">privacyInformationUrl</span></span>|<span data-ttu-id="a23f3-163">String</span><span class="sxs-lookup"><span data-stu-id="a23f3-163">String</span></span>|<span data-ttu-id="a23f3-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a23f3-164">The privacy statement Url.</span></span> <span data-ttu-id="a23f3-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a23f3-166">informationUrl</span></span>|<span data-ttu-id="a23f3-167">String</span><span class="sxs-lookup"><span data-stu-id="a23f3-167">String</span></span>|<span data-ttu-id="a23f3-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a23f3-168">The more information Url.</span></span> <span data-ttu-id="a23f3-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-170">owner</span><span class="sxs-lookup"><span data-stu-id="a23f3-170">owner</span></span>|<span data-ttu-id="a23f3-171">Строка</span><span class="sxs-lookup"><span data-stu-id="a23f3-171">String</span></span>|<span data-ttu-id="a23f3-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a23f3-172">The owner of the app.</span></span> <span data-ttu-id="a23f3-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-174">developer</span><span class="sxs-lookup"><span data-stu-id="a23f3-174">developer</span></span>|<span data-ttu-id="a23f3-175">String</span><span class="sxs-lookup"><span data-stu-id="a23f3-175">String</span></span>|<span data-ttu-id="a23f3-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a23f3-176">The developer of the app.</span></span> <span data-ttu-id="a23f3-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-178">notes</span><span class="sxs-lookup"><span data-stu-id="a23f3-178">notes</span></span>|<span data-ttu-id="a23f3-179">String</span><span class="sxs-lookup"><span data-stu-id="a23f3-179">String</span></span>|<span data-ttu-id="a23f3-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="a23f3-180">Notes for the app.</span></span> <span data-ttu-id="a23f3-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a23f3-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="a23f3-182">publishingState</span></span>|[<span data-ttu-id="a23f3-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="a23f3-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a23f3-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="a23f3-184">The publishing state for the app.</span></span> <span data-ttu-id="a23f3-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a23f3-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a23f3-186">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a23f3-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a23f3-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a23f3-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a23f3-188">packageId</span><span class="sxs-lookup"><span data-stu-id="a23f3-188">packageId</span></span>|<span data-ttu-id="a23f3-189">String</span><span class="sxs-lookup"><span data-stu-id="a23f3-189">String</span></span>|<span data-ttu-id="a23f3-190">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="a23f3-190">The package identifier.</span></span>|
|<span data-ttu-id="a23f3-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a23f3-191">appStoreUrl</span></span>|<span data-ttu-id="a23f3-192">String</span><span class="sxs-lookup"><span data-stu-id="a23f3-192">String</span></span>|<span data-ttu-id="a23f3-193">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="a23f3-193">The Android app store URL.</span></span>|
|<span data-ttu-id="a23f3-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a23f3-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a23f3-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a23f3-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="a23f3-196">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="a23f3-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="a23f3-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="a23f3-197">Response</span></span>
<span data-ttu-id="a23f3-198">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a23f3-198">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a23f3-199">Пример</span><span class="sxs-lookup"><span data-stu-id="a23f3-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="a23f3-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="a23f3-200">Request</span></span>
<span data-ttu-id="a23f3-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a23f3-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a23f3-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="a23f3-202">Response</span></span>
<span data-ttu-id="a23f3-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a23f3-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



