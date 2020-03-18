---
title: Создание Виндовсстореапп
description: Создание нового объекта Виндовсстореапп.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b42b2376b84d1b18e63aa5cc4cfdb1419217e3e0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760713"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="34234-103">Создание Виндовсстореапп</span><span class="sxs-lookup"><span data-stu-id="34234-103">Create windowsStoreApp</span></span>

> <span data-ttu-id="34234-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34234-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34234-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34234-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34234-106">Создание нового объекта [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="34234-106">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34234-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="34234-107">Prerequisites</span></span>
<span data-ttu-id="34234-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34234-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34234-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34234-110">Permission type</span></span>|<span data-ttu-id="34234-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34234-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34234-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34234-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34234-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34234-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="34234-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34234-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34234-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34234-115">Not supported.</span></span>|
|<span data-ttu-id="34234-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="34234-116">Application</span></span>|<span data-ttu-id="34234-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34234-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34234-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34234-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="34234-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="34234-119">Request headers</span></span>
|<span data-ttu-id="34234-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34234-120">Header</span></span>|<span data-ttu-id="34234-121">Значение</span><span class="sxs-lookup"><span data-stu-id="34234-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34234-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="34234-122">Authorization</span></span>|<span data-ttu-id="34234-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34234-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34234-124">Accept</span><span class="sxs-lookup"><span data-stu-id="34234-124">Accept</span></span>|<span data-ttu-id="34234-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34234-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34234-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34234-126">Request body</span></span>
<span data-ttu-id="34234-127">В тексте запроса добавьте представление объекта Виндовсстореапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34234-127">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="34234-128">В следующей таблице приведены свойства, необходимые при создании Виндовсстореапп.</span><span class="sxs-lookup"><span data-stu-id="34234-128">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="34234-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="34234-129">Property</span></span>|<span data-ttu-id="34234-130">Тип</span><span class="sxs-lookup"><span data-stu-id="34234-130">Type</span></span>|<span data-ttu-id="34234-131">Описание</span><span class="sxs-lookup"><span data-stu-id="34234-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34234-132">id</span><span class="sxs-lookup"><span data-stu-id="34234-132">id</span></span>|<span data-ttu-id="34234-133">Строка</span><span class="sxs-lookup"><span data-stu-id="34234-133">String</span></span>|<span data-ttu-id="34234-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="34234-134">Key of the entity.</span></span> <span data-ttu-id="34234-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-136">displayName</span><span class="sxs-lookup"><span data-stu-id="34234-136">displayName</span></span>|<span data-ttu-id="34234-137">Строка</span><span class="sxs-lookup"><span data-stu-id="34234-137">String</span></span>|<span data-ttu-id="34234-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="34234-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="34234-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-140">description</span><span class="sxs-lookup"><span data-stu-id="34234-140">description</span></span>|<span data-ttu-id="34234-141">Строка</span><span class="sxs-lookup"><span data-stu-id="34234-141">String</span></span>|<span data-ttu-id="34234-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="34234-142">The description of the app.</span></span> <span data-ttu-id="34234-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-144">publisher</span><span class="sxs-lookup"><span data-stu-id="34234-144">publisher</span></span>|<span data-ttu-id="34234-145">String</span><span class="sxs-lookup"><span data-stu-id="34234-145">String</span></span>|<span data-ttu-id="34234-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="34234-146">The publisher of the app.</span></span> <span data-ttu-id="34234-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="34234-148">largeIcon</span></span>|[<span data-ttu-id="34234-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="34234-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="34234-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="34234-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="34234-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34234-152">createdDateTime</span></span>|<span data-ttu-id="34234-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34234-153">DateTimeOffset</span></span>|<span data-ttu-id="34234-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="34234-154">The date and time the app was created.</span></span> <span data-ttu-id="34234-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34234-156">lastModifiedDateTime</span></span>|<span data-ttu-id="34234-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34234-157">DateTimeOffset</span></span>|<span data-ttu-id="34234-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="34234-158">The date and time the app was last modified.</span></span> <span data-ttu-id="34234-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="34234-160">isFeatured</span></span>|<span data-ttu-id="34234-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="34234-161">Boolean</span></span>|<span data-ttu-id="34234-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="34234-163">privacyInformationUrl</span></span>|<span data-ttu-id="34234-164">String</span><span class="sxs-lookup"><span data-stu-id="34234-164">String</span></span>|<span data-ttu-id="34234-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="34234-165">The privacy statement Url.</span></span> <span data-ttu-id="34234-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="34234-167">informationUrl</span></span>|<span data-ttu-id="34234-168">String</span><span class="sxs-lookup"><span data-stu-id="34234-168">String</span></span>|<span data-ttu-id="34234-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="34234-169">The more information Url.</span></span> <span data-ttu-id="34234-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-171">owner</span><span class="sxs-lookup"><span data-stu-id="34234-171">owner</span></span>|<span data-ttu-id="34234-172">String</span><span class="sxs-lookup"><span data-stu-id="34234-172">String</span></span>|<span data-ttu-id="34234-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="34234-173">The owner of the app.</span></span> <span data-ttu-id="34234-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-175">developer</span><span class="sxs-lookup"><span data-stu-id="34234-175">developer</span></span>|<span data-ttu-id="34234-176">String</span><span class="sxs-lookup"><span data-stu-id="34234-176">String</span></span>|<span data-ttu-id="34234-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="34234-177">The developer of the app.</span></span> <span data-ttu-id="34234-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-179">notes</span><span class="sxs-lookup"><span data-stu-id="34234-179">notes</span></span>|<span data-ttu-id="34234-180">String</span><span class="sxs-lookup"><span data-stu-id="34234-180">String</span></span>|<span data-ttu-id="34234-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="34234-181">Notes for the app.</span></span> <span data-ttu-id="34234-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="34234-183">uploadState</span></span>|<span data-ttu-id="34234-184">Int32</span><span class="sxs-lookup"><span data-stu-id="34234-184">Int32</span></span>|<span data-ttu-id="34234-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="34234-185">The upload state.</span></span> <span data-ttu-id="34234-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="34234-187">publishingState</span></span>|[<span data-ttu-id="34234-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="34234-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="34234-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="34234-189">The publishing state for the app.</span></span> <span data-ttu-id="34234-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="34234-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="34234-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="34234-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="34234-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="34234-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="34234-193">isAssigned</span></span>|<span data-ttu-id="34234-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="34234-194">Boolean</span></span>|<span data-ttu-id="34234-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="34234-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="34234-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34234-197">roleScopeTagIds</span></span>|<span data-ttu-id="34234-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="34234-198">String collection</span></span>|<span data-ttu-id="34234-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="34234-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="34234-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="34234-201">dependentAppCount</span></span>|<span data-ttu-id="34234-202">Int32</span><span class="sxs-lookup"><span data-stu-id="34234-202">Int32</span></span>|<span data-ttu-id="34234-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="34234-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="34234-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34234-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="34234-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="34234-205">appStoreUrl</span></span>|<span data-ttu-id="34234-206">String</span><span class="sxs-lookup"><span data-stu-id="34234-206">String</span></span>|<span data-ttu-id="34234-207">URL-адрес хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="34234-207">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="34234-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="34234-208">Response</span></span>
<span data-ttu-id="34234-209">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34234-209">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34234-210">Пример</span><span class="sxs-lookup"><span data-stu-id="34234-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="34234-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="34234-211">Request</span></span>
<span data-ttu-id="34234-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34234-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 768

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

### <a name="response"></a><span data-ttu-id="34234-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="34234-213">Response</span></span>
<span data-ttu-id="34234-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34234-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 940

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




