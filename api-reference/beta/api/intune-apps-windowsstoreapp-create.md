---
title: Создание Виндовсстореапп
description: Создание нового объекта Виндовсстореапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b2a06aeb7f24bce2da24fabfb0cce6e57fcc35b0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959777"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="d8666-103">Создание Виндовсстореапп</span><span class="sxs-lookup"><span data-stu-id="d8666-103">Create windowsStoreApp</span></span>

> <span data-ttu-id="d8666-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8666-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8666-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8666-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8666-106">Создание нового объекта [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d8666-106">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8666-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d8666-107">Prerequisites</span></span>
<span data-ttu-id="d8666-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8666-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8666-110">Permission type</span></span>|<span data-ttu-id="d8666-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8666-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8666-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8666-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8666-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8666-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8666-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8666-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8666-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8666-115">Not supported.</span></span>|
|<span data-ttu-id="d8666-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8666-116">Application</span></span>|<span data-ttu-id="d8666-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8666-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8666-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8666-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d8666-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8666-119">Request headers</span></span>
|<span data-ttu-id="d8666-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8666-120">Header</span></span>|<span data-ttu-id="d8666-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d8666-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8666-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8666-122">Authorization</span></span>|<span data-ttu-id="d8666-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8666-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8666-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d8666-124">Accept</span></span>|<span data-ttu-id="d8666-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8666-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8666-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8666-126">Request body</span></span>
<span data-ttu-id="d8666-127">В тексте запроса добавьте представление объекта Виндовсстореапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8666-127">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="d8666-128">В следующей таблице приведены свойства, необходимые при создании Виндовсстореапп.</span><span class="sxs-lookup"><span data-stu-id="d8666-128">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="d8666-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8666-129">Property</span></span>|<span data-ttu-id="d8666-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d8666-130">Type</span></span>|<span data-ttu-id="d8666-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d8666-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8666-132">id</span><span class="sxs-lookup"><span data-stu-id="d8666-132">id</span></span>|<span data-ttu-id="d8666-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d8666-133">String</span></span>|<span data-ttu-id="d8666-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d8666-134">Key of the entity.</span></span> <span data-ttu-id="d8666-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d8666-136">displayName</span></span>|<span data-ttu-id="d8666-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d8666-137">String</span></span>|<span data-ttu-id="d8666-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d8666-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d8666-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-140">description</span><span class="sxs-lookup"><span data-stu-id="d8666-140">description</span></span>|<span data-ttu-id="d8666-141">Строка</span><span class="sxs-lookup"><span data-stu-id="d8666-141">String</span></span>|<span data-ttu-id="d8666-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d8666-142">The description of the app.</span></span> <span data-ttu-id="d8666-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-144">publisher</span><span class="sxs-lookup"><span data-stu-id="d8666-144">publisher</span></span>|<span data-ttu-id="d8666-145">String</span><span class="sxs-lookup"><span data-stu-id="d8666-145">String</span></span>|<span data-ttu-id="d8666-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d8666-146">The publisher of the app.</span></span> <span data-ttu-id="d8666-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d8666-148">largeIcon</span></span>|[<span data-ttu-id="d8666-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d8666-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d8666-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d8666-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d8666-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8666-152">createdDateTime</span></span>|<span data-ttu-id="d8666-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8666-153">DateTimeOffset</span></span>|<span data-ttu-id="d8666-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d8666-154">The date and time the app was created.</span></span> <span data-ttu-id="d8666-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8666-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d8666-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8666-157">DateTimeOffset</span></span>|<span data-ttu-id="d8666-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d8666-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d8666-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d8666-160">isFeatured</span></span>|<span data-ttu-id="d8666-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8666-161">Boolean</span></span>|<span data-ttu-id="d8666-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d8666-163">privacyInformationUrl</span></span>|<span data-ttu-id="d8666-164">String</span><span class="sxs-lookup"><span data-stu-id="d8666-164">String</span></span>|<span data-ttu-id="d8666-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d8666-165">The privacy statement Url.</span></span> <span data-ttu-id="d8666-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d8666-167">informationUrl</span></span>|<span data-ttu-id="d8666-168">String</span><span class="sxs-lookup"><span data-stu-id="d8666-168">String</span></span>|<span data-ttu-id="d8666-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d8666-169">The more information Url.</span></span> <span data-ttu-id="d8666-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-171">owner</span><span class="sxs-lookup"><span data-stu-id="d8666-171">owner</span></span>|<span data-ttu-id="d8666-172">String</span><span class="sxs-lookup"><span data-stu-id="d8666-172">String</span></span>|<span data-ttu-id="d8666-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d8666-173">The owner of the app.</span></span> <span data-ttu-id="d8666-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-175">developer</span><span class="sxs-lookup"><span data-stu-id="d8666-175">developer</span></span>|<span data-ttu-id="d8666-176">String</span><span class="sxs-lookup"><span data-stu-id="d8666-176">String</span></span>|<span data-ttu-id="d8666-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d8666-177">The developer of the app.</span></span> <span data-ttu-id="d8666-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-179">notes</span><span class="sxs-lookup"><span data-stu-id="d8666-179">notes</span></span>|<span data-ttu-id="d8666-180">String</span><span class="sxs-lookup"><span data-stu-id="d8666-180">String</span></span>|<span data-ttu-id="d8666-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="d8666-181">Notes for the app.</span></span> <span data-ttu-id="d8666-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="d8666-183">uploadState</span></span>|<span data-ttu-id="d8666-184">Int32</span><span class="sxs-lookup"><span data-stu-id="d8666-184">Int32</span></span>|<span data-ttu-id="d8666-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="d8666-185">The upload state.</span></span> <span data-ttu-id="d8666-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="d8666-187">publishingState</span></span>|[<span data-ttu-id="d8666-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="d8666-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d8666-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="d8666-189">The publishing state for the app.</span></span> <span data-ttu-id="d8666-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d8666-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d8666-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d8666-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d8666-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d8666-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d8666-193">isAssigned</span></span>|<span data-ttu-id="d8666-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8666-194">Boolean</span></span>|<span data-ttu-id="d8666-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="d8666-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d8666-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8666-197">roleScopeTagIds</span></span>|<span data-ttu-id="d8666-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d8666-198">String collection</span></span>|<span data-ttu-id="d8666-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d8666-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d8666-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="d8666-201">dependentAppCount</span></span>|<span data-ttu-id="d8666-202">Int32</span><span class="sxs-lookup"><span data-stu-id="d8666-202">Int32</span></span>|<span data-ttu-id="d8666-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="d8666-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d8666-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8666-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d8666-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d8666-205">appStoreUrl</span></span>|<span data-ttu-id="d8666-206">String</span><span class="sxs-lookup"><span data-stu-id="d8666-206">String</span></span>|<span data-ttu-id="d8666-207">URL-адрес хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="d8666-207">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="d8666-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8666-208">Response</span></span>
<span data-ttu-id="d8666-209">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8666-209">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8666-210">Пример</span><span class="sxs-lookup"><span data-stu-id="d8666-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8666-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8666-211">Request</span></span>
<span data-ttu-id="d8666-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8666-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d8666-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8666-213">Response</span></span>
<span data-ttu-id="d8666-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8666-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





