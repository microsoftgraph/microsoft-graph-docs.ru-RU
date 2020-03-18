---
title: Обновление windowsPhone81StoreApp
description: Обновление свойств объекта windowsPhone81StoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 50f87db27ff37a06946a0fdf852c754f7465ea5f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760762"
---
# <a name="update-windowsphone81storeapp"></a><span data-ttu-id="534ee-103">Обновление windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="534ee-103">Update windowsPhone81StoreApp</span></span>

> <span data-ttu-id="534ee-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="534ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="534ee-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="534ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="534ee-106">Обновление свойств объекта [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="534ee-106">Update the properties of a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="534ee-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="534ee-107">Prerequisites</span></span>
<span data-ttu-id="534ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="534ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="534ee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="534ee-110">Permission type</span></span>|<span data-ttu-id="534ee-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="534ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="534ee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="534ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="534ee-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="534ee-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="534ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="534ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="534ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="534ee-115">Not supported.</span></span>|
|<span data-ttu-id="534ee-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="534ee-116">Application</span></span>|<span data-ttu-id="534ee-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="534ee-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="534ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="534ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="534ee-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="534ee-119">Request headers</span></span>
|<span data-ttu-id="534ee-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="534ee-120">Header</span></span>|<span data-ttu-id="534ee-121">Значение</span><span class="sxs-lookup"><span data-stu-id="534ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="534ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="534ee-122">Authorization</span></span>|<span data-ttu-id="534ee-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="534ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="534ee-124">Accept</span><span class="sxs-lookup"><span data-stu-id="534ee-124">Accept</span></span>|<span data-ttu-id="534ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="534ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="534ee-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="534ee-126">Request body</span></span>
<span data-ttu-id="534ee-127">В тексте запроса добавьте представление объекта [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="534ee-127">In the request body, supply a JSON representation for the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

<span data-ttu-id="534ee-128">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-128">The following table shows the properties that are required when you create the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span></span>

|<span data-ttu-id="534ee-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="534ee-129">Property</span></span>|<span data-ttu-id="534ee-130">Тип</span><span class="sxs-lookup"><span data-stu-id="534ee-130">Type</span></span>|<span data-ttu-id="534ee-131">Описание</span><span class="sxs-lookup"><span data-stu-id="534ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="534ee-132">id</span><span class="sxs-lookup"><span data-stu-id="534ee-132">id</span></span>|<span data-ttu-id="534ee-133">Строка</span><span class="sxs-lookup"><span data-stu-id="534ee-133">String</span></span>|<span data-ttu-id="534ee-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="534ee-134">Key of the entity.</span></span> <span data-ttu-id="534ee-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-136">displayName</span><span class="sxs-lookup"><span data-stu-id="534ee-136">displayName</span></span>|<span data-ttu-id="534ee-137">Строка</span><span class="sxs-lookup"><span data-stu-id="534ee-137">String</span></span>|<span data-ttu-id="534ee-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="534ee-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="534ee-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-140">description</span><span class="sxs-lookup"><span data-stu-id="534ee-140">description</span></span>|<span data-ttu-id="534ee-141">Строка</span><span class="sxs-lookup"><span data-stu-id="534ee-141">String</span></span>|<span data-ttu-id="534ee-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="534ee-142">The description of the app.</span></span> <span data-ttu-id="534ee-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-144">publisher</span><span class="sxs-lookup"><span data-stu-id="534ee-144">publisher</span></span>|<span data-ttu-id="534ee-145">String</span><span class="sxs-lookup"><span data-stu-id="534ee-145">String</span></span>|<span data-ttu-id="534ee-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="534ee-146">The publisher of the app.</span></span> <span data-ttu-id="534ee-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="534ee-148">largeIcon</span></span>|[<span data-ttu-id="534ee-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="534ee-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="534ee-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="534ee-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="534ee-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="534ee-152">createdDateTime</span></span>|<span data-ttu-id="534ee-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="534ee-153">DateTimeOffset</span></span>|<span data-ttu-id="534ee-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="534ee-154">The date and time the app was created.</span></span> <span data-ttu-id="534ee-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="534ee-156">lastModifiedDateTime</span></span>|<span data-ttu-id="534ee-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="534ee-157">DateTimeOffset</span></span>|<span data-ttu-id="534ee-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="534ee-158">The date and time the app was last modified.</span></span> <span data-ttu-id="534ee-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="534ee-160">isFeatured</span></span>|<span data-ttu-id="534ee-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="534ee-161">Boolean</span></span>|<span data-ttu-id="534ee-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="534ee-163">privacyInformationUrl</span></span>|<span data-ttu-id="534ee-164">String</span><span class="sxs-lookup"><span data-stu-id="534ee-164">String</span></span>|<span data-ttu-id="534ee-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="534ee-165">The privacy statement Url.</span></span> <span data-ttu-id="534ee-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="534ee-167">informationUrl</span></span>|<span data-ttu-id="534ee-168">String</span><span class="sxs-lookup"><span data-stu-id="534ee-168">String</span></span>|<span data-ttu-id="534ee-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="534ee-169">The more information Url.</span></span> <span data-ttu-id="534ee-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-171">owner</span><span class="sxs-lookup"><span data-stu-id="534ee-171">owner</span></span>|<span data-ttu-id="534ee-172">String</span><span class="sxs-lookup"><span data-stu-id="534ee-172">String</span></span>|<span data-ttu-id="534ee-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="534ee-173">The owner of the app.</span></span> <span data-ttu-id="534ee-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-175">developer</span><span class="sxs-lookup"><span data-stu-id="534ee-175">developer</span></span>|<span data-ttu-id="534ee-176">String</span><span class="sxs-lookup"><span data-stu-id="534ee-176">String</span></span>|<span data-ttu-id="534ee-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="534ee-177">The developer of the app.</span></span> <span data-ttu-id="534ee-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-179">notes</span><span class="sxs-lookup"><span data-stu-id="534ee-179">notes</span></span>|<span data-ttu-id="534ee-180">String</span><span class="sxs-lookup"><span data-stu-id="534ee-180">String</span></span>|<span data-ttu-id="534ee-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="534ee-181">Notes for the app.</span></span> <span data-ttu-id="534ee-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="534ee-183">uploadState</span></span>|<span data-ttu-id="534ee-184">Int32</span><span class="sxs-lookup"><span data-stu-id="534ee-184">Int32</span></span>|<span data-ttu-id="534ee-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="534ee-185">The upload state.</span></span> <span data-ttu-id="534ee-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="534ee-187">publishingState</span></span>|[<span data-ttu-id="534ee-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="534ee-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="534ee-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="534ee-189">The publishing state for the app.</span></span> <span data-ttu-id="534ee-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="534ee-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="534ee-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="534ee-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="534ee-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="534ee-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="534ee-193">isAssigned</span></span>|<span data-ttu-id="534ee-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="534ee-194">Boolean</span></span>|<span data-ttu-id="534ee-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="534ee-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="534ee-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="534ee-197">roleScopeTagIds</span></span>|<span data-ttu-id="534ee-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="534ee-198">String collection</span></span>|<span data-ttu-id="534ee-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="534ee-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="534ee-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="534ee-201">dependentAppCount</span></span>|<span data-ttu-id="534ee-202">Int32</span><span class="sxs-lookup"><span data-stu-id="534ee-202">Int32</span></span>|<span data-ttu-id="534ee-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="534ee-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="534ee-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="534ee-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="534ee-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="534ee-205">appStoreUrl</span></span>|<span data-ttu-id="534ee-206">String</span><span class="sxs-lookup"><span data-stu-id="534ee-206">String</span></span>|<span data-ttu-id="534ee-207">URL-адрес магазина приложений Windows Phone 8,1.</span><span class="sxs-lookup"><span data-stu-id="534ee-207">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="534ee-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="534ee-208">Response</span></span>
<span data-ttu-id="534ee-209">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="534ee-209">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="534ee-210">Пример</span><span class="sxs-lookup"><span data-stu-id="534ee-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="534ee-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="534ee-211">Request</span></span>
<span data-ttu-id="534ee-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="534ee-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="534ee-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="534ee-213">Response</span></span>
<span data-ttu-id="534ee-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="534ee-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




