---
title: Создание windowsStoreApp
description: Создание нового объекта windowsStoreApp.
author: tfitzmac
ms.openlocfilehash: 0640975c41aa8ad12abf481ae37c6770976f321a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356639"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="9688c-103">Создание windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="9688c-103">Create windowsStoreApp</span></span>

> <span data-ttu-id="9688c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9688c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9688c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9688c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9688c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9688c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9688c-107">Создание нового объекта [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9688c-107">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9688c-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9688c-108">Prerequisites</span></span>
<span data-ttu-id="9688c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9688c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9688c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9688c-111">Permission type</span></span>|<span data-ttu-id="9688c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9688c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9688c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9688c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9688c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9688c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9688c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9688c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9688c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9688c-116">Not supported.</span></span>|
|<span data-ttu-id="9688c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9688c-117">Application</span></span>|<span data-ttu-id="9688c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9688c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9688c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9688c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9688c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9688c-120">Request headers</span></span>
|<span data-ttu-id="9688c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9688c-121">Header</span></span>|<span data-ttu-id="9688c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9688c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9688c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9688c-123">Authorization</span></span>|<span data-ttu-id="9688c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9688c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9688c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9688c-125">Accept</span></span>|<span data-ttu-id="9688c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9688c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9688c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9688c-127">Request body</span></span>
<span data-ttu-id="9688c-128">В тексте запроса укажите представление JSON для объекта windowsStoreApp.</span><span class="sxs-lookup"><span data-stu-id="9688c-128">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="9688c-129">В следующей таблице показаны свойства, которые необходимы для создания windowsStoreApp.</span><span class="sxs-lookup"><span data-stu-id="9688c-129">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="9688c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9688c-130">Property</span></span>|<span data-ttu-id="9688c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9688c-131">Type</span></span>|<span data-ttu-id="9688c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9688c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9688c-133">id</span><span class="sxs-lookup"><span data-stu-id="9688c-133">id</span></span>|<span data-ttu-id="9688c-134">String</span><span class="sxs-lookup"><span data-stu-id="9688c-134">String</span></span>|<span data-ttu-id="9688c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9688c-135">Key of the entity.</span></span> <span data-ttu-id="9688c-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9688c-137">displayName</span></span>|<span data-ttu-id="9688c-138">String</span><span class="sxs-lookup"><span data-stu-id="9688c-138">String</span></span>|<span data-ttu-id="9688c-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9688c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9688c-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-141">описание</span><span class="sxs-lookup"><span data-stu-id="9688c-141">description</span></span>|<span data-ttu-id="9688c-142">String</span><span class="sxs-lookup"><span data-stu-id="9688c-142">String</span></span>|<span data-ttu-id="9688c-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9688c-143">The description of the app.</span></span> <span data-ttu-id="9688c-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-145">publisher</span><span class="sxs-lookup"><span data-stu-id="9688c-145">publisher</span></span>|<span data-ttu-id="9688c-146">String</span><span class="sxs-lookup"><span data-stu-id="9688c-146">String</span></span>|<span data-ttu-id="9688c-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9688c-147">The publisher of the app.</span></span> <span data-ttu-id="9688c-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9688c-149">largeIcon</span></span>|[<span data-ttu-id="9688c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9688c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9688c-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9688c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9688c-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9688c-153">createdDateTime</span></span>|<span data-ttu-id="9688c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9688c-154">DateTimeOffset</span></span>|<span data-ttu-id="9688c-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9688c-155">The date and time the app was created.</span></span> <span data-ttu-id="9688c-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9688c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9688c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9688c-158">DateTimeOffset</span></span>|<span data-ttu-id="9688c-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9688c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9688c-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9688c-161">isFeatured</span></span>|<span data-ttu-id="9688c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9688c-162">Boolean</span></span>|<span data-ttu-id="9688c-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9688c-164">privacyInformationUrl</span></span>|<span data-ttu-id="9688c-165">String</span><span class="sxs-lookup"><span data-stu-id="9688c-165">String</span></span>|<span data-ttu-id="9688c-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9688c-166">The privacy statement Url.</span></span> <span data-ttu-id="9688c-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9688c-168">informationUrl</span></span>|<span data-ttu-id="9688c-169">String</span><span class="sxs-lookup"><span data-stu-id="9688c-169">String</span></span>|<span data-ttu-id="9688c-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9688c-170">The more information Url.</span></span> <span data-ttu-id="9688c-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-172">owner</span><span class="sxs-lookup"><span data-stu-id="9688c-172">owner</span></span>|<span data-ttu-id="9688c-173">String</span><span class="sxs-lookup"><span data-stu-id="9688c-173">String</span></span>|<span data-ttu-id="9688c-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9688c-174">The owner of the app.</span></span> <span data-ttu-id="9688c-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-176">developer</span><span class="sxs-lookup"><span data-stu-id="9688c-176">developer</span></span>|<span data-ttu-id="9688c-177">String</span><span class="sxs-lookup"><span data-stu-id="9688c-177">String</span></span>|<span data-ttu-id="9688c-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9688c-178">The developer of the app.</span></span> <span data-ttu-id="9688c-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-180">notes</span><span class="sxs-lookup"><span data-stu-id="9688c-180">notes</span></span>|<span data-ttu-id="9688c-181">String</span><span class="sxs-lookup"><span data-stu-id="9688c-181">String</span></span>|<span data-ttu-id="9688c-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="9688c-182">Notes for the app.</span></span> <span data-ttu-id="9688c-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9688c-184">uploadState</span></span>|<span data-ttu-id="9688c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9688c-185">Int32</span></span>|<span data-ttu-id="9688c-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="9688c-186">The upload state.</span></span> <span data-ttu-id="9688c-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9688c-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="9688c-188">publishingState</span></span>|[<span data-ttu-id="9688c-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9688c-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9688c-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="9688c-190">The publishing state for the app.</span></span> <span data-ttu-id="9688c-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9688c-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9688c-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9688c-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9688c-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9688c-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9688c-194">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9688c-194">appStoreUrl</span></span>|<span data-ttu-id="9688c-195">String</span><span class="sxs-lookup"><span data-stu-id="9688c-195">String</span></span>|<span data-ttu-id="9688c-196">Windows store URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="9688c-196">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="9688c-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="9688c-197">Response</span></span>
<span data-ttu-id="9688c-198">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9688c-198">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9688c-199">Пример</span><span class="sxs-lookup"><span data-stu-id="9688c-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="9688c-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="9688c-200">Request</span></span>
<span data-ttu-id="9688c-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9688c-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 720

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
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

### <a name="response"></a><span data-ttu-id="9688c-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="9688c-202">Response</span></span>
<span data-ttu-id="9688c-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9688c-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





