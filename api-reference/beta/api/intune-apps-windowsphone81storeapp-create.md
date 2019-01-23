---
title: Создание windowsPhone81StoreApp
description: Создание нового объекта windowsPhone81StoreApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cab4143bd2ffd623b4e38d73d11228a6ba3f4b34
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394448"
---
# <a name="create-windowsphone81storeapp"></a><span data-ttu-id="20149-103">Создание windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="20149-103">Create windowsPhone81StoreApp</span></span>

> <span data-ttu-id="20149-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="20149-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="20149-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20149-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20149-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20149-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20149-107">Создание нового объекта [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="20149-107">Create a new [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20149-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="20149-108">Prerequisites</span></span>
<span data-ttu-id="20149-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="20149-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="20149-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20149-111">Permission type</span></span>|<span data-ttu-id="20149-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20149-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20149-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20149-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20149-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20149-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="20149-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20149-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20149-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20149-116">Not supported.</span></span>|
|<span data-ttu-id="20149-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20149-117">Application</span></span>|<span data-ttu-id="20149-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20149-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20149-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20149-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="20149-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20149-120">Request headers</span></span>
|<span data-ttu-id="20149-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20149-121">Header</span></span>|<span data-ttu-id="20149-122">Значение</span><span class="sxs-lookup"><span data-stu-id="20149-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20149-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20149-123">Authorization</span></span>|<span data-ttu-id="20149-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="20149-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20149-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20149-125">Accept</span></span>|<span data-ttu-id="20149-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20149-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20149-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20149-127">Request body</span></span>
<span data-ttu-id="20149-128">В тексте запроса укажите представление JSON для объекта windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="20149-128">In the request body, supply a JSON representation for the windowsPhone81StoreApp object.</span></span>

<span data-ttu-id="20149-129">В следующей таблице показаны свойства, которые необходимы для создания windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="20149-129">The following table shows the properties that are required when you create the windowsPhone81StoreApp.</span></span>

|<span data-ttu-id="20149-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="20149-130">Property</span></span>|<span data-ttu-id="20149-131">Тип</span><span class="sxs-lookup"><span data-stu-id="20149-131">Type</span></span>|<span data-ttu-id="20149-132">Описание</span><span class="sxs-lookup"><span data-stu-id="20149-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20149-133">id</span><span class="sxs-lookup"><span data-stu-id="20149-133">id</span></span>|<span data-ttu-id="20149-134">String</span><span class="sxs-lookup"><span data-stu-id="20149-134">String</span></span>|<span data-ttu-id="20149-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="20149-135">Key of the entity.</span></span> <span data-ttu-id="20149-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-137">displayName</span><span class="sxs-lookup"><span data-stu-id="20149-137">displayName</span></span>|<span data-ttu-id="20149-138">String</span><span class="sxs-lookup"><span data-stu-id="20149-138">String</span></span>|<span data-ttu-id="20149-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="20149-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="20149-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-141">description</span><span class="sxs-lookup"><span data-stu-id="20149-141">description</span></span>|<span data-ttu-id="20149-142">String</span><span class="sxs-lookup"><span data-stu-id="20149-142">String</span></span>|<span data-ttu-id="20149-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="20149-143">The description of the app.</span></span> <span data-ttu-id="20149-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-145">publisher</span><span class="sxs-lookup"><span data-stu-id="20149-145">publisher</span></span>|<span data-ttu-id="20149-146">String</span><span class="sxs-lookup"><span data-stu-id="20149-146">String</span></span>|<span data-ttu-id="20149-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="20149-147">The publisher of the app.</span></span> <span data-ttu-id="20149-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="20149-149">largeIcon</span></span>|[<span data-ttu-id="20149-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="20149-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="20149-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="20149-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="20149-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20149-153">createdDateTime</span></span>|<span data-ttu-id="20149-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20149-154">DateTimeOffset</span></span>|<span data-ttu-id="20149-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="20149-155">The date and time the app was created.</span></span> <span data-ttu-id="20149-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20149-157">lastModifiedDateTime</span></span>|<span data-ttu-id="20149-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20149-158">DateTimeOffset</span></span>|<span data-ttu-id="20149-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="20149-159">The date and time the app was last modified.</span></span> <span data-ttu-id="20149-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="20149-161">isFeatured</span></span>|<span data-ttu-id="20149-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="20149-162">Boolean</span></span>|<span data-ttu-id="20149-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="20149-164">privacyInformationUrl</span></span>|<span data-ttu-id="20149-165">String</span><span class="sxs-lookup"><span data-stu-id="20149-165">String</span></span>|<span data-ttu-id="20149-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="20149-166">The privacy statement Url.</span></span> <span data-ttu-id="20149-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="20149-168">informationUrl</span></span>|<span data-ttu-id="20149-169">String</span><span class="sxs-lookup"><span data-stu-id="20149-169">String</span></span>|<span data-ttu-id="20149-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="20149-170">The more information Url.</span></span> <span data-ttu-id="20149-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-172">owner</span><span class="sxs-lookup"><span data-stu-id="20149-172">owner</span></span>|<span data-ttu-id="20149-173">String</span><span class="sxs-lookup"><span data-stu-id="20149-173">String</span></span>|<span data-ttu-id="20149-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="20149-174">The owner of the app.</span></span> <span data-ttu-id="20149-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-176">developer</span><span class="sxs-lookup"><span data-stu-id="20149-176">developer</span></span>|<span data-ttu-id="20149-177">String</span><span class="sxs-lookup"><span data-stu-id="20149-177">String</span></span>|<span data-ttu-id="20149-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="20149-178">The developer of the app.</span></span> <span data-ttu-id="20149-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-180">notes</span><span class="sxs-lookup"><span data-stu-id="20149-180">notes</span></span>|<span data-ttu-id="20149-181">String</span><span class="sxs-lookup"><span data-stu-id="20149-181">String</span></span>|<span data-ttu-id="20149-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="20149-182">Notes for the app.</span></span> <span data-ttu-id="20149-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="20149-184">uploadState</span></span>|<span data-ttu-id="20149-185">Int32</span><span class="sxs-lookup"><span data-stu-id="20149-185">Int32</span></span>|<span data-ttu-id="20149-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="20149-186">The upload state.</span></span> <span data-ttu-id="20149-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="20149-188">publishingState</span></span>|[<span data-ttu-id="20149-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="20149-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="20149-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="20149-190">The publishing state for the app.</span></span> <span data-ttu-id="20149-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="20149-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="20149-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="20149-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="20149-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="20149-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="20149-194">isAssigned</span></span>|<span data-ttu-id="20149-195">Логический</span><span class="sxs-lookup"><span data-stu-id="20149-195">Boolean</span></span>|<span data-ttu-id="20149-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="20149-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="20149-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20149-198">roleScopeTagIds</span></span>|<span data-ttu-id="20149-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="20149-199">String collection</span></span>|<span data-ttu-id="20149-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="20149-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="20149-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20149-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="20149-202">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="20149-202">appStoreUrl</span></span>|<span data-ttu-id="20149-203">String</span><span class="sxs-lookup"><span data-stu-id="20149-203">String</span></span>|<span data-ttu-id="20149-204">Windows Phone 8.1 хранилища URL-адрес приложения.</span><span class="sxs-lookup"><span data-stu-id="20149-204">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="20149-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="20149-205">Response</span></span>
<span data-ttu-id="20149-206">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="20149-206">If successful, this method returns a `201 Created` response code and a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20149-207">Пример</span><span class="sxs-lookup"><span data-stu-id="20149-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="20149-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="20149-208">Request</span></span>
<span data-ttu-id="20149-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20149-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 748

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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="20149-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="20149-210">Response</span></span>
<span data-ttu-id="20149-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="20149-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 920

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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




