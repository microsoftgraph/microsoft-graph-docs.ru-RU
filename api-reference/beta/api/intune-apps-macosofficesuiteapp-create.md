---
title: Создание объекта macOSOfficeSuiteApp
description: Создание объекта macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f82ebbaa3b7a5936d45f36a56a929eb6472600a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824138"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="00484-103">Создание объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="00484-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="00484-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="00484-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00484-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00484-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00484-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00484-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00484-107">Создание объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-107">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00484-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="00484-108">Prerequisites</span></span>
<span data-ttu-id="00484-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00484-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00484-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00484-111">Permission type</span></span>|<span data-ttu-id="00484-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00484-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00484-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00484-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00484-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00484-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="00484-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00484-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00484-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00484-116">Not supported.</span></span>|
|<span data-ttu-id="00484-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00484-117">Application</span></span>|<span data-ttu-id="00484-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00484-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00484-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00484-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="00484-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00484-120">Request headers</span></span>
|<span data-ttu-id="00484-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00484-121">Header</span></span>|<span data-ttu-id="00484-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00484-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00484-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00484-123">Authorization</span></span>|<span data-ttu-id="00484-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="00484-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00484-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00484-125">Accept</span></span>|<span data-ttu-id="00484-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00484-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00484-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00484-127">Request body</span></span>
<span data-ttu-id="00484-128">В тексте запроса добавьте представление объекта macOSOfficeSuiteApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00484-128">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="00484-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="00484-129">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="00484-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="00484-130">Property</span></span>|<span data-ttu-id="00484-131">Тип</span><span class="sxs-lookup"><span data-stu-id="00484-131">Type</span></span>|<span data-ttu-id="00484-132">Описание</span><span class="sxs-lookup"><span data-stu-id="00484-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00484-133">id</span><span class="sxs-lookup"><span data-stu-id="00484-133">id</span></span>|<span data-ttu-id="00484-134">Строка</span><span class="sxs-lookup"><span data-stu-id="00484-134">String</span></span>|<span data-ttu-id="00484-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="00484-135">Key of the entity.</span></span> <span data-ttu-id="00484-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-137">displayName</span><span class="sxs-lookup"><span data-stu-id="00484-137">displayName</span></span>|<span data-ttu-id="00484-138">String</span><span class="sxs-lookup"><span data-stu-id="00484-138">String</span></span>|<span data-ttu-id="00484-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="00484-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="00484-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-141">описание</span><span class="sxs-lookup"><span data-stu-id="00484-141">description</span></span>|<span data-ttu-id="00484-142">String</span><span class="sxs-lookup"><span data-stu-id="00484-142">String</span></span>|<span data-ttu-id="00484-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="00484-143">The description of the app.</span></span> <span data-ttu-id="00484-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-145">publisher</span><span class="sxs-lookup"><span data-stu-id="00484-145">publisher</span></span>|<span data-ttu-id="00484-146">String</span><span class="sxs-lookup"><span data-stu-id="00484-146">String</span></span>|<span data-ttu-id="00484-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="00484-147">The publisher of the app.</span></span> <span data-ttu-id="00484-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="00484-149">largeIcon</span></span>|[<span data-ttu-id="00484-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="00484-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="00484-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="00484-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="00484-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00484-153">createdDateTime</span></span>|<span data-ttu-id="00484-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00484-154">DateTimeOffset</span></span>|<span data-ttu-id="00484-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="00484-155">The date and time the app was created.</span></span> <span data-ttu-id="00484-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00484-157">lastModifiedDateTime</span></span>|<span data-ttu-id="00484-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00484-158">DateTimeOffset</span></span>|<span data-ttu-id="00484-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="00484-159">The date and time the app was last modified.</span></span> <span data-ttu-id="00484-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="00484-161">isFeatured</span></span>|<span data-ttu-id="00484-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="00484-162">Boolean</span></span>|<span data-ttu-id="00484-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="00484-164">privacyInformationUrl</span></span>|<span data-ttu-id="00484-165">String</span><span class="sxs-lookup"><span data-stu-id="00484-165">String</span></span>|<span data-ttu-id="00484-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="00484-166">The privacy statement Url.</span></span> <span data-ttu-id="00484-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="00484-168">informationUrl</span></span>|<span data-ttu-id="00484-169">String</span><span class="sxs-lookup"><span data-stu-id="00484-169">String</span></span>|<span data-ttu-id="00484-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="00484-170">The more information Url.</span></span> <span data-ttu-id="00484-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-172">owner</span><span class="sxs-lookup"><span data-stu-id="00484-172">owner</span></span>|<span data-ttu-id="00484-173">String</span><span class="sxs-lookup"><span data-stu-id="00484-173">String</span></span>|<span data-ttu-id="00484-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="00484-174">The owner of the app.</span></span> <span data-ttu-id="00484-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-176">developer</span><span class="sxs-lookup"><span data-stu-id="00484-176">developer</span></span>|<span data-ttu-id="00484-177">String</span><span class="sxs-lookup"><span data-stu-id="00484-177">String</span></span>|<span data-ttu-id="00484-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="00484-178">The developer of the app.</span></span> <span data-ttu-id="00484-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-180">notes</span><span class="sxs-lookup"><span data-stu-id="00484-180">notes</span></span>|<span data-ttu-id="00484-181">String</span><span class="sxs-lookup"><span data-stu-id="00484-181">String</span></span>|<span data-ttu-id="00484-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="00484-182">Notes for the app.</span></span> <span data-ttu-id="00484-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="00484-184">uploadState</span></span>|<span data-ttu-id="00484-185">Int32</span><span class="sxs-lookup"><span data-stu-id="00484-185">Int32</span></span>|<span data-ttu-id="00484-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="00484-186">The upload state.</span></span> <span data-ttu-id="00484-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="00484-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="00484-188">publishingState</span></span>|[<span data-ttu-id="00484-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="00484-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="00484-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="00484-190">The publishing state for the app.</span></span> <span data-ttu-id="00484-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="00484-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="00484-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="00484-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="00484-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="00484-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="00484-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="00484-194">Response</span></span>
<span data-ttu-id="00484-195">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00484-195">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00484-196">Пример</span><span class="sxs-lookup"><span data-stu-id="00484-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="00484-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="00484-197">Request</span></span>
<span data-ttu-id="00484-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00484-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 670

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

### <a name="response"></a><span data-ttu-id="00484-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="00484-199">Response</span></span>
<span data-ttu-id="00484-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="00484-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





