---
title: Обновление Виндовсстореапп
description: Обновление свойств объекта Виндовсстореапп.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e86afaf2c60aae3273bd5f8a59df095bb45ca2e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149233"
---
# <a name="update-windowsstoreapp"></a><span data-ttu-id="809e0-103">Обновление Виндовсстореапп</span><span class="sxs-lookup"><span data-stu-id="809e0-103">Update windowsStoreApp</span></span>

> <span data-ttu-id="809e0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="809e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="809e0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="809e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="809e0-106">Обновление свойств объекта [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="809e0-106">Update the properties of a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="809e0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="809e0-107">Prerequisites</span></span>
<span data-ttu-id="809e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="809e0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="809e0-110">Permission type</span></span>|<span data-ttu-id="809e0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="809e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="809e0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="809e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="809e0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="809e0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="809e0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="809e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="809e0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="809e0-115">Not supported.</span></span>|
|<span data-ttu-id="809e0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="809e0-116">Application</span></span>|<span data-ttu-id="809e0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="809e0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="809e0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="809e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="809e0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="809e0-119">Request headers</span></span>
|<span data-ttu-id="809e0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="809e0-120">Header</span></span>|<span data-ttu-id="809e0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="809e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="809e0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="809e0-122">Authorization</span></span>|<span data-ttu-id="809e0-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="809e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="809e0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="809e0-124">Accept</span></span>|<span data-ttu-id="809e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="809e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="809e0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="809e0-126">Request body</span></span>
<span data-ttu-id="809e0-127">В тексте запроса добавьте представление объекта [Виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="809e0-127">In the request body, supply a JSON representation for the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

<span data-ttu-id="809e0-128">В следующей таблице приведены свойства, необходимые при создании [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-128">The following table shows the properties that are required when you create the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span></span>

|<span data-ttu-id="809e0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="809e0-129">Property</span></span>|<span data-ttu-id="809e0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="809e0-130">Type</span></span>|<span data-ttu-id="809e0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="809e0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="809e0-132">id</span><span class="sxs-lookup"><span data-stu-id="809e0-132">id</span></span>|<span data-ttu-id="809e0-133">Строка</span><span class="sxs-lookup"><span data-stu-id="809e0-133">String</span></span>|<span data-ttu-id="809e0-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="809e0-134">Key of the entity.</span></span> <span data-ttu-id="809e0-135">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="809e0-136">displayName</span></span>|<span data-ttu-id="809e0-137">String</span><span class="sxs-lookup"><span data-stu-id="809e0-137">String</span></span>|<span data-ttu-id="809e0-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="809e0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="809e0-139">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-140">description</span><span class="sxs-lookup"><span data-stu-id="809e0-140">description</span></span>|<span data-ttu-id="809e0-141">Строка</span><span class="sxs-lookup"><span data-stu-id="809e0-141">String</span></span>|<span data-ttu-id="809e0-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="809e0-142">The description of the app.</span></span> <span data-ttu-id="809e0-143">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-144">publisher</span><span class="sxs-lookup"><span data-stu-id="809e0-144">publisher</span></span>|<span data-ttu-id="809e0-145">String</span><span class="sxs-lookup"><span data-stu-id="809e0-145">String</span></span>|<span data-ttu-id="809e0-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="809e0-146">The publisher of the app.</span></span> <span data-ttu-id="809e0-147">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="809e0-148">largeIcon</span></span>|[<span data-ttu-id="809e0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="809e0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="809e0-150">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="809e0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="809e0-151">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="809e0-152">createdDateTime</span></span>|<span data-ttu-id="809e0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="809e0-153">DateTimeOffset</span></span>|<span data-ttu-id="809e0-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="809e0-154">The date and time the app was created.</span></span> <span data-ttu-id="809e0-155">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="809e0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="809e0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="809e0-157">DateTimeOffset</span></span>|<span data-ttu-id="809e0-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="809e0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="809e0-159">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="809e0-160">isFeatured</span></span>|<span data-ttu-id="809e0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="809e0-161">Boolean</span></span>|<span data-ttu-id="809e0-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="809e0-163">privacyInformationUrl</span></span>|<span data-ttu-id="809e0-164">String</span><span class="sxs-lookup"><span data-stu-id="809e0-164">String</span></span>|<span data-ttu-id="809e0-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="809e0-165">The privacy statement Url.</span></span> <span data-ttu-id="809e0-166">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="809e0-167">informationUrl</span></span>|<span data-ttu-id="809e0-168">String</span><span class="sxs-lookup"><span data-stu-id="809e0-168">String</span></span>|<span data-ttu-id="809e0-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="809e0-169">The more information Url.</span></span> <span data-ttu-id="809e0-170">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-171">owner</span><span class="sxs-lookup"><span data-stu-id="809e0-171">owner</span></span>|<span data-ttu-id="809e0-172">String</span><span class="sxs-lookup"><span data-stu-id="809e0-172">String</span></span>|<span data-ttu-id="809e0-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="809e0-173">The owner of the app.</span></span> <span data-ttu-id="809e0-174">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-175">developer</span><span class="sxs-lookup"><span data-stu-id="809e0-175">developer</span></span>|<span data-ttu-id="809e0-176">String</span><span class="sxs-lookup"><span data-stu-id="809e0-176">String</span></span>|<span data-ttu-id="809e0-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="809e0-177">The developer of the app.</span></span> <span data-ttu-id="809e0-178">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-179">notes</span><span class="sxs-lookup"><span data-stu-id="809e0-179">notes</span></span>|<span data-ttu-id="809e0-180">String</span><span class="sxs-lookup"><span data-stu-id="809e0-180">String</span></span>|<span data-ttu-id="809e0-181">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="809e0-181">Notes for the app.</span></span> <span data-ttu-id="809e0-182">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="809e0-183">uploadState</span></span>|<span data-ttu-id="809e0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="809e0-184">Int32</span></span>|<span data-ttu-id="809e0-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="809e0-185">The upload state.</span></span> <span data-ttu-id="809e0-186">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="809e0-187">publishingState</span></span>|[<span data-ttu-id="809e0-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="809e0-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="809e0-189">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="809e0-189">The publishing state for the app.</span></span> <span data-ttu-id="809e0-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="809e0-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="809e0-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="809e0-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="809e0-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="809e0-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="809e0-193">isAssigned</span></span>|<span data-ttu-id="809e0-194">Логический</span><span class="sxs-lookup"><span data-stu-id="809e0-194">Boolean</span></span>|<span data-ttu-id="809e0-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="809e0-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="809e0-196">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="809e0-197">roleScopeTagIds</span></span>|<span data-ttu-id="809e0-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="809e0-198">String collection</span></span>|<span data-ttu-id="809e0-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="809e0-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="809e0-200">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="809e0-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="809e0-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="809e0-201">appStoreUrl</span></span>|<span data-ttu-id="809e0-202">String</span><span class="sxs-lookup"><span data-stu-id="809e0-202">String</span></span>|<span data-ttu-id="809e0-203">URL-адрес хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="809e0-203">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="809e0-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="809e0-204">Response</span></span>
<span data-ttu-id="809e0-205">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="809e0-205">If successful, this method returns a `200 OK` response code and an updated [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="809e0-206">Пример</span><span class="sxs-lookup"><span data-stu-id="809e0-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="809e0-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="809e0-207">Request</span></span>
<span data-ttu-id="809e0-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="809e0-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="809e0-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="809e0-209">Response</span></span>
<span data-ttu-id="809e0-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="809e0-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




