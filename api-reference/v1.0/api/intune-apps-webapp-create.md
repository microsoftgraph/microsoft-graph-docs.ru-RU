---
title: Create webApp
description: Создание объекта webApp.
author: tfitzmac
ms.openlocfilehash: 75d26e735db898f6175aed3ce5999c3a47e6bcdb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343794"
---
# <a name="create-webapp"></a><span data-ttu-id="658ed-103">Create webApp</span><span class="sxs-lookup"><span data-stu-id="658ed-103">Create webApp</span></span>

> <span data-ttu-id="658ed-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="658ed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="658ed-105">Создание объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-105">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="658ed-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="658ed-106">Prerequisites</span></span>
<span data-ttu-id="658ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="658ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="658ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="658ed-109">Permission type</span></span>|<span data-ttu-id="658ed-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="658ed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="658ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="658ed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="658ed-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="658ed-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="658ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="658ed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="658ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="658ed-114">Not supported.</span></span>|
|<span data-ttu-id="658ed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="658ed-115">Application</span></span>|<span data-ttu-id="658ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="658ed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="658ed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="658ed-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="658ed-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="658ed-118">Request headers</span></span>
|<span data-ttu-id="658ed-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="658ed-119">Header</span></span>|<span data-ttu-id="658ed-120">Значение</span><span class="sxs-lookup"><span data-stu-id="658ed-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="658ed-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="658ed-121">Authorization</span></span>|<span data-ttu-id="658ed-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="658ed-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="658ed-123">Accept</span><span class="sxs-lookup"><span data-stu-id="658ed-123">Accept</span></span>|<span data-ttu-id="658ed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="658ed-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="658ed-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="658ed-125">Request body</span></span>
<span data-ttu-id="658ed-126">В теле запроса добавьте представление объекта webApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="658ed-126">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="658ed-127">Ниже показаны свойства, которые необходимо указывать при создании объекта webApp.</span><span class="sxs-lookup"><span data-stu-id="658ed-127">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="658ed-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="658ed-128">Property</span></span>|<span data-ttu-id="658ed-129">Тип</span><span class="sxs-lookup"><span data-stu-id="658ed-129">Type</span></span>|<span data-ttu-id="658ed-130">Описание</span><span class="sxs-lookup"><span data-stu-id="658ed-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="658ed-131">id</span><span class="sxs-lookup"><span data-stu-id="658ed-131">id</span></span>|<span data-ttu-id="658ed-132">Строка</span><span class="sxs-lookup"><span data-stu-id="658ed-132">String</span></span>|<span data-ttu-id="658ed-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="658ed-133">Key of the entity.</span></span> <span data-ttu-id="658ed-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-135">displayName</span><span class="sxs-lookup"><span data-stu-id="658ed-135">displayName</span></span>|<span data-ttu-id="658ed-136">String</span><span class="sxs-lookup"><span data-stu-id="658ed-136">String</span></span>|<span data-ttu-id="658ed-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="658ed-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="658ed-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-139">описание</span><span class="sxs-lookup"><span data-stu-id="658ed-139">description</span></span>|<span data-ttu-id="658ed-140">String</span><span class="sxs-lookup"><span data-stu-id="658ed-140">String</span></span>|<span data-ttu-id="658ed-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="658ed-141">The description of the app.</span></span> <span data-ttu-id="658ed-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-143">publisher</span><span class="sxs-lookup"><span data-stu-id="658ed-143">publisher</span></span>|<span data-ttu-id="658ed-144">String</span><span class="sxs-lookup"><span data-stu-id="658ed-144">String</span></span>|<span data-ttu-id="658ed-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="658ed-145">The publisher of the app.</span></span> <span data-ttu-id="658ed-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="658ed-147">largeIcon</span></span>|[<span data-ttu-id="658ed-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="658ed-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="658ed-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="658ed-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="658ed-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="658ed-151">createdDateTime</span></span>|<span data-ttu-id="658ed-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="658ed-152">DateTimeOffset</span></span>|<span data-ttu-id="658ed-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="658ed-153">The date and time the app was created.</span></span> <span data-ttu-id="658ed-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="658ed-155">lastModifiedDateTime</span></span>|<span data-ttu-id="658ed-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="658ed-156">DateTimeOffset</span></span>|<span data-ttu-id="658ed-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="658ed-157">The date and time the app was last modified.</span></span> <span data-ttu-id="658ed-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="658ed-159">isFeatured</span></span>|<span data-ttu-id="658ed-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="658ed-160">Boolean</span></span>|<span data-ttu-id="658ed-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="658ed-162">privacyInformationUrl</span></span>|<span data-ttu-id="658ed-163">String</span><span class="sxs-lookup"><span data-stu-id="658ed-163">String</span></span>|<span data-ttu-id="658ed-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="658ed-164">The privacy statement Url.</span></span> <span data-ttu-id="658ed-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="658ed-166">informationUrl</span></span>|<span data-ttu-id="658ed-167">String</span><span class="sxs-lookup"><span data-stu-id="658ed-167">String</span></span>|<span data-ttu-id="658ed-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="658ed-168">The more information Url.</span></span> <span data-ttu-id="658ed-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-170">owner</span><span class="sxs-lookup"><span data-stu-id="658ed-170">owner</span></span>|<span data-ttu-id="658ed-171">String</span><span class="sxs-lookup"><span data-stu-id="658ed-171">String</span></span>|<span data-ttu-id="658ed-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="658ed-172">The owner of the app.</span></span> <span data-ttu-id="658ed-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-174">developer</span><span class="sxs-lookup"><span data-stu-id="658ed-174">developer</span></span>|<span data-ttu-id="658ed-175">String</span><span class="sxs-lookup"><span data-stu-id="658ed-175">String</span></span>|<span data-ttu-id="658ed-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="658ed-176">The developer of the app.</span></span> <span data-ttu-id="658ed-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-178">notes</span><span class="sxs-lookup"><span data-stu-id="658ed-178">notes</span></span>|<span data-ttu-id="658ed-179">String</span><span class="sxs-lookup"><span data-stu-id="658ed-179">String</span></span>|<span data-ttu-id="658ed-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="658ed-180">Notes for the app.</span></span> <span data-ttu-id="658ed-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="658ed-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="658ed-182">publishingState</span></span>|[<span data-ttu-id="658ed-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="658ed-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="658ed-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="658ed-184">The publishing state for the app.</span></span> <span data-ttu-id="658ed-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="658ed-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="658ed-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="658ed-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="658ed-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="658ed-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="658ed-188">appUrl</span><span class="sxs-lookup"><span data-stu-id="658ed-188">appUrl</span></span>|<span data-ttu-id="658ed-189">String</span><span class="sxs-lookup"><span data-stu-id="658ed-189">String</span></span>|<span data-ttu-id="658ed-190">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="658ed-190">The web app URL.</span></span>|
|<span data-ttu-id="658ed-191">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="658ed-191">useManagedBrowser</span></span>|<span data-ttu-id="658ed-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="658ed-192">Boolean</span></span>|<span data-ttu-id="658ed-193">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="658ed-193">Whether or not to use managed browser.</span></span> <span data-ttu-id="658ed-194">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="658ed-194">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="658ed-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="658ed-195">Response</span></span>
<span data-ttu-id="658ed-196">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [webApp](../resources/intune-apps-webapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="658ed-196">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="658ed-197">Пример</span><span class="sxs-lookup"><span data-stu-id="658ed-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="658ed-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="658ed-198">Request</span></span>
<span data-ttu-id="658ed-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="658ed-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="658ed-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="658ed-200">Response</span></span>
<span data-ttu-id="658ed-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="658ed-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 817

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```



