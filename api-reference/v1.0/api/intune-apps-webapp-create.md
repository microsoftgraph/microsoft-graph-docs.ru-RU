---
title: Create webApp
description: Создание объекта webApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5425ad08e7680fe276ebffb90399dc484b4e5372
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580610"
---
# <a name="create-webapp"></a><span data-ttu-id="d4070-103">Create webApp</span><span class="sxs-lookup"><span data-stu-id="d4070-103">Create webApp</span></span>

> <span data-ttu-id="d4070-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4070-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4070-105">Создание объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-105">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4070-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d4070-106">Prerequisites</span></span>
<span data-ttu-id="d4070-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4070-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4070-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4070-109">Permission type</span></span>|<span data-ttu-id="d4070-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4070-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4070-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4070-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4070-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4070-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d4070-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4070-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4070-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4070-114">Not supported.</span></span>|
|<span data-ttu-id="d4070-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4070-115">Application</span></span>|<span data-ttu-id="d4070-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4070-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4070-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4070-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d4070-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4070-118">Request headers</span></span>
|<span data-ttu-id="d4070-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4070-119">Header</span></span>|<span data-ttu-id="d4070-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d4070-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4070-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4070-121">Authorization</span></span>|<span data-ttu-id="d4070-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4070-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4070-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d4070-123">Accept</span></span>|<span data-ttu-id="d4070-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d4070-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4070-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4070-125">Request body</span></span>
<span data-ttu-id="d4070-126">В теле запроса добавьте представление объекта webApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4070-126">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="d4070-127">Ниже показаны свойства, которые необходимо указывать при создании объекта webApp.</span><span class="sxs-lookup"><span data-stu-id="d4070-127">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="d4070-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4070-128">Property</span></span>|<span data-ttu-id="d4070-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d4070-129">Type</span></span>|<span data-ttu-id="d4070-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d4070-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4070-131">id</span><span class="sxs-lookup"><span data-stu-id="d4070-131">id</span></span>|<span data-ttu-id="d4070-132">Строка</span><span class="sxs-lookup"><span data-stu-id="d4070-132">String</span></span>|<span data-ttu-id="d4070-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d4070-133">Key of the entity.</span></span> <span data-ttu-id="d4070-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d4070-135">displayName</span></span>|<span data-ttu-id="d4070-136">Строка</span><span class="sxs-lookup"><span data-stu-id="d4070-136">String</span></span>|<span data-ttu-id="d4070-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d4070-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d4070-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-139">description</span><span class="sxs-lookup"><span data-stu-id="d4070-139">description</span></span>|<span data-ttu-id="d4070-140">String</span><span class="sxs-lookup"><span data-stu-id="d4070-140">String</span></span>|<span data-ttu-id="d4070-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d4070-141">The description of the app.</span></span> <span data-ttu-id="d4070-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-143">publisher</span><span class="sxs-lookup"><span data-stu-id="d4070-143">publisher</span></span>|<span data-ttu-id="d4070-144">String</span><span class="sxs-lookup"><span data-stu-id="d4070-144">String</span></span>|<span data-ttu-id="d4070-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d4070-145">The publisher of the app.</span></span> <span data-ttu-id="d4070-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d4070-147">largeIcon</span></span>|[<span data-ttu-id="d4070-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d4070-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d4070-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d4070-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d4070-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4070-151">createdDateTime</span></span>|<span data-ttu-id="d4070-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4070-152">DateTimeOffset</span></span>|<span data-ttu-id="d4070-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d4070-153">The date and time the app was created.</span></span> <span data-ttu-id="d4070-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4070-155">lastModifiedDateTime</span></span>|<span data-ttu-id="d4070-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4070-156">DateTimeOffset</span></span>|<span data-ttu-id="d4070-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d4070-157">The date and time the app was last modified.</span></span> <span data-ttu-id="d4070-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d4070-159">isFeatured</span></span>|<span data-ttu-id="d4070-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4070-160">Boolean</span></span>|<span data-ttu-id="d4070-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d4070-162">privacyInformationUrl</span></span>|<span data-ttu-id="d4070-163">String</span><span class="sxs-lookup"><span data-stu-id="d4070-163">String</span></span>|<span data-ttu-id="d4070-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d4070-164">The privacy statement Url.</span></span> <span data-ttu-id="d4070-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d4070-166">informationUrl</span></span>|<span data-ttu-id="d4070-167">String</span><span class="sxs-lookup"><span data-stu-id="d4070-167">String</span></span>|<span data-ttu-id="d4070-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d4070-168">The more information Url.</span></span> <span data-ttu-id="d4070-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-170">owner</span><span class="sxs-lookup"><span data-stu-id="d4070-170">owner</span></span>|<span data-ttu-id="d4070-171">String</span><span class="sxs-lookup"><span data-stu-id="d4070-171">String</span></span>|<span data-ttu-id="d4070-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d4070-172">The owner of the app.</span></span> <span data-ttu-id="d4070-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-174">developer</span><span class="sxs-lookup"><span data-stu-id="d4070-174">developer</span></span>|<span data-ttu-id="d4070-175">String</span><span class="sxs-lookup"><span data-stu-id="d4070-175">String</span></span>|<span data-ttu-id="d4070-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d4070-176">The developer of the app.</span></span> <span data-ttu-id="d4070-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-178">notes</span><span class="sxs-lookup"><span data-stu-id="d4070-178">notes</span></span>|<span data-ttu-id="d4070-179">String</span><span class="sxs-lookup"><span data-stu-id="d4070-179">String</span></span>|<span data-ttu-id="d4070-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="d4070-180">Notes for the app.</span></span> <span data-ttu-id="d4070-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4070-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="d4070-182">publishingState</span></span>|[<span data-ttu-id="d4070-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="d4070-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d4070-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="d4070-184">The publishing state for the app.</span></span> <span data-ttu-id="d4070-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d4070-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d4070-186">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4070-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d4070-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d4070-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d4070-188">appUrl</span><span class="sxs-lookup"><span data-stu-id="d4070-188">appUrl</span></span>|<span data-ttu-id="d4070-189">String</span><span class="sxs-lookup"><span data-stu-id="d4070-189">String</span></span>|<span data-ttu-id="d4070-190">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="d4070-190">The web app URL.</span></span>|
|<span data-ttu-id="d4070-191">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="d4070-191">useManagedBrowser</span></span>|<span data-ttu-id="d4070-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4070-192">Boolean</span></span>|<span data-ttu-id="d4070-193">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="d4070-193">Whether or not to use managed browser.</span></span> <span data-ttu-id="d4070-194">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="d4070-194">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="d4070-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="d4070-195">Response</span></span>
<span data-ttu-id="d4070-196">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [webApp](../resources/intune-apps-webapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d4070-196">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4070-197">Пример</span><span class="sxs-lookup"><span data-stu-id="d4070-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4070-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4070-198">Request</span></span>
<span data-ttu-id="d4070-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4070-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4070-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4070-200">Response</span></span>
<span data-ttu-id="d4070-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4070-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



