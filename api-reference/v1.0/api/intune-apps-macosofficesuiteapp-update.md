---
title: Обновление объекта macOSOfficeSuiteApp
description: Обновление свойств объекта macOSOfficeSuiteApp.
ms.openlocfilehash: a7747c4b4bd4325a2a39477de9d2593bb436024b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027094"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="3b4d2-103">Обновление объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="3b4d2-103">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="3b4d2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b4d2-105">Обновление свойств объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-105">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b4d2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3b4d2-106">Prerequisites</span></span>
<span data-ttu-id="3b4d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b4d2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b4d2-109">Permission type</span></span>|<span data-ttu-id="3b4d2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b4d2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b4d2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b4d2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b4d2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b4d2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3b4d2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b4d2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b4d2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-114">Not supported.</span></span>|
|<span data-ttu-id="3b4d2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b4d2-115">Application</span></span>|<span data-ttu-id="3b4d2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b4d2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b4d2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="3b4d2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b4d2-118">Request headers</span></span>
|<span data-ttu-id="3b4d2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b4d2-119">Header</span></span>|<span data-ttu-id="3b4d2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3b4d2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b4d2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b4d2-121">Authorization</span></span>|<span data-ttu-id="3b4d2-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3b4d2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b4d2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3b4d2-123">Accept</span></span>|<span data-ttu-id="3b4d2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3b4d2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b4d2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b4d2-125">Request body</span></span>
<span data-ttu-id="3b4d2-126">В тексте запроса добавьте представление объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-126">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="3b4d2-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-127">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="3b4d2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b4d2-128">Property</span></span>|<span data-ttu-id="3b4d2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3b4d2-129">Type</span></span>|<span data-ttu-id="3b4d2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3b4d2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b4d2-131">id</span><span class="sxs-lookup"><span data-stu-id="3b4d2-131">id</span></span>|<span data-ttu-id="3b4d2-132">String</span><span class="sxs-lookup"><span data-stu-id="3b4d2-132">String</span></span>|<span data-ttu-id="3b4d2-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-133">Key of the entity.</span></span> <span data-ttu-id="3b4d2-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3b4d2-135">displayName</span></span>|<span data-ttu-id="3b4d2-136">String</span><span class="sxs-lookup"><span data-stu-id="3b4d2-136">String</span></span>|<span data-ttu-id="3b4d2-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3b4d2-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-139">описание</span><span class="sxs-lookup"><span data-stu-id="3b4d2-139">description</span></span>|<span data-ttu-id="3b4d2-140">String</span><span class="sxs-lookup"><span data-stu-id="3b4d2-140">String</span></span>|<span data-ttu-id="3b4d2-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-141">The description of the app.</span></span> <span data-ttu-id="3b4d2-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-143">publisher</span><span class="sxs-lookup"><span data-stu-id="3b4d2-143">publisher</span></span>|<span data-ttu-id="3b4d2-144">String</span><span class="sxs-lookup"><span data-stu-id="3b4d2-144">String</span></span>|<span data-ttu-id="3b4d2-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-145">The publisher of the app.</span></span> <span data-ttu-id="3b4d2-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3b4d2-147">largeIcon</span></span>|[<span data-ttu-id="3b4d2-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3b4d2-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3b4d2-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3b4d2-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b4d2-151">createdDateTime</span></span>|<span data-ttu-id="3b4d2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b4d2-152">DateTimeOffset</span></span>|<span data-ttu-id="3b4d2-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-153">The date and time the app was created.</span></span> <span data-ttu-id="3b4d2-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b4d2-155">lastModifiedDateTime</span></span>|<span data-ttu-id="3b4d2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b4d2-156">DateTimeOffset</span></span>|<span data-ttu-id="3b4d2-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-157">The date and time the app was last modified.</span></span> <span data-ttu-id="3b4d2-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3b4d2-159">isFeatured</span></span>|<span data-ttu-id="3b4d2-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b4d2-160">Boolean</span></span>|<span data-ttu-id="3b4d2-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3b4d2-162">privacyInformationUrl</span></span>|<span data-ttu-id="3b4d2-163">String</span><span class="sxs-lookup"><span data-stu-id="3b4d2-163">String</span></span>|<span data-ttu-id="3b4d2-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-164">The privacy statement Url.</span></span> <span data-ttu-id="3b4d2-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3b4d2-166">informationUrl</span></span>|<span data-ttu-id="3b4d2-167">String</span><span class="sxs-lookup"><span data-stu-id="3b4d2-167">String</span></span>|<span data-ttu-id="3b4d2-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-168">The more information Url.</span></span> <span data-ttu-id="3b4d2-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-170">owner</span><span class="sxs-lookup"><span data-stu-id="3b4d2-170">owner</span></span>|<span data-ttu-id="3b4d2-171">String</span><span class="sxs-lookup"><span data-stu-id="3b4d2-171">String</span></span>|<span data-ttu-id="3b4d2-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-172">The owner of the app.</span></span> <span data-ttu-id="3b4d2-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-174">developer</span><span class="sxs-lookup"><span data-stu-id="3b4d2-174">developer</span></span>|<span data-ttu-id="3b4d2-175">String</span><span class="sxs-lookup"><span data-stu-id="3b4d2-175">String</span></span>|<span data-ttu-id="3b4d2-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-176">The developer of the app.</span></span> <span data-ttu-id="3b4d2-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-178">notes</span><span class="sxs-lookup"><span data-stu-id="3b4d2-178">notes</span></span>|<span data-ttu-id="3b4d2-179">String</span><span class="sxs-lookup"><span data-stu-id="3b4d2-179">String</span></span>|<span data-ttu-id="3b4d2-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-180">Notes for the app.</span></span> <span data-ttu-id="3b4d2-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b4d2-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="3b4d2-182">publishingState</span></span>|[<span data-ttu-id="3b4d2-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3b4d2-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3b4d2-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-184">The publishing state for the app.</span></span> <span data-ttu-id="3b4d2-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3b4d2-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b4d2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3b4d2-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="3b4d2-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b4d2-188">Response</span></span>
<span data-ttu-id="3b4d2-189">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-189">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b4d2-190">Пример</span><span class="sxs-lookup"><span data-stu-id="3b4d2-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b4d2-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b4d2-191">Request</span></span>
<span data-ttu-id="3b4d2-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b4d2-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 584

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="3b4d2-193">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b4d2-193">Response</span></span>
<span data-ttu-id="3b4d2-p115">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3b4d2-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

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
  "publishingState": "processing"
}
```



