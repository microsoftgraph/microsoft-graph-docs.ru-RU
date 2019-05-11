---
title: Создание windowsPhone81StoreApp
description: Создание нового объекта windowsPhone81StoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c38ca7ea2f6e974dffad06855be2b25688fb2c7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934581"
---
# <a name="create-windowsphone81storeapp"></a><span data-ttu-id="426cb-103">Создание windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="426cb-103">Create windowsPhone81StoreApp</span></span>

> <span data-ttu-id="426cb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="426cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="426cb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="426cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="426cb-106">Создание нового объекта [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="426cb-106">Create a new [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="426cb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="426cb-107">Prerequisites</span></span>
<span data-ttu-id="426cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="426cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="426cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="426cb-110">Permission type</span></span>|<span data-ttu-id="426cb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="426cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="426cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="426cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="426cb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="426cb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="426cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="426cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="426cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="426cb-115">Not supported.</span></span>|
|<span data-ttu-id="426cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="426cb-116">Application</span></span>|<span data-ttu-id="426cb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="426cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="426cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="426cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="426cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="426cb-119">Request headers</span></span>
|<span data-ttu-id="426cb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="426cb-120">Header</span></span>|<span data-ttu-id="426cb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="426cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="426cb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="426cb-122">Authorization</span></span>|<span data-ttu-id="426cb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="426cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="426cb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="426cb-124">Accept</span></span>|<span data-ttu-id="426cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="426cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="426cb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="426cb-126">Request body</span></span>
<span data-ttu-id="426cb-127">В тексте запроса добавьте представление объекта windowsPhone81StoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="426cb-127">In the request body, supply a JSON representation for the windowsPhone81StoreApp object.</span></span>

<span data-ttu-id="426cb-128">В следующей таблице приведены свойства, необходимые при создании windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="426cb-128">The following table shows the properties that are required when you create the windowsPhone81StoreApp.</span></span>

|<span data-ttu-id="426cb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="426cb-129">Property</span></span>|<span data-ttu-id="426cb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="426cb-130">Type</span></span>|<span data-ttu-id="426cb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="426cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="426cb-132">id</span><span class="sxs-lookup"><span data-stu-id="426cb-132">id</span></span>|<span data-ttu-id="426cb-133">Строка</span><span class="sxs-lookup"><span data-stu-id="426cb-133">String</span></span>|<span data-ttu-id="426cb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="426cb-134">Key of the entity.</span></span> <span data-ttu-id="426cb-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="426cb-136">displayName</span></span>|<span data-ttu-id="426cb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="426cb-137">String</span></span>|<span data-ttu-id="426cb-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="426cb-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="426cb-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-140">description</span><span class="sxs-lookup"><span data-stu-id="426cb-140">description</span></span>|<span data-ttu-id="426cb-141">Строка</span><span class="sxs-lookup"><span data-stu-id="426cb-141">String</span></span>|<span data-ttu-id="426cb-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="426cb-142">The description of the app.</span></span> <span data-ttu-id="426cb-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-144">publisher</span><span class="sxs-lookup"><span data-stu-id="426cb-144">publisher</span></span>|<span data-ttu-id="426cb-145">Строка</span><span class="sxs-lookup"><span data-stu-id="426cb-145">String</span></span>|<span data-ttu-id="426cb-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="426cb-146">The publisher of the app.</span></span> <span data-ttu-id="426cb-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="426cb-148">largeIcon</span></span>|[<span data-ttu-id="426cb-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="426cb-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="426cb-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="426cb-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="426cb-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="426cb-152">createdDateTime</span></span>|<span data-ttu-id="426cb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="426cb-153">DateTimeOffset</span></span>|<span data-ttu-id="426cb-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="426cb-154">The date and time the app was created.</span></span> <span data-ttu-id="426cb-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="426cb-156">lastModifiedDateTime</span></span>|<span data-ttu-id="426cb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="426cb-157">DateTimeOffset</span></span>|<span data-ttu-id="426cb-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="426cb-158">The date and time the app was last modified.</span></span> <span data-ttu-id="426cb-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="426cb-160">isFeatured</span></span>|<span data-ttu-id="426cb-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="426cb-161">Boolean</span></span>|<span data-ttu-id="426cb-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="426cb-163">privacyInformationUrl</span></span>|<span data-ttu-id="426cb-164">Строка</span><span class="sxs-lookup"><span data-stu-id="426cb-164">String</span></span>|<span data-ttu-id="426cb-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="426cb-165">The privacy statement Url.</span></span> <span data-ttu-id="426cb-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="426cb-167">informationUrl</span></span>|<span data-ttu-id="426cb-168">Строка</span><span class="sxs-lookup"><span data-stu-id="426cb-168">String</span></span>|<span data-ttu-id="426cb-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="426cb-169">The more information Url.</span></span> <span data-ttu-id="426cb-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-171">owner</span><span class="sxs-lookup"><span data-stu-id="426cb-171">owner</span></span>|<span data-ttu-id="426cb-172">String</span><span class="sxs-lookup"><span data-stu-id="426cb-172">String</span></span>|<span data-ttu-id="426cb-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="426cb-173">The owner of the app.</span></span> <span data-ttu-id="426cb-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-175">developer</span><span class="sxs-lookup"><span data-stu-id="426cb-175">developer</span></span>|<span data-ttu-id="426cb-176">Строка</span><span class="sxs-lookup"><span data-stu-id="426cb-176">String</span></span>|<span data-ttu-id="426cb-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="426cb-177">The developer of the app.</span></span> <span data-ttu-id="426cb-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-179">notes</span><span class="sxs-lookup"><span data-stu-id="426cb-179">notes</span></span>|<span data-ttu-id="426cb-180">String</span><span class="sxs-lookup"><span data-stu-id="426cb-180">String</span></span>|<span data-ttu-id="426cb-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="426cb-181">Notes for the app.</span></span> <span data-ttu-id="426cb-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="426cb-183">uploadState</span></span>|<span data-ttu-id="426cb-184">Int32</span><span class="sxs-lookup"><span data-stu-id="426cb-184">Int32</span></span>|<span data-ttu-id="426cb-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="426cb-185">The upload state.</span></span> <span data-ttu-id="426cb-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="426cb-187">publishingState</span></span>|[<span data-ttu-id="426cb-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="426cb-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="426cb-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="426cb-189">The publishing state for the app.</span></span> <span data-ttu-id="426cb-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="426cb-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="426cb-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="426cb-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="426cb-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="426cb-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="426cb-193">isAssigned</span></span>|<span data-ttu-id="426cb-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="426cb-194">Boolean</span></span>|<span data-ttu-id="426cb-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="426cb-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="426cb-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="426cb-197">roleScopeTagIds</span></span>|<span data-ttu-id="426cb-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="426cb-198">String collection</span></span>|<span data-ttu-id="426cb-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="426cb-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="426cb-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="426cb-201">dependentAppCount</span></span>|<span data-ttu-id="426cb-202">Int32</span><span class="sxs-lookup"><span data-stu-id="426cb-202">Int32</span></span>|<span data-ttu-id="426cb-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="426cb-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="426cb-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="426cb-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="426cb-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="426cb-205">appStoreUrl</span></span>|<span data-ttu-id="426cb-206">String</span><span class="sxs-lookup"><span data-stu-id="426cb-206">String</span></span>|<span data-ttu-id="426cb-207">URL-адрес магазина приложений Windows Phone 8,1.</span><span class="sxs-lookup"><span data-stu-id="426cb-207">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="426cb-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="426cb-208">Response</span></span>
<span data-ttu-id="426cb-209">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="426cb-209">If successful, this method returns a `201 Created` response code and a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="426cb-210">Пример</span><span class="sxs-lookup"><span data-stu-id="426cb-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="426cb-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="426cb-211">Request</span></span>
<span data-ttu-id="426cb-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="426cb-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 775

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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="426cb-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="426cb-213">Response</span></span>
<span data-ttu-id="426cb-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="426cb-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 947

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




