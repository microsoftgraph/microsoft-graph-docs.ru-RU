---
title: Обновление объекта macOSOfficeSuiteApp
description: Обновление свойств объекта macOSOfficeSuiteApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 675372d58c67c15fccfce0c3797c36045687e6e2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761694"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="877ab-103">Обновление объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="877ab-103">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="877ab-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="877ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="877ab-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="877ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="877ab-106">Обновление свойств объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-106">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="877ab-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="877ab-107">Prerequisites</span></span>
<span data-ttu-id="877ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="877ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="877ab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="877ab-110">Permission type</span></span>|<span data-ttu-id="877ab-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="877ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="877ab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="877ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="877ab-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="877ab-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="877ab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="877ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="877ab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="877ab-115">Not supported.</span></span>|
|<span data-ttu-id="877ab-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="877ab-116">Application</span></span>|<span data-ttu-id="877ab-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="877ab-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="877ab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="877ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="877ab-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="877ab-119">Request headers</span></span>
|<span data-ttu-id="877ab-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="877ab-120">Header</span></span>|<span data-ttu-id="877ab-121">Значение</span><span class="sxs-lookup"><span data-stu-id="877ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="877ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="877ab-122">Authorization</span></span>|<span data-ttu-id="877ab-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="877ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="877ab-124">Accept</span><span class="sxs-lookup"><span data-stu-id="877ab-124">Accept</span></span>|<span data-ttu-id="877ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="877ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="877ab-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="877ab-126">Request body</span></span>
<span data-ttu-id="877ab-127">В тексте запроса добавьте представление объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="877ab-127">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="877ab-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-128">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="877ab-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="877ab-129">Property</span></span>|<span data-ttu-id="877ab-130">Тип</span><span class="sxs-lookup"><span data-stu-id="877ab-130">Type</span></span>|<span data-ttu-id="877ab-131">Описание</span><span class="sxs-lookup"><span data-stu-id="877ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="877ab-132">id</span><span class="sxs-lookup"><span data-stu-id="877ab-132">id</span></span>|<span data-ttu-id="877ab-133">Строка</span><span class="sxs-lookup"><span data-stu-id="877ab-133">String</span></span>|<span data-ttu-id="877ab-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="877ab-134">Key of the entity.</span></span> <span data-ttu-id="877ab-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-136">displayName</span><span class="sxs-lookup"><span data-stu-id="877ab-136">displayName</span></span>|<span data-ttu-id="877ab-137">Строка</span><span class="sxs-lookup"><span data-stu-id="877ab-137">String</span></span>|<span data-ttu-id="877ab-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="877ab-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="877ab-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-140">description</span><span class="sxs-lookup"><span data-stu-id="877ab-140">description</span></span>|<span data-ttu-id="877ab-141">Строка</span><span class="sxs-lookup"><span data-stu-id="877ab-141">String</span></span>|<span data-ttu-id="877ab-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="877ab-142">The description of the app.</span></span> <span data-ttu-id="877ab-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-144">publisher</span><span class="sxs-lookup"><span data-stu-id="877ab-144">publisher</span></span>|<span data-ttu-id="877ab-145">String</span><span class="sxs-lookup"><span data-stu-id="877ab-145">String</span></span>|<span data-ttu-id="877ab-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="877ab-146">The publisher of the app.</span></span> <span data-ttu-id="877ab-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="877ab-148">largeIcon</span></span>|[<span data-ttu-id="877ab-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="877ab-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="877ab-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="877ab-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="877ab-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="877ab-152">createdDateTime</span></span>|<span data-ttu-id="877ab-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="877ab-153">DateTimeOffset</span></span>|<span data-ttu-id="877ab-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="877ab-154">The date and time the app was created.</span></span> <span data-ttu-id="877ab-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="877ab-156">lastModifiedDateTime</span></span>|<span data-ttu-id="877ab-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="877ab-157">DateTimeOffset</span></span>|<span data-ttu-id="877ab-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="877ab-158">The date and time the app was last modified.</span></span> <span data-ttu-id="877ab-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="877ab-160">isFeatured</span></span>|<span data-ttu-id="877ab-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="877ab-161">Boolean</span></span>|<span data-ttu-id="877ab-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="877ab-163">privacyInformationUrl</span></span>|<span data-ttu-id="877ab-164">String</span><span class="sxs-lookup"><span data-stu-id="877ab-164">String</span></span>|<span data-ttu-id="877ab-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="877ab-165">The privacy statement Url.</span></span> <span data-ttu-id="877ab-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="877ab-167">informationUrl</span></span>|<span data-ttu-id="877ab-168">String</span><span class="sxs-lookup"><span data-stu-id="877ab-168">String</span></span>|<span data-ttu-id="877ab-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="877ab-169">The more information Url.</span></span> <span data-ttu-id="877ab-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-171">owner</span><span class="sxs-lookup"><span data-stu-id="877ab-171">owner</span></span>|<span data-ttu-id="877ab-172">String</span><span class="sxs-lookup"><span data-stu-id="877ab-172">String</span></span>|<span data-ttu-id="877ab-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="877ab-173">The owner of the app.</span></span> <span data-ttu-id="877ab-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-175">developer</span><span class="sxs-lookup"><span data-stu-id="877ab-175">developer</span></span>|<span data-ttu-id="877ab-176">String</span><span class="sxs-lookup"><span data-stu-id="877ab-176">String</span></span>|<span data-ttu-id="877ab-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="877ab-177">The developer of the app.</span></span> <span data-ttu-id="877ab-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-179">notes</span><span class="sxs-lookup"><span data-stu-id="877ab-179">notes</span></span>|<span data-ttu-id="877ab-180">String</span><span class="sxs-lookup"><span data-stu-id="877ab-180">String</span></span>|<span data-ttu-id="877ab-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="877ab-181">Notes for the app.</span></span> <span data-ttu-id="877ab-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="877ab-183">uploadState</span></span>|<span data-ttu-id="877ab-184">Int32</span><span class="sxs-lookup"><span data-stu-id="877ab-184">Int32</span></span>|<span data-ttu-id="877ab-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="877ab-185">The upload state.</span></span> <span data-ttu-id="877ab-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="877ab-187">publishingState</span></span>|[<span data-ttu-id="877ab-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="877ab-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="877ab-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="877ab-189">The publishing state for the app.</span></span> <span data-ttu-id="877ab-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="877ab-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="877ab-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="877ab-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="877ab-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="877ab-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="877ab-193">isAssigned</span></span>|<span data-ttu-id="877ab-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="877ab-194">Boolean</span></span>|<span data-ttu-id="877ab-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="877ab-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="877ab-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="877ab-197">roleScopeTagIds</span></span>|<span data-ttu-id="877ab-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="877ab-198">String collection</span></span>|<span data-ttu-id="877ab-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="877ab-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="877ab-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="877ab-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="877ab-201">dependentAppCount</span></span>|<span data-ttu-id="877ab-202">Int32</span><span class="sxs-lookup"><span data-stu-id="877ab-202">Int32</span></span>|<span data-ttu-id="877ab-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="877ab-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="877ab-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="877ab-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="877ab-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="877ab-205">Response</span></span>
<span data-ttu-id="877ab-206">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="877ab-206">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="877ab-207">Пример</span><span class="sxs-lookup"><span data-stu-id="877ab-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="877ab-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="877ab-208">Request</span></span>
<span data-ttu-id="877ab-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="877ab-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 718

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="877ab-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="877ab-210">Response</span></span>
<span data-ttu-id="877ab-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="877ab-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 890

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
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1
}
```




