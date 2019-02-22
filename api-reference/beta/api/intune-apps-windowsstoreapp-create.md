---
title: Создание Виндовсстореапп
description: Создание нового объекта Виндовсстореапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33388b171e73a3d830f3703018a2f0490650c358
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147483"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="42ee8-103">Создание Виндовсстореапп</span><span class="sxs-lookup"><span data-stu-id="42ee8-103">Create windowsStoreApp</span></span>

> <span data-ttu-id="42ee8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42ee8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42ee8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42ee8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42ee8-106">Создание нового объекта [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="42ee8-106">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42ee8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="42ee8-107">Prerequisites</span></span>
<span data-ttu-id="42ee8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="42ee8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42ee8-110">Permission type</span></span>|<span data-ttu-id="42ee8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42ee8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42ee8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42ee8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42ee8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42ee8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="42ee8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42ee8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42ee8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42ee8-115">Not supported.</span></span>|
|<span data-ttu-id="42ee8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42ee8-116">Application</span></span>|<span data-ttu-id="42ee8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42ee8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42ee8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42ee8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="42ee8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42ee8-119">Request headers</span></span>
|<span data-ttu-id="42ee8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42ee8-120">Header</span></span>|<span data-ttu-id="42ee8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="42ee8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42ee8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42ee8-122">Authorization</span></span>|<span data-ttu-id="42ee8-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="42ee8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42ee8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="42ee8-124">Accept</span></span>|<span data-ttu-id="42ee8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42ee8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42ee8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42ee8-126">Request body</span></span>
<span data-ttu-id="42ee8-127">В тексте запроса добавьте представление объекта Виндовсстореапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42ee8-127">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="42ee8-128">В следующей таблице приведены свойства, необходимые при создании Виндовсстореапп.</span><span class="sxs-lookup"><span data-stu-id="42ee8-128">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="42ee8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="42ee8-129">Property</span></span>|<span data-ttu-id="42ee8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="42ee8-130">Type</span></span>|<span data-ttu-id="42ee8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="42ee8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42ee8-132">id</span><span class="sxs-lookup"><span data-stu-id="42ee8-132">id</span></span>|<span data-ttu-id="42ee8-133">Строка</span><span class="sxs-lookup"><span data-stu-id="42ee8-133">String</span></span>|<span data-ttu-id="42ee8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="42ee8-134">Key of the entity.</span></span> <span data-ttu-id="42ee8-135">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="42ee8-136">displayName</span></span>|<span data-ttu-id="42ee8-137">String</span><span class="sxs-lookup"><span data-stu-id="42ee8-137">String</span></span>|<span data-ttu-id="42ee8-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="42ee8-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="42ee8-139">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-140">description</span><span class="sxs-lookup"><span data-stu-id="42ee8-140">description</span></span>|<span data-ttu-id="42ee8-141">Строка</span><span class="sxs-lookup"><span data-stu-id="42ee8-141">String</span></span>|<span data-ttu-id="42ee8-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="42ee8-142">The description of the app.</span></span> <span data-ttu-id="42ee8-143">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-144">publisher</span><span class="sxs-lookup"><span data-stu-id="42ee8-144">publisher</span></span>|<span data-ttu-id="42ee8-145">String</span><span class="sxs-lookup"><span data-stu-id="42ee8-145">String</span></span>|<span data-ttu-id="42ee8-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="42ee8-146">The publisher of the app.</span></span> <span data-ttu-id="42ee8-147">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="42ee8-148">largeIcon</span></span>|[<span data-ttu-id="42ee8-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="42ee8-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="42ee8-150">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="42ee8-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="42ee8-151">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42ee8-152">createdDateTime</span></span>|<span data-ttu-id="42ee8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42ee8-153">DateTimeOffset</span></span>|<span data-ttu-id="42ee8-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="42ee8-154">The date and time the app was created.</span></span> <span data-ttu-id="42ee8-155">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42ee8-156">lastModifiedDateTime</span></span>|<span data-ttu-id="42ee8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42ee8-157">DateTimeOffset</span></span>|<span data-ttu-id="42ee8-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="42ee8-158">The date and time the app was last modified.</span></span> <span data-ttu-id="42ee8-159">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="42ee8-160">isFeatured</span></span>|<span data-ttu-id="42ee8-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="42ee8-161">Boolean</span></span>|<span data-ttu-id="42ee8-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="42ee8-163">privacyInformationUrl</span></span>|<span data-ttu-id="42ee8-164">String</span><span class="sxs-lookup"><span data-stu-id="42ee8-164">String</span></span>|<span data-ttu-id="42ee8-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="42ee8-165">The privacy statement Url.</span></span> <span data-ttu-id="42ee8-166">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="42ee8-167">informationUrl</span></span>|<span data-ttu-id="42ee8-168">String</span><span class="sxs-lookup"><span data-stu-id="42ee8-168">String</span></span>|<span data-ttu-id="42ee8-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="42ee8-169">The more information Url.</span></span> <span data-ttu-id="42ee8-170">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-171">owner</span><span class="sxs-lookup"><span data-stu-id="42ee8-171">owner</span></span>|<span data-ttu-id="42ee8-172">String</span><span class="sxs-lookup"><span data-stu-id="42ee8-172">String</span></span>|<span data-ttu-id="42ee8-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="42ee8-173">The owner of the app.</span></span> <span data-ttu-id="42ee8-174">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-175">developer</span><span class="sxs-lookup"><span data-stu-id="42ee8-175">developer</span></span>|<span data-ttu-id="42ee8-176">String</span><span class="sxs-lookup"><span data-stu-id="42ee8-176">String</span></span>|<span data-ttu-id="42ee8-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="42ee8-177">The developer of the app.</span></span> <span data-ttu-id="42ee8-178">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-179">notes</span><span class="sxs-lookup"><span data-stu-id="42ee8-179">notes</span></span>|<span data-ttu-id="42ee8-180">String</span><span class="sxs-lookup"><span data-stu-id="42ee8-180">String</span></span>|<span data-ttu-id="42ee8-181">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="42ee8-181">Notes for the app.</span></span> <span data-ttu-id="42ee8-182">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="42ee8-183">uploadState</span></span>|<span data-ttu-id="42ee8-184">Int32</span><span class="sxs-lookup"><span data-stu-id="42ee8-184">Int32</span></span>|<span data-ttu-id="42ee8-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="42ee8-185">The upload state.</span></span> <span data-ttu-id="42ee8-186">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="42ee8-187">publishingState</span></span>|[<span data-ttu-id="42ee8-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="42ee8-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="42ee8-189">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="42ee8-189">The publishing state for the app.</span></span> <span data-ttu-id="42ee8-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="42ee8-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="42ee8-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="42ee8-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="42ee8-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="42ee8-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="42ee8-193">isAssigned</span></span>|<span data-ttu-id="42ee8-194">Логический</span><span class="sxs-lookup"><span data-stu-id="42ee8-194">Boolean</span></span>|<span data-ttu-id="42ee8-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="42ee8-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="42ee8-196">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42ee8-197">roleScopeTagIds</span></span>|<span data-ttu-id="42ee8-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="42ee8-198">String collection</span></span>|<span data-ttu-id="42ee8-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="42ee8-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="42ee8-200">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42ee8-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="42ee8-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="42ee8-201">appStoreUrl</span></span>|<span data-ttu-id="42ee8-202">String</span><span class="sxs-lookup"><span data-stu-id="42ee8-202">String</span></span>|<span data-ttu-id="42ee8-203">URL-адрес хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="42ee8-203">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="42ee8-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="42ee8-204">Response</span></span>
<span data-ttu-id="42ee8-205">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42ee8-205">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42ee8-206">Пример</span><span class="sxs-lookup"><span data-stu-id="42ee8-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="42ee8-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="42ee8-207">Request</span></span>
<span data-ttu-id="42ee8-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42ee8-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 741

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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="42ee8-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="42ee8-209">Response</span></span>
<span data-ttu-id="42ee8-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42ee8-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 913

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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




