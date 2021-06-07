---
title: Update webApp
description: Обновление свойств объекта webApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 798eb1c5388e75a7fa63b9f8ad79558e439c4885
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750317"
---
# <a name="update-webapp"></a><span data-ttu-id="79647-103">Update webApp</span><span class="sxs-lookup"><span data-stu-id="79647-103">Update webApp</span></span>

<span data-ttu-id="79647-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79647-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79647-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79647-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79647-106">Обновление свойств объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-106">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79647-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="79647-107">Prerequisites</span></span>
<span data-ttu-id="79647-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79647-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79647-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79647-110">Permission type</span></span>|<span data-ttu-id="79647-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79647-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79647-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79647-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79647-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79647-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79647-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79647-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79647-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79647-115">Not supported.</span></span>|
|<span data-ttu-id="79647-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="79647-116">Application</span></span>|<span data-ttu-id="79647-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79647-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79647-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79647-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="79647-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="79647-119">Request headers</span></span>
|<span data-ttu-id="79647-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="79647-120">Header</span></span>|<span data-ttu-id="79647-121">Значение</span><span class="sxs-lookup"><span data-stu-id="79647-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79647-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79647-122">Authorization</span></span>|<span data-ttu-id="79647-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79647-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79647-124">Accept</span><span class="sxs-lookup"><span data-stu-id="79647-124">Accept</span></span>|<span data-ttu-id="79647-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79647-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79647-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79647-126">Request body</span></span>
<span data-ttu-id="79647-127">В тексте запроса добавьте представление объекта [webApp](../resources/intune-apps-webapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79647-127">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="79647-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-128">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="79647-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="79647-129">Property</span></span>|<span data-ttu-id="79647-130">Тип</span><span class="sxs-lookup"><span data-stu-id="79647-130">Type</span></span>|<span data-ttu-id="79647-131">Описание</span><span class="sxs-lookup"><span data-stu-id="79647-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79647-132">id</span><span class="sxs-lookup"><span data-stu-id="79647-132">id</span></span>|<span data-ttu-id="79647-133">String</span><span class="sxs-lookup"><span data-stu-id="79647-133">String</span></span>|<span data-ttu-id="79647-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="79647-134">Key of the entity.</span></span> <span data-ttu-id="79647-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-136">displayName</span><span class="sxs-lookup"><span data-stu-id="79647-136">displayName</span></span>|<span data-ttu-id="79647-137">String</span><span class="sxs-lookup"><span data-stu-id="79647-137">String</span></span>|<span data-ttu-id="79647-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="79647-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="79647-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-140">description</span><span class="sxs-lookup"><span data-stu-id="79647-140">description</span></span>|<span data-ttu-id="79647-141">String</span><span class="sxs-lookup"><span data-stu-id="79647-141">String</span></span>|<span data-ttu-id="79647-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="79647-142">The description of the app.</span></span> <span data-ttu-id="79647-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-144">publisher</span><span class="sxs-lookup"><span data-stu-id="79647-144">publisher</span></span>|<span data-ttu-id="79647-145">String</span><span class="sxs-lookup"><span data-stu-id="79647-145">String</span></span>|<span data-ttu-id="79647-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="79647-146">The publisher of the app.</span></span> <span data-ttu-id="79647-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="79647-148">largeIcon</span></span>|[<span data-ttu-id="79647-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="79647-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="79647-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="79647-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="79647-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79647-152">createdDateTime</span></span>|<span data-ttu-id="79647-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79647-153">DateTimeOffset</span></span>|<span data-ttu-id="79647-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="79647-154">The date and time the app was created.</span></span> <span data-ttu-id="79647-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79647-156">lastModifiedDateTime</span></span>|<span data-ttu-id="79647-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79647-157">DateTimeOffset</span></span>|<span data-ttu-id="79647-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="79647-158">The date and time the app was last modified.</span></span> <span data-ttu-id="79647-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="79647-160">isFeatured</span></span>|<span data-ttu-id="79647-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="79647-161">Boolean</span></span>|<span data-ttu-id="79647-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="79647-163">privacyInformationUrl</span></span>|<span data-ttu-id="79647-164">String</span><span class="sxs-lookup"><span data-stu-id="79647-164">String</span></span>|<span data-ttu-id="79647-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="79647-165">The privacy statement Url.</span></span> <span data-ttu-id="79647-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="79647-167">informationUrl</span></span>|<span data-ttu-id="79647-168">String</span><span class="sxs-lookup"><span data-stu-id="79647-168">String</span></span>|<span data-ttu-id="79647-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="79647-169">The more information Url.</span></span> <span data-ttu-id="79647-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-171">owner</span><span class="sxs-lookup"><span data-stu-id="79647-171">owner</span></span>|<span data-ttu-id="79647-172">String</span><span class="sxs-lookup"><span data-stu-id="79647-172">String</span></span>|<span data-ttu-id="79647-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="79647-173">The owner of the app.</span></span> <span data-ttu-id="79647-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-175">developer</span><span class="sxs-lookup"><span data-stu-id="79647-175">developer</span></span>|<span data-ttu-id="79647-176">String</span><span class="sxs-lookup"><span data-stu-id="79647-176">String</span></span>|<span data-ttu-id="79647-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="79647-177">The developer of the app.</span></span> <span data-ttu-id="79647-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-179">notes</span><span class="sxs-lookup"><span data-stu-id="79647-179">notes</span></span>|<span data-ttu-id="79647-180">String</span><span class="sxs-lookup"><span data-stu-id="79647-180">String</span></span>|<span data-ttu-id="79647-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="79647-181">Notes for the app.</span></span> <span data-ttu-id="79647-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79647-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="79647-183">publishingState</span></span>|[<span data-ttu-id="79647-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="79647-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="79647-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="79647-185">The publishing state for the app.</span></span> <span data-ttu-id="79647-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="79647-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="79647-187">Унаследованный от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="79647-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="79647-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="79647-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="79647-189">appUrl</span><span class="sxs-lookup"><span data-stu-id="79647-189">appUrl</span></span>|<span data-ttu-id="79647-190">String</span><span class="sxs-lookup"><span data-stu-id="79647-190">String</span></span>|<span data-ttu-id="79647-191">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="79647-191">The web app URL.</span></span> <span data-ttu-id="79647-192">Это свойство не может быть PATCHed.</span><span class="sxs-lookup"><span data-stu-id="79647-192">This property cannot be PATCHed.</span></span>|
|<span data-ttu-id="79647-193">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="79647-193">useManagedBrowser</span></span>|<span data-ttu-id="79647-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="79647-194">Boolean</span></span>|<span data-ttu-id="79647-195">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="79647-195">Whether or not to use managed browser.</span></span> <span data-ttu-id="79647-196">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="79647-196">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="79647-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="79647-197">Response</span></span>
<span data-ttu-id="79647-198">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [webApp](../resources/intune-apps-webapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="79647-198">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79647-199">Пример</span><span class="sxs-lookup"><span data-stu-id="79647-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="79647-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="79647-200">Request</span></span>
<span data-ttu-id="79647-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79647-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="79647-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="79647-202">Response</span></span>
<span data-ttu-id="79647-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79647-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




