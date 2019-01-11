---
title: Обновление объекта macOSOfficeSuiteApp
description: Обновление свойств объекта macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 545a9e6e36ec7860b3cad4f0865d59f397b64079
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813897"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="a868a-103">Обновление объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="a868a-103">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="a868a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a868a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a868a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a868a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a868a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a868a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a868a-107">Обновление свойств объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-107">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a868a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a868a-108">Prerequisites</span></span>
<span data-ttu-id="a868a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a868a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a868a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a868a-111">Permission type</span></span>|<span data-ttu-id="a868a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a868a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a868a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a868a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a868a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a868a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a868a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a868a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a868a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a868a-116">Not supported.</span></span>|
|<span data-ttu-id="a868a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a868a-117">Application</span></span>|<span data-ttu-id="a868a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a868a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a868a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a868a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a868a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a868a-120">Request headers</span></span>
|<span data-ttu-id="a868a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a868a-121">Header</span></span>|<span data-ttu-id="a868a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a868a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a868a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a868a-123">Authorization</span></span>|<span data-ttu-id="a868a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a868a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a868a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a868a-125">Accept</span></span>|<span data-ttu-id="a868a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a868a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a868a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a868a-127">Request body</span></span>
<span data-ttu-id="a868a-128">В тексте запроса добавьте представление объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a868a-128">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="a868a-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-129">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="a868a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a868a-130">Property</span></span>|<span data-ttu-id="a868a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a868a-131">Type</span></span>|<span data-ttu-id="a868a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a868a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a868a-133">id</span><span class="sxs-lookup"><span data-stu-id="a868a-133">id</span></span>|<span data-ttu-id="a868a-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a868a-134">String</span></span>|<span data-ttu-id="a868a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a868a-135">Key of the entity.</span></span> <span data-ttu-id="a868a-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a868a-137">displayName</span></span>|<span data-ttu-id="a868a-138">String</span><span class="sxs-lookup"><span data-stu-id="a868a-138">String</span></span>|<span data-ttu-id="a868a-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a868a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a868a-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-141">описание</span><span class="sxs-lookup"><span data-stu-id="a868a-141">description</span></span>|<span data-ttu-id="a868a-142">String</span><span class="sxs-lookup"><span data-stu-id="a868a-142">String</span></span>|<span data-ttu-id="a868a-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a868a-143">The description of the app.</span></span> <span data-ttu-id="a868a-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a868a-145">publisher</span></span>|<span data-ttu-id="a868a-146">String</span><span class="sxs-lookup"><span data-stu-id="a868a-146">String</span></span>|<span data-ttu-id="a868a-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a868a-147">The publisher of the app.</span></span> <span data-ttu-id="a868a-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a868a-149">largeIcon</span></span>|[<span data-ttu-id="a868a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a868a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a868a-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a868a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a868a-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a868a-153">createdDateTime</span></span>|<span data-ttu-id="a868a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a868a-154">DateTimeOffset</span></span>|<span data-ttu-id="a868a-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a868a-155">The date and time the app was created.</span></span> <span data-ttu-id="a868a-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a868a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a868a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a868a-158">DateTimeOffset</span></span>|<span data-ttu-id="a868a-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a868a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a868a-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a868a-161">isFeatured</span></span>|<span data-ttu-id="a868a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a868a-162">Boolean</span></span>|<span data-ttu-id="a868a-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a868a-164">privacyInformationUrl</span></span>|<span data-ttu-id="a868a-165">String</span><span class="sxs-lookup"><span data-stu-id="a868a-165">String</span></span>|<span data-ttu-id="a868a-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a868a-166">The privacy statement Url.</span></span> <span data-ttu-id="a868a-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a868a-168">informationUrl</span></span>|<span data-ttu-id="a868a-169">String</span><span class="sxs-lookup"><span data-stu-id="a868a-169">String</span></span>|<span data-ttu-id="a868a-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a868a-170">The more information Url.</span></span> <span data-ttu-id="a868a-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-172">owner</span><span class="sxs-lookup"><span data-stu-id="a868a-172">owner</span></span>|<span data-ttu-id="a868a-173">String</span><span class="sxs-lookup"><span data-stu-id="a868a-173">String</span></span>|<span data-ttu-id="a868a-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a868a-174">The owner of the app.</span></span> <span data-ttu-id="a868a-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-176">developer</span><span class="sxs-lookup"><span data-stu-id="a868a-176">developer</span></span>|<span data-ttu-id="a868a-177">String</span><span class="sxs-lookup"><span data-stu-id="a868a-177">String</span></span>|<span data-ttu-id="a868a-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a868a-178">The developer of the app.</span></span> <span data-ttu-id="a868a-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-180">notes</span><span class="sxs-lookup"><span data-stu-id="a868a-180">notes</span></span>|<span data-ttu-id="a868a-181">String</span><span class="sxs-lookup"><span data-stu-id="a868a-181">String</span></span>|<span data-ttu-id="a868a-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="a868a-182">Notes for the app.</span></span> <span data-ttu-id="a868a-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a868a-184">uploadState</span></span>|<span data-ttu-id="a868a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a868a-185">Int32</span></span>|<span data-ttu-id="a868a-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="a868a-186">The upload state.</span></span> <span data-ttu-id="a868a-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a868a-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="a868a-188">publishingState</span></span>|[<span data-ttu-id="a868a-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a868a-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a868a-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="a868a-190">The publishing state for the app.</span></span> <span data-ttu-id="a868a-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a868a-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a868a-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a868a-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a868a-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a868a-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="a868a-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="a868a-194">Response</span></span>
<span data-ttu-id="a868a-195">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a868a-195">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a868a-196">Пример</span><span class="sxs-lookup"><span data-stu-id="a868a-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="a868a-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="a868a-197">Request</span></span>
<span data-ttu-id="a868a-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a868a-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 612

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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="a868a-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="a868a-199">Response</span></span>
<span data-ttu-id="a868a-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a868a-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 778

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "publishingState": "processing"
}
```





