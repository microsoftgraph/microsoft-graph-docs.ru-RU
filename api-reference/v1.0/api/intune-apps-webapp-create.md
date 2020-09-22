---
title: Create webApp
description: Создание объекта webApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c43bd91bf846f5e262cf1ec4ecf1998ebd4c520c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013211"
---
# <a name="create-webapp"></a><span data-ttu-id="3ad45-103">Create webApp</span><span class="sxs-lookup"><span data-stu-id="3ad45-103">Create webApp</span></span>

<span data-ttu-id="3ad45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ad45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ad45-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ad45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ad45-106">Создание объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-106">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ad45-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3ad45-107">Prerequisites</span></span>
<span data-ttu-id="3ad45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ad45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ad45-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ad45-110">Permission type</span></span>|<span data-ttu-id="3ad45-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ad45-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ad45-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ad45-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ad45-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ad45-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3ad45-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ad45-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ad45-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ad45-115">Not supported.</span></span>|
|<span data-ttu-id="3ad45-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ad45-116">Application</span></span>|<span data-ttu-id="3ad45-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ad45-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ad45-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ad45-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3ad45-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3ad45-119">Request headers</span></span>
|<span data-ttu-id="3ad45-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ad45-120">Header</span></span>|<span data-ttu-id="3ad45-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3ad45-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ad45-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ad45-122">Authorization</span></span>|<span data-ttu-id="3ad45-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ad45-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ad45-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3ad45-124">Accept</span></span>|<span data-ttu-id="3ad45-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ad45-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ad45-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ad45-126">Request body</span></span>
<span data-ttu-id="3ad45-127">В теле запроса добавьте представление объекта webApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ad45-127">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="3ad45-128">Ниже показаны свойства, которые необходимо указывать при создании объекта webApp.</span><span class="sxs-lookup"><span data-stu-id="3ad45-128">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="3ad45-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ad45-129">Property</span></span>|<span data-ttu-id="3ad45-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3ad45-130">Type</span></span>|<span data-ttu-id="3ad45-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3ad45-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ad45-132">id</span><span class="sxs-lookup"><span data-stu-id="3ad45-132">id</span></span>|<span data-ttu-id="3ad45-133">String</span><span class="sxs-lookup"><span data-stu-id="3ad45-133">String</span></span>|<span data-ttu-id="3ad45-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3ad45-134">Key of the entity.</span></span> <span data-ttu-id="3ad45-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3ad45-136">displayName</span></span>|<span data-ttu-id="3ad45-137">String</span><span class="sxs-lookup"><span data-stu-id="3ad45-137">String</span></span>|<span data-ttu-id="3ad45-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="3ad45-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3ad45-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-140">description</span><span class="sxs-lookup"><span data-stu-id="3ad45-140">description</span></span>|<span data-ttu-id="3ad45-141">String</span><span class="sxs-lookup"><span data-stu-id="3ad45-141">String</span></span>|<span data-ttu-id="3ad45-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="3ad45-142">The description of the app.</span></span> <span data-ttu-id="3ad45-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-144">publisher</span><span class="sxs-lookup"><span data-stu-id="3ad45-144">publisher</span></span>|<span data-ttu-id="3ad45-145">String</span><span class="sxs-lookup"><span data-stu-id="3ad45-145">String</span></span>|<span data-ttu-id="3ad45-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="3ad45-146">The publisher of the app.</span></span> <span data-ttu-id="3ad45-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3ad45-148">largeIcon</span></span>|[<span data-ttu-id="3ad45-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3ad45-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3ad45-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="3ad45-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3ad45-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ad45-152">createdDateTime</span></span>|<span data-ttu-id="3ad45-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ad45-153">DateTimeOffset</span></span>|<span data-ttu-id="3ad45-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="3ad45-154">The date and time the app was created.</span></span> <span data-ttu-id="3ad45-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ad45-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3ad45-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ad45-157">DateTimeOffset</span></span>|<span data-ttu-id="3ad45-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="3ad45-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3ad45-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3ad45-160">isFeatured</span></span>|<span data-ttu-id="3ad45-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ad45-161">Boolean</span></span>|<span data-ttu-id="3ad45-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3ad45-163">privacyInformationUrl</span></span>|<span data-ttu-id="3ad45-164">String</span><span class="sxs-lookup"><span data-stu-id="3ad45-164">String</span></span>|<span data-ttu-id="3ad45-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3ad45-165">The privacy statement Url.</span></span> <span data-ttu-id="3ad45-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3ad45-167">informationUrl</span></span>|<span data-ttu-id="3ad45-168">String</span><span class="sxs-lookup"><span data-stu-id="3ad45-168">String</span></span>|<span data-ttu-id="3ad45-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3ad45-169">The more information Url.</span></span> <span data-ttu-id="3ad45-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-171">owner</span><span class="sxs-lookup"><span data-stu-id="3ad45-171">owner</span></span>|<span data-ttu-id="3ad45-172">String</span><span class="sxs-lookup"><span data-stu-id="3ad45-172">String</span></span>|<span data-ttu-id="3ad45-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="3ad45-173">The owner of the app.</span></span> <span data-ttu-id="3ad45-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-175">developer</span><span class="sxs-lookup"><span data-stu-id="3ad45-175">developer</span></span>|<span data-ttu-id="3ad45-176">String</span><span class="sxs-lookup"><span data-stu-id="3ad45-176">String</span></span>|<span data-ttu-id="3ad45-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="3ad45-177">The developer of the app.</span></span> <span data-ttu-id="3ad45-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-179">notes</span><span class="sxs-lookup"><span data-stu-id="3ad45-179">notes</span></span>|<span data-ttu-id="3ad45-180">String</span><span class="sxs-lookup"><span data-stu-id="3ad45-180">String</span></span>|<span data-ttu-id="3ad45-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="3ad45-181">Notes for the app.</span></span> <span data-ttu-id="3ad45-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3ad45-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="3ad45-183">publishingState</span></span>|[<span data-ttu-id="3ad45-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="3ad45-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3ad45-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="3ad45-185">The publishing state for the app.</span></span> <span data-ttu-id="3ad45-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="3ad45-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3ad45-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ad45-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3ad45-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3ad45-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3ad45-189">appUrl</span><span class="sxs-lookup"><span data-stu-id="3ad45-189">appUrl</span></span>|<span data-ttu-id="3ad45-190">String</span><span class="sxs-lookup"><span data-stu-id="3ad45-190">String</span></span>|<span data-ttu-id="3ad45-191">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="3ad45-191">The web app URL.</span></span>|
|<span data-ttu-id="3ad45-192">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="3ad45-192">useManagedBrowser</span></span>|<span data-ttu-id="3ad45-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ad45-193">Boolean</span></span>|<span data-ttu-id="3ad45-194">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="3ad45-194">Whether or not to use managed browser.</span></span> <span data-ttu-id="3ad45-195">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="3ad45-195">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="3ad45-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ad45-196">Response</span></span>
<span data-ttu-id="3ad45-197">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [webApp](../resources/intune-apps-webapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3ad45-197">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ad45-198">Пример</span><span class="sxs-lookup"><span data-stu-id="3ad45-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ad45-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ad45-199">Request</span></span>
<span data-ttu-id="3ad45-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ad45-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3ad45-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ad45-201">Response</span></span>
<span data-ttu-id="3ad45-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ad45-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









