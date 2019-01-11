---
title: Создание windowsPhone81StoreApp
description: Создание нового объекта windowsPhone81StoreApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e17b119bd29cb59080c05b3b1c8bc6547a2694c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864570"
---
# <a name="create-windowsphone81storeapp"></a><span data-ttu-id="71fba-103">Создание windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="71fba-103">Create windowsPhone81StoreApp</span></span>

> <span data-ttu-id="71fba-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71fba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71fba-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71fba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71fba-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="71fba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71fba-107">Создание нового объекта [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="71fba-107">Create a new [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71fba-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="71fba-108">Prerequisites</span></span>
<span data-ttu-id="71fba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71fba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71fba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71fba-111">Permission type</span></span>|<span data-ttu-id="71fba-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71fba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71fba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71fba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71fba-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71fba-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="71fba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71fba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71fba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71fba-116">Not supported.</span></span>|
|<span data-ttu-id="71fba-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71fba-117">Application</span></span>|<span data-ttu-id="71fba-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71fba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71fba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71fba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="71fba-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71fba-120">Request headers</span></span>
|<span data-ttu-id="71fba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71fba-121">Header</span></span>|<span data-ttu-id="71fba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71fba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71fba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71fba-123">Authorization</span></span>|<span data-ttu-id="71fba-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="71fba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71fba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71fba-125">Accept</span></span>|<span data-ttu-id="71fba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71fba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71fba-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="71fba-127">Request body</span></span>
<span data-ttu-id="71fba-128">В тексте запроса укажите представление JSON для объекта windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="71fba-128">In the request body, supply a JSON representation for the windowsPhone81StoreApp object.</span></span>

<span data-ttu-id="71fba-129">В следующей таблице показаны свойства, которые необходимы для создания windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="71fba-129">The following table shows the properties that are required when you create the windowsPhone81StoreApp.</span></span>

|<span data-ttu-id="71fba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="71fba-130">Property</span></span>|<span data-ttu-id="71fba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="71fba-131">Type</span></span>|<span data-ttu-id="71fba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="71fba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71fba-133">id</span><span class="sxs-lookup"><span data-stu-id="71fba-133">id</span></span>|<span data-ttu-id="71fba-134">Строка</span><span class="sxs-lookup"><span data-stu-id="71fba-134">String</span></span>|<span data-ttu-id="71fba-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="71fba-135">Key of the entity.</span></span> <span data-ttu-id="71fba-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-137">displayName</span><span class="sxs-lookup"><span data-stu-id="71fba-137">displayName</span></span>|<span data-ttu-id="71fba-138">String</span><span class="sxs-lookup"><span data-stu-id="71fba-138">String</span></span>|<span data-ttu-id="71fba-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="71fba-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="71fba-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-141">описание</span><span class="sxs-lookup"><span data-stu-id="71fba-141">description</span></span>|<span data-ttu-id="71fba-142">String</span><span class="sxs-lookup"><span data-stu-id="71fba-142">String</span></span>|<span data-ttu-id="71fba-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="71fba-143">The description of the app.</span></span> <span data-ttu-id="71fba-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-145">publisher</span><span class="sxs-lookup"><span data-stu-id="71fba-145">publisher</span></span>|<span data-ttu-id="71fba-146">String</span><span class="sxs-lookup"><span data-stu-id="71fba-146">String</span></span>|<span data-ttu-id="71fba-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="71fba-147">The publisher of the app.</span></span> <span data-ttu-id="71fba-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="71fba-149">largeIcon</span></span>|[<span data-ttu-id="71fba-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="71fba-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="71fba-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="71fba-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="71fba-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71fba-153">createdDateTime</span></span>|<span data-ttu-id="71fba-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71fba-154">DateTimeOffset</span></span>|<span data-ttu-id="71fba-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="71fba-155">The date and time the app was created.</span></span> <span data-ttu-id="71fba-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71fba-157">lastModifiedDateTime</span></span>|<span data-ttu-id="71fba-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71fba-158">DateTimeOffset</span></span>|<span data-ttu-id="71fba-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="71fba-159">The date and time the app was last modified.</span></span> <span data-ttu-id="71fba-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="71fba-161">isFeatured</span></span>|<span data-ttu-id="71fba-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="71fba-162">Boolean</span></span>|<span data-ttu-id="71fba-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="71fba-164">privacyInformationUrl</span></span>|<span data-ttu-id="71fba-165">String</span><span class="sxs-lookup"><span data-stu-id="71fba-165">String</span></span>|<span data-ttu-id="71fba-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="71fba-166">The privacy statement Url.</span></span> <span data-ttu-id="71fba-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="71fba-168">informationUrl</span></span>|<span data-ttu-id="71fba-169">String</span><span class="sxs-lookup"><span data-stu-id="71fba-169">String</span></span>|<span data-ttu-id="71fba-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="71fba-170">The more information Url.</span></span> <span data-ttu-id="71fba-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-172">owner</span><span class="sxs-lookup"><span data-stu-id="71fba-172">owner</span></span>|<span data-ttu-id="71fba-173">String</span><span class="sxs-lookup"><span data-stu-id="71fba-173">String</span></span>|<span data-ttu-id="71fba-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="71fba-174">The owner of the app.</span></span> <span data-ttu-id="71fba-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-176">developer</span><span class="sxs-lookup"><span data-stu-id="71fba-176">developer</span></span>|<span data-ttu-id="71fba-177">String</span><span class="sxs-lookup"><span data-stu-id="71fba-177">String</span></span>|<span data-ttu-id="71fba-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="71fba-178">The developer of the app.</span></span> <span data-ttu-id="71fba-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-180">notes</span><span class="sxs-lookup"><span data-stu-id="71fba-180">notes</span></span>|<span data-ttu-id="71fba-181">String</span><span class="sxs-lookup"><span data-stu-id="71fba-181">String</span></span>|<span data-ttu-id="71fba-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="71fba-182">Notes for the app.</span></span> <span data-ttu-id="71fba-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="71fba-184">uploadState</span></span>|<span data-ttu-id="71fba-185">Int32</span><span class="sxs-lookup"><span data-stu-id="71fba-185">Int32</span></span>|<span data-ttu-id="71fba-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="71fba-186">The upload state.</span></span> <span data-ttu-id="71fba-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fba-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="71fba-188">publishingState</span></span>|[<span data-ttu-id="71fba-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="71fba-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="71fba-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="71fba-190">The publishing state for the app.</span></span> <span data-ttu-id="71fba-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="71fba-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="71fba-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fba-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="71fba-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="71fba-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="71fba-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="71fba-194">appStoreUrl</span></span>|<span data-ttu-id="71fba-195">String</span><span class="sxs-lookup"><span data-stu-id="71fba-195">String</span></span>|<span data-ttu-id="71fba-196">Windows Phone 8.1 хранилища URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="71fba-196">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="71fba-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="71fba-197">Response</span></span>
<span data-ttu-id="71fba-198">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="71fba-198">If successful, this method returns a `201 Created` response code and a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71fba-199">Пример</span><span class="sxs-lookup"><span data-stu-id="71fba-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="71fba-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="71fba-200">Request</span></span>
<span data-ttu-id="71fba-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71fba-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 727

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
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

### <a name="response"></a><span data-ttu-id="71fba-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="71fba-202">Response</span></span>
<span data-ttu-id="71fba-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="71fba-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 835

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
  "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
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





