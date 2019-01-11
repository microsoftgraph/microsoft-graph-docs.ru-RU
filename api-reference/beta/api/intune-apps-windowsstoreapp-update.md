---
title: Обновление windowsStoreApp
description: Обновление свойства объекта windowsStoreApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 098af04c29e27188ef20712fe46982d09e96697f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842779"
---
# <a name="update-windowsstoreapp"></a><span data-ttu-id="014ae-103">Обновление windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="014ae-103">Update windowsStoreApp</span></span>

> <span data-ttu-id="014ae-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="014ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="014ae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="014ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="014ae-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="014ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="014ae-107">Обновление свойства объекта [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="014ae-107">Update the properties of a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="014ae-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="014ae-108">Prerequisites</span></span>
<span data-ttu-id="014ae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="014ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="014ae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="014ae-111">Permission type</span></span>|<span data-ttu-id="014ae-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="014ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="014ae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="014ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="014ae-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="014ae-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="014ae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="014ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="014ae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="014ae-116">Not supported.</span></span>|
|<span data-ttu-id="014ae-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="014ae-117">Application</span></span>|<span data-ttu-id="014ae-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="014ae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="014ae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="014ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="014ae-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="014ae-120">Request headers</span></span>
|<span data-ttu-id="014ae-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="014ae-121">Header</span></span>|<span data-ttu-id="014ae-122">Значение</span><span class="sxs-lookup"><span data-stu-id="014ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="014ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="014ae-123">Authorization</span></span>|<span data-ttu-id="014ae-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="014ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="014ae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="014ae-125">Accept</span></span>|<span data-ttu-id="014ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="014ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="014ae-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="014ae-127">Request body</span></span>
<span data-ttu-id="014ae-128">В тексте запроса укажите представление JSON для объекта [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="014ae-128">In the request body, supply a JSON representation for the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

<span data-ttu-id="014ae-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-129">The following table shows the properties that are required when you create the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span></span>

|<span data-ttu-id="014ae-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="014ae-130">Property</span></span>|<span data-ttu-id="014ae-131">Тип</span><span class="sxs-lookup"><span data-stu-id="014ae-131">Type</span></span>|<span data-ttu-id="014ae-132">Описание</span><span class="sxs-lookup"><span data-stu-id="014ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="014ae-133">id</span><span class="sxs-lookup"><span data-stu-id="014ae-133">id</span></span>|<span data-ttu-id="014ae-134">Строка</span><span class="sxs-lookup"><span data-stu-id="014ae-134">String</span></span>|<span data-ttu-id="014ae-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="014ae-135">Key of the entity.</span></span> <span data-ttu-id="014ae-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-137">displayName</span><span class="sxs-lookup"><span data-stu-id="014ae-137">displayName</span></span>|<span data-ttu-id="014ae-138">String</span><span class="sxs-lookup"><span data-stu-id="014ae-138">String</span></span>|<span data-ttu-id="014ae-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="014ae-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="014ae-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-141">описание</span><span class="sxs-lookup"><span data-stu-id="014ae-141">description</span></span>|<span data-ttu-id="014ae-142">String</span><span class="sxs-lookup"><span data-stu-id="014ae-142">String</span></span>|<span data-ttu-id="014ae-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="014ae-143">The description of the app.</span></span> <span data-ttu-id="014ae-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-145">publisher</span><span class="sxs-lookup"><span data-stu-id="014ae-145">publisher</span></span>|<span data-ttu-id="014ae-146">String</span><span class="sxs-lookup"><span data-stu-id="014ae-146">String</span></span>|<span data-ttu-id="014ae-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="014ae-147">The publisher of the app.</span></span> <span data-ttu-id="014ae-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="014ae-149">largeIcon</span></span>|[<span data-ttu-id="014ae-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="014ae-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="014ae-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="014ae-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="014ae-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="014ae-153">createdDateTime</span></span>|<span data-ttu-id="014ae-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="014ae-154">DateTimeOffset</span></span>|<span data-ttu-id="014ae-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="014ae-155">The date and time the app was created.</span></span> <span data-ttu-id="014ae-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="014ae-157">lastModifiedDateTime</span></span>|<span data-ttu-id="014ae-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="014ae-158">DateTimeOffset</span></span>|<span data-ttu-id="014ae-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="014ae-159">The date and time the app was last modified.</span></span> <span data-ttu-id="014ae-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="014ae-161">isFeatured</span></span>|<span data-ttu-id="014ae-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="014ae-162">Boolean</span></span>|<span data-ttu-id="014ae-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="014ae-164">privacyInformationUrl</span></span>|<span data-ttu-id="014ae-165">String</span><span class="sxs-lookup"><span data-stu-id="014ae-165">String</span></span>|<span data-ttu-id="014ae-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="014ae-166">The privacy statement Url.</span></span> <span data-ttu-id="014ae-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="014ae-168">informationUrl</span></span>|<span data-ttu-id="014ae-169">String</span><span class="sxs-lookup"><span data-stu-id="014ae-169">String</span></span>|<span data-ttu-id="014ae-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="014ae-170">The more information Url.</span></span> <span data-ttu-id="014ae-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-172">owner</span><span class="sxs-lookup"><span data-stu-id="014ae-172">owner</span></span>|<span data-ttu-id="014ae-173">String</span><span class="sxs-lookup"><span data-stu-id="014ae-173">String</span></span>|<span data-ttu-id="014ae-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="014ae-174">The owner of the app.</span></span> <span data-ttu-id="014ae-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-176">developer</span><span class="sxs-lookup"><span data-stu-id="014ae-176">developer</span></span>|<span data-ttu-id="014ae-177">String</span><span class="sxs-lookup"><span data-stu-id="014ae-177">String</span></span>|<span data-ttu-id="014ae-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="014ae-178">The developer of the app.</span></span> <span data-ttu-id="014ae-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-180">notes</span><span class="sxs-lookup"><span data-stu-id="014ae-180">notes</span></span>|<span data-ttu-id="014ae-181">String</span><span class="sxs-lookup"><span data-stu-id="014ae-181">String</span></span>|<span data-ttu-id="014ae-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="014ae-182">Notes for the app.</span></span> <span data-ttu-id="014ae-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="014ae-184">uploadState</span></span>|<span data-ttu-id="014ae-185">Int32</span><span class="sxs-lookup"><span data-stu-id="014ae-185">Int32</span></span>|<span data-ttu-id="014ae-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="014ae-186">The upload state.</span></span> <span data-ttu-id="014ae-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="014ae-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="014ae-188">publishingState</span></span>|[<span data-ttu-id="014ae-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="014ae-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="014ae-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="014ae-190">The publishing state for the app.</span></span> <span data-ttu-id="014ae-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="014ae-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="014ae-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014ae-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="014ae-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="014ae-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="014ae-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="014ae-194">appStoreUrl</span></span>|<span data-ttu-id="014ae-195">String</span><span class="sxs-lookup"><span data-stu-id="014ae-195">String</span></span>|<span data-ttu-id="014ae-196">Windows store URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="014ae-196">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="014ae-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="014ae-197">Response</span></span>
<span data-ttu-id="014ae-198">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="014ae-198">If successful, this method returns a `200 OK` response code and an updated [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="014ae-199">Пример</span><span class="sxs-lookup"><span data-stu-id="014ae-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="014ae-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="014ae-200">Request</span></span>
<span data-ttu-id="014ae-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="014ae-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 666

{
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="014ae-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="014ae-202">Response</span></span>
<span data-ttu-id="014ae-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="014ae-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 828

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
  "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





