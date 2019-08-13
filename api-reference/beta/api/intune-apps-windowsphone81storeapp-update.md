---
title: Обновление windowsPhone81StoreApp
description: Обновление свойств объекта windowsPhone81StoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c8a85388bce5c9a678b97059e24f7bd83039ae83
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328678"
---
# <a name="update-windowsphone81storeapp"></a><span data-ttu-id="9b787-103">Обновление windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="9b787-103">Update windowsPhone81StoreApp</span></span>

> <span data-ttu-id="9b787-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b787-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b787-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b787-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b787-106">Обновление свойств объекта [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9b787-106">Update the properties of a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b787-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b787-107">Prerequisites</span></span>
<span data-ttu-id="9b787-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b787-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b787-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b787-110">Permission type</span></span>|<span data-ttu-id="9b787-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b787-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b787-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b787-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b787-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b787-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9b787-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b787-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b787-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b787-115">Not supported.</span></span>|
|<span data-ttu-id="9b787-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b787-116">Application</span></span>|<span data-ttu-id="9b787-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b787-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b787-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b787-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9b787-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b787-119">Request headers</span></span>
|<span data-ttu-id="9b787-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b787-120">Header</span></span>|<span data-ttu-id="9b787-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9b787-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b787-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b787-122">Authorization</span></span>|<span data-ttu-id="9b787-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b787-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b787-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9b787-124">Accept</span></span>|<span data-ttu-id="9b787-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b787-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b787-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9b787-126">Request body</span></span>
<span data-ttu-id="9b787-127">В тексте запроса добавьте представление объекта [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b787-127">In the request body, supply a JSON representation for the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

<span data-ttu-id="9b787-128">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-128">The following table shows the properties that are required when you create the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span></span>

|<span data-ttu-id="9b787-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b787-129">Property</span></span>|<span data-ttu-id="9b787-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9b787-130">Type</span></span>|<span data-ttu-id="9b787-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9b787-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b787-132">id</span><span class="sxs-lookup"><span data-stu-id="9b787-132">id</span></span>|<span data-ttu-id="9b787-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9b787-133">String</span></span>|<span data-ttu-id="9b787-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9b787-134">Key of the entity.</span></span> <span data-ttu-id="9b787-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9b787-136">displayName</span></span>|<span data-ttu-id="9b787-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9b787-137">String</span></span>|<span data-ttu-id="9b787-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9b787-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9b787-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-140">description</span><span class="sxs-lookup"><span data-stu-id="9b787-140">description</span></span>|<span data-ttu-id="9b787-141">Строка</span><span class="sxs-lookup"><span data-stu-id="9b787-141">String</span></span>|<span data-ttu-id="9b787-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9b787-142">The description of the app.</span></span> <span data-ttu-id="9b787-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9b787-144">publisher</span></span>|<span data-ttu-id="9b787-145">String</span><span class="sxs-lookup"><span data-stu-id="9b787-145">String</span></span>|<span data-ttu-id="9b787-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9b787-146">The publisher of the app.</span></span> <span data-ttu-id="9b787-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9b787-148">largeIcon</span></span>|[<span data-ttu-id="9b787-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9b787-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9b787-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9b787-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9b787-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b787-152">createdDateTime</span></span>|<span data-ttu-id="9b787-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b787-153">DateTimeOffset</span></span>|<span data-ttu-id="9b787-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9b787-154">The date and time the app was created.</span></span> <span data-ttu-id="9b787-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b787-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9b787-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b787-157">DateTimeOffset</span></span>|<span data-ttu-id="9b787-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9b787-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9b787-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9b787-160">isFeatured</span></span>|<span data-ttu-id="9b787-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b787-161">Boolean</span></span>|<span data-ttu-id="9b787-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9b787-163">privacyInformationUrl</span></span>|<span data-ttu-id="9b787-164">String</span><span class="sxs-lookup"><span data-stu-id="9b787-164">String</span></span>|<span data-ttu-id="9b787-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9b787-165">The privacy statement Url.</span></span> <span data-ttu-id="9b787-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9b787-167">informationUrl</span></span>|<span data-ttu-id="9b787-168">String</span><span class="sxs-lookup"><span data-stu-id="9b787-168">String</span></span>|<span data-ttu-id="9b787-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9b787-169">The more information Url.</span></span> <span data-ttu-id="9b787-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-171">owner</span><span class="sxs-lookup"><span data-stu-id="9b787-171">owner</span></span>|<span data-ttu-id="9b787-172">String</span><span class="sxs-lookup"><span data-stu-id="9b787-172">String</span></span>|<span data-ttu-id="9b787-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9b787-173">The owner of the app.</span></span> <span data-ttu-id="9b787-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-175">developer</span><span class="sxs-lookup"><span data-stu-id="9b787-175">developer</span></span>|<span data-ttu-id="9b787-176">String</span><span class="sxs-lookup"><span data-stu-id="9b787-176">String</span></span>|<span data-ttu-id="9b787-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9b787-177">The developer of the app.</span></span> <span data-ttu-id="9b787-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-179">notes</span><span class="sxs-lookup"><span data-stu-id="9b787-179">notes</span></span>|<span data-ttu-id="9b787-180">String</span><span class="sxs-lookup"><span data-stu-id="9b787-180">String</span></span>|<span data-ttu-id="9b787-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9b787-181">Notes for the app.</span></span> <span data-ttu-id="9b787-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9b787-183">uploadState</span></span>|<span data-ttu-id="9b787-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9b787-184">Int32</span></span>|<span data-ttu-id="9b787-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="9b787-185">The upload state.</span></span> <span data-ttu-id="9b787-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9b787-187">publishingState</span></span>|[<span data-ttu-id="9b787-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9b787-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9b787-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="9b787-189">The publishing state for the app.</span></span> <span data-ttu-id="9b787-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9b787-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9b787-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9b787-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9b787-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9b787-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9b787-193">isAssigned</span></span>|<span data-ttu-id="9b787-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b787-194">Boolean</span></span>|<span data-ttu-id="9b787-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="9b787-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9b787-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9b787-197">roleScopeTagIds</span></span>|<span data-ttu-id="9b787-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9b787-198">String collection</span></span>|<span data-ttu-id="9b787-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9b787-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9b787-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="9b787-201">dependentAppCount</span></span>|<span data-ttu-id="9b787-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9b787-202">Int32</span></span>|<span data-ttu-id="9b787-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="9b787-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9b787-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b787-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b787-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9b787-205">appStoreUrl</span></span>|<span data-ttu-id="9b787-206">String</span><span class="sxs-lookup"><span data-stu-id="9b787-206">String</span></span>|<span data-ttu-id="9b787-207">URL-адрес магазина приложений Windows Phone 8,1.</span><span class="sxs-lookup"><span data-stu-id="9b787-207">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="9b787-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b787-208">Response</span></span>
<span data-ttu-id="9b787-209">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b787-209">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b787-210">Пример</span><span class="sxs-lookup"><span data-stu-id="9b787-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b787-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b787-211">Request</span></span>
<span data-ttu-id="9b787-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b787-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9b787-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b787-213">Response</span></span>
<span data-ttu-id="9b787-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b787-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






