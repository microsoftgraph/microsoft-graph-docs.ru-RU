---
title: Create webApp
description: Создание объекта webApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 16faa92f95f1175d1e317ebec365dc5ebd858819
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535144"
---
# <a name="create-webapp"></a><span data-ttu-id="59fed-103">Create webApp</span><span class="sxs-lookup"><span data-stu-id="59fed-103">Create webApp</span></span>

> <span data-ttu-id="59fed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59fed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59fed-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59fed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59fed-106">Создание объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-106">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59fed-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="59fed-107">Prerequisites</span></span>
<span data-ttu-id="59fed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59fed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59fed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59fed-110">Permission type</span></span>|<span data-ttu-id="59fed-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="59fed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59fed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59fed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59fed-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fed-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="59fed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59fed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59fed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59fed-115">Not supported.</span></span>|
|<span data-ttu-id="59fed-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="59fed-116">Application</span></span>|<span data-ttu-id="59fed-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59fed-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59fed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59fed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="59fed-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59fed-119">Request headers</span></span>
|<span data-ttu-id="59fed-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59fed-120">Header</span></span>|<span data-ttu-id="59fed-121">Значение</span><span class="sxs-lookup"><span data-stu-id="59fed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59fed-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59fed-122">Authorization</span></span>|<span data-ttu-id="59fed-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59fed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59fed-124">Accept</span><span class="sxs-lookup"><span data-stu-id="59fed-124">Accept</span></span>|<span data-ttu-id="59fed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59fed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59fed-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59fed-126">Request body</span></span>
<span data-ttu-id="59fed-127">В теле запроса добавьте представление объекта webApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59fed-127">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="59fed-128">Ниже показаны свойства, которые необходимо указывать при создании объекта webApp.</span><span class="sxs-lookup"><span data-stu-id="59fed-128">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="59fed-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="59fed-129">Property</span></span>|<span data-ttu-id="59fed-130">Тип</span><span class="sxs-lookup"><span data-stu-id="59fed-130">Type</span></span>|<span data-ttu-id="59fed-131">Описание</span><span class="sxs-lookup"><span data-stu-id="59fed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59fed-132">id</span><span class="sxs-lookup"><span data-stu-id="59fed-132">id</span></span>|<span data-ttu-id="59fed-133">Строка</span><span class="sxs-lookup"><span data-stu-id="59fed-133">String</span></span>|<span data-ttu-id="59fed-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="59fed-134">Key of the entity.</span></span> <span data-ttu-id="59fed-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-136">displayName</span><span class="sxs-lookup"><span data-stu-id="59fed-136">displayName</span></span>|<span data-ttu-id="59fed-137">Строка</span><span class="sxs-lookup"><span data-stu-id="59fed-137">String</span></span>|<span data-ttu-id="59fed-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="59fed-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="59fed-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-140">description</span><span class="sxs-lookup"><span data-stu-id="59fed-140">description</span></span>|<span data-ttu-id="59fed-141">Строка</span><span class="sxs-lookup"><span data-stu-id="59fed-141">String</span></span>|<span data-ttu-id="59fed-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="59fed-142">The description of the app.</span></span> <span data-ttu-id="59fed-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-144">publisher</span><span class="sxs-lookup"><span data-stu-id="59fed-144">publisher</span></span>|<span data-ttu-id="59fed-145">String</span><span class="sxs-lookup"><span data-stu-id="59fed-145">String</span></span>|<span data-ttu-id="59fed-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="59fed-146">The publisher of the app.</span></span> <span data-ttu-id="59fed-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="59fed-148">largeIcon</span></span>|[<span data-ttu-id="59fed-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="59fed-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="59fed-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="59fed-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="59fed-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59fed-152">createdDateTime</span></span>|<span data-ttu-id="59fed-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59fed-153">DateTimeOffset</span></span>|<span data-ttu-id="59fed-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="59fed-154">The date and time the app was created.</span></span> <span data-ttu-id="59fed-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59fed-156">lastModifiedDateTime</span></span>|<span data-ttu-id="59fed-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59fed-157">DateTimeOffset</span></span>|<span data-ttu-id="59fed-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="59fed-158">The date and time the app was last modified.</span></span> <span data-ttu-id="59fed-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="59fed-160">isFeatured</span></span>|<span data-ttu-id="59fed-161">Логический</span><span class="sxs-lookup"><span data-stu-id="59fed-161">Boolean</span></span>|<span data-ttu-id="59fed-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="59fed-163">privacyInformationUrl</span></span>|<span data-ttu-id="59fed-164">String</span><span class="sxs-lookup"><span data-stu-id="59fed-164">String</span></span>|<span data-ttu-id="59fed-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="59fed-165">The privacy statement Url.</span></span> <span data-ttu-id="59fed-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="59fed-167">informationUrl</span></span>|<span data-ttu-id="59fed-168">String</span><span class="sxs-lookup"><span data-stu-id="59fed-168">String</span></span>|<span data-ttu-id="59fed-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="59fed-169">The more information Url.</span></span> <span data-ttu-id="59fed-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-171">owner</span><span class="sxs-lookup"><span data-stu-id="59fed-171">owner</span></span>|<span data-ttu-id="59fed-172">String</span><span class="sxs-lookup"><span data-stu-id="59fed-172">String</span></span>|<span data-ttu-id="59fed-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="59fed-173">The owner of the app.</span></span> <span data-ttu-id="59fed-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-175">developer</span><span class="sxs-lookup"><span data-stu-id="59fed-175">developer</span></span>|<span data-ttu-id="59fed-176">String</span><span class="sxs-lookup"><span data-stu-id="59fed-176">String</span></span>|<span data-ttu-id="59fed-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="59fed-177">The developer of the app.</span></span> <span data-ttu-id="59fed-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-179">notes</span><span class="sxs-lookup"><span data-stu-id="59fed-179">notes</span></span>|<span data-ttu-id="59fed-180">String</span><span class="sxs-lookup"><span data-stu-id="59fed-180">String</span></span>|<span data-ttu-id="59fed-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="59fed-181">Notes for the app.</span></span> <span data-ttu-id="59fed-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="59fed-183">uploadState</span></span>|<span data-ttu-id="59fed-184">Int32</span><span class="sxs-lookup"><span data-stu-id="59fed-184">Int32</span></span>|<span data-ttu-id="59fed-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="59fed-185">The upload state.</span></span> <span data-ttu-id="59fed-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="59fed-187">publishingState</span></span>|[<span data-ttu-id="59fed-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="59fed-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="59fed-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="59fed-189">The publishing state for the app.</span></span> <span data-ttu-id="59fed-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="59fed-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="59fed-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="59fed-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="59fed-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="59fed-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="59fed-193">isAssigned</span></span>|<span data-ttu-id="59fed-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="59fed-194">Boolean</span></span>|<span data-ttu-id="59fed-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="59fed-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="59fed-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="59fed-197">roleScopeTagIds</span></span>|<span data-ttu-id="59fed-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="59fed-198">String collection</span></span>|<span data-ttu-id="59fed-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="59fed-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="59fed-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="59fed-201">dependentAppCount</span></span>|<span data-ttu-id="59fed-202">Int32</span><span class="sxs-lookup"><span data-stu-id="59fed-202">Int32</span></span>|<span data-ttu-id="59fed-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="59fed-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="59fed-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59fed-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59fed-205">appUrl</span><span class="sxs-lookup"><span data-stu-id="59fed-205">appUrl</span></span>|<span data-ttu-id="59fed-206">String</span><span class="sxs-lookup"><span data-stu-id="59fed-206">String</span></span>|<span data-ttu-id="59fed-207">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="59fed-207">The web app URL.</span></span>|
|<span data-ttu-id="59fed-208">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="59fed-208">useManagedBrowser</span></span>|<span data-ttu-id="59fed-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="59fed-209">Boolean</span></span>|<span data-ttu-id="59fed-210">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="59fed-210">Whether or not to use managed browser.</span></span> <span data-ttu-id="59fed-211">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="59fed-211">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="59fed-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="59fed-212">Response</span></span>
<span data-ttu-id="59fed-213">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [webApp](../resources/intune-apps-webapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="59fed-213">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59fed-214">Пример</span><span class="sxs-lookup"><span data-stu-id="59fed-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="59fed-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="59fed-215">Request</span></span>
<span data-ttu-id="59fed-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59fed-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 779

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="59fed-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="59fed-217">Response</span></span>
<span data-ttu-id="59fed-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59fed-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 951

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```






