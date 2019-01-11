---
title: Create webApp
description: Создание объекта webApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 87a293f1f4839fd02eac072a38ca1f91a2c3f7b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823431"
---
# <a name="create-webapp"></a><span data-ttu-id="fe5bb-103">Create webApp</span><span class="sxs-lookup"><span data-stu-id="fe5bb-103">Create webApp</span></span>

> <span data-ttu-id="fe5bb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe5bb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe5bb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe5bb-107">Создание объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-107">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe5bb-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fe5bb-108">Prerequisites</span></span>
<span data-ttu-id="fe5bb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe5bb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe5bb-111">Permission type</span></span>|<span data-ttu-id="fe5bb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe5bb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe5bb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe5bb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe5bb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe5bb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fe5bb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe5bb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe5bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-116">Not supported.</span></span>|
|<span data-ttu-id="fe5bb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe5bb-117">Application</span></span>|<span data-ttu-id="fe5bb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe5bb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe5bb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fe5bb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe5bb-120">Request headers</span></span>
|<span data-ttu-id="fe5bb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe5bb-121">Header</span></span>|<span data-ttu-id="fe5bb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fe5bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe5bb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe5bb-123">Authorization</span></span>|<span data-ttu-id="fe5bb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fe5bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe5bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe5bb-125">Accept</span></span>|<span data-ttu-id="fe5bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe5bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe5bb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe5bb-127">Request body</span></span>
<span data-ttu-id="fe5bb-128">В теле запроса добавьте представление объекта webApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-128">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="fe5bb-129">Ниже показаны свойства, которые необходимо указывать при создании объекта webApp.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-129">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="fe5bb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe5bb-130">Property</span></span>|<span data-ttu-id="fe5bb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fe5bb-131">Type</span></span>|<span data-ttu-id="fe5bb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fe5bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe5bb-133">id</span><span class="sxs-lookup"><span data-stu-id="fe5bb-133">id</span></span>|<span data-ttu-id="fe5bb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fe5bb-134">String</span></span>|<span data-ttu-id="fe5bb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-135">Key of the entity.</span></span> <span data-ttu-id="fe5bb-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fe5bb-137">displayName</span></span>|<span data-ttu-id="fe5bb-138">String</span><span class="sxs-lookup"><span data-stu-id="fe5bb-138">String</span></span>|<span data-ttu-id="fe5bb-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fe5bb-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-141">описание</span><span class="sxs-lookup"><span data-stu-id="fe5bb-141">description</span></span>|<span data-ttu-id="fe5bb-142">String</span><span class="sxs-lookup"><span data-stu-id="fe5bb-142">String</span></span>|<span data-ttu-id="fe5bb-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-143">The description of the app.</span></span> <span data-ttu-id="fe5bb-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-145">publisher</span><span class="sxs-lookup"><span data-stu-id="fe5bb-145">publisher</span></span>|<span data-ttu-id="fe5bb-146">String</span><span class="sxs-lookup"><span data-stu-id="fe5bb-146">String</span></span>|<span data-ttu-id="fe5bb-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-147">The publisher of the app.</span></span> <span data-ttu-id="fe5bb-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fe5bb-149">largeIcon</span></span>|[<span data-ttu-id="fe5bb-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fe5bb-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fe5bb-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fe5bb-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe5bb-153">createdDateTime</span></span>|<span data-ttu-id="fe5bb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe5bb-154">DateTimeOffset</span></span>|<span data-ttu-id="fe5bb-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-155">The date and time the app was created.</span></span> <span data-ttu-id="fe5bb-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe5bb-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fe5bb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe5bb-158">DateTimeOffset</span></span>|<span data-ttu-id="fe5bb-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-159">The date and time the app was last modified.</span></span> <span data-ttu-id="fe5bb-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fe5bb-161">isFeatured</span></span>|<span data-ttu-id="fe5bb-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe5bb-162">Boolean</span></span>|<span data-ttu-id="fe5bb-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fe5bb-164">privacyInformationUrl</span></span>|<span data-ttu-id="fe5bb-165">String</span><span class="sxs-lookup"><span data-stu-id="fe5bb-165">String</span></span>|<span data-ttu-id="fe5bb-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-166">The privacy statement Url.</span></span> <span data-ttu-id="fe5bb-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fe5bb-168">informationUrl</span></span>|<span data-ttu-id="fe5bb-169">String</span><span class="sxs-lookup"><span data-stu-id="fe5bb-169">String</span></span>|<span data-ttu-id="fe5bb-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-170">The more information Url.</span></span> <span data-ttu-id="fe5bb-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-172">owner</span><span class="sxs-lookup"><span data-stu-id="fe5bb-172">owner</span></span>|<span data-ttu-id="fe5bb-173">String</span><span class="sxs-lookup"><span data-stu-id="fe5bb-173">String</span></span>|<span data-ttu-id="fe5bb-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-174">The owner of the app.</span></span> <span data-ttu-id="fe5bb-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-176">developer</span><span class="sxs-lookup"><span data-stu-id="fe5bb-176">developer</span></span>|<span data-ttu-id="fe5bb-177">String</span><span class="sxs-lookup"><span data-stu-id="fe5bb-177">String</span></span>|<span data-ttu-id="fe5bb-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-178">The developer of the app.</span></span> <span data-ttu-id="fe5bb-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-180">notes</span><span class="sxs-lookup"><span data-stu-id="fe5bb-180">notes</span></span>|<span data-ttu-id="fe5bb-181">String</span><span class="sxs-lookup"><span data-stu-id="fe5bb-181">String</span></span>|<span data-ttu-id="fe5bb-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-182">Notes for the app.</span></span> <span data-ttu-id="fe5bb-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="fe5bb-184">uploadState</span></span>|<span data-ttu-id="fe5bb-185">Int32</span><span class="sxs-lookup"><span data-stu-id="fe5bb-185">Int32</span></span>|<span data-ttu-id="fe5bb-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-186">The upload state.</span></span> <span data-ttu-id="fe5bb-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe5bb-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="fe5bb-188">publishingState</span></span>|[<span data-ttu-id="fe5bb-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fe5bb-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fe5bb-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-190">The publishing state for the app.</span></span> <span data-ttu-id="fe5bb-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fe5bb-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe5bb-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="fe5bb-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fe5bb-194">appUrl</span><span class="sxs-lookup"><span data-stu-id="fe5bb-194">appUrl</span></span>|<span data-ttu-id="fe5bb-195">String</span><span class="sxs-lookup"><span data-stu-id="fe5bb-195">String</span></span>|<span data-ttu-id="fe5bb-196">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-196">The web app URL.</span></span>|
|<span data-ttu-id="fe5bb-197">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="fe5bb-197">useManagedBrowser</span></span>|<span data-ttu-id="fe5bb-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe5bb-198">Boolean</span></span>|<span data-ttu-id="fe5bb-199">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-199">Whether or not to use managed browser.</span></span> <span data-ttu-id="fe5bb-200">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-200">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="fe5bb-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe5bb-201">Response</span></span>
<span data-ttu-id="fe5bb-202">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [webApp](../resources/intune-apps-webapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-202">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe5bb-203">Пример</span><span class="sxs-lookup"><span data-stu-id="fe5bb-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe5bb-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe5bb-204">Request</span></span>
<span data-ttu-id="fe5bb-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 731

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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="fe5bb-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe5bb-206">Response</span></span>
<span data-ttu-id="fe5bb-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fe5bb-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 839

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
  "uploadState": 11,
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```





