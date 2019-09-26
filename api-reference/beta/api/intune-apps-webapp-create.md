---
title: Create webApp
description: Создание объекта webApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d45c9a99931190b844cf607b15c588b95e1e055
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37172186"
---
# <a name="create-webapp"></a><span data-ttu-id="3357a-103">Create webApp</span><span class="sxs-lookup"><span data-stu-id="3357a-103">Create webApp</span></span>

> <span data-ttu-id="3357a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3357a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3357a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3357a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3357a-106">Создание объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-106">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3357a-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3357a-107">Prerequisites</span></span>
<span data-ttu-id="3357a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3357a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3357a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3357a-110">Permission type</span></span>|<span data-ttu-id="3357a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3357a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3357a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3357a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3357a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3357a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3357a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3357a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3357a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3357a-115">Not supported.</span></span>|
|<span data-ttu-id="3357a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3357a-116">Application</span></span>|<span data-ttu-id="3357a-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3357a-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3357a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3357a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3357a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3357a-119">Request headers</span></span>
|<span data-ttu-id="3357a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3357a-120">Header</span></span>|<span data-ttu-id="3357a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3357a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3357a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3357a-122">Authorization</span></span>|<span data-ttu-id="3357a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3357a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3357a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3357a-124">Accept</span></span>|<span data-ttu-id="3357a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3357a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3357a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3357a-126">Request body</span></span>
<span data-ttu-id="3357a-127">В теле запроса добавьте представление объекта webApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3357a-127">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="3357a-128">Ниже показаны свойства, которые необходимо указывать при создании объекта webApp.</span><span class="sxs-lookup"><span data-stu-id="3357a-128">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="3357a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3357a-129">Property</span></span>|<span data-ttu-id="3357a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3357a-130">Type</span></span>|<span data-ttu-id="3357a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3357a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3357a-132">id</span><span class="sxs-lookup"><span data-stu-id="3357a-132">id</span></span>|<span data-ttu-id="3357a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="3357a-133">String</span></span>|<span data-ttu-id="3357a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3357a-134">Key of the entity.</span></span> <span data-ttu-id="3357a-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3357a-136">displayName</span></span>|<span data-ttu-id="3357a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3357a-137">String</span></span>|<span data-ttu-id="3357a-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="3357a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3357a-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-140">description</span><span class="sxs-lookup"><span data-stu-id="3357a-140">description</span></span>|<span data-ttu-id="3357a-141">Строка</span><span class="sxs-lookup"><span data-stu-id="3357a-141">String</span></span>|<span data-ttu-id="3357a-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="3357a-142">The description of the app.</span></span> <span data-ttu-id="3357a-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-144">publisher</span><span class="sxs-lookup"><span data-stu-id="3357a-144">publisher</span></span>|<span data-ttu-id="3357a-145">String.</span><span class="sxs-lookup"><span data-stu-id="3357a-145">String</span></span>|<span data-ttu-id="3357a-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="3357a-146">The publisher of the app.</span></span> <span data-ttu-id="3357a-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3357a-148">largeIcon</span></span>|[<span data-ttu-id="3357a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3357a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3357a-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="3357a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3357a-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3357a-152">createdDateTime</span></span>|<span data-ttu-id="3357a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3357a-153">DateTimeOffset</span></span>|<span data-ttu-id="3357a-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="3357a-154">The date and time the app was created.</span></span> <span data-ttu-id="3357a-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3357a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3357a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3357a-157">DateTimeOffset</span></span>|<span data-ttu-id="3357a-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="3357a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3357a-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3357a-160">isFeatured</span></span>|<span data-ttu-id="3357a-161">Boolean.</span><span class="sxs-lookup"><span data-stu-id="3357a-161">Boolean</span></span>|<span data-ttu-id="3357a-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3357a-163">privacyInformationUrl</span></span>|<span data-ttu-id="3357a-164">String.</span><span class="sxs-lookup"><span data-stu-id="3357a-164">String</span></span>|<span data-ttu-id="3357a-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3357a-165">The privacy statement Url.</span></span> <span data-ttu-id="3357a-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3357a-167">informationUrl</span></span>|<span data-ttu-id="3357a-168">String.</span><span class="sxs-lookup"><span data-stu-id="3357a-168">String</span></span>|<span data-ttu-id="3357a-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3357a-169">The more information Url.</span></span> <span data-ttu-id="3357a-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-171">owner</span><span class="sxs-lookup"><span data-stu-id="3357a-171">owner</span></span>|<span data-ttu-id="3357a-172">String</span><span class="sxs-lookup"><span data-stu-id="3357a-172">String</span></span>|<span data-ttu-id="3357a-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="3357a-173">The owner of the app.</span></span> <span data-ttu-id="3357a-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-175">developer</span><span class="sxs-lookup"><span data-stu-id="3357a-175">developer</span></span>|<span data-ttu-id="3357a-176">String.</span><span class="sxs-lookup"><span data-stu-id="3357a-176">String</span></span>|<span data-ttu-id="3357a-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="3357a-177">The developer of the app.</span></span> <span data-ttu-id="3357a-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-179">notes</span><span class="sxs-lookup"><span data-stu-id="3357a-179">notes</span></span>|<span data-ttu-id="3357a-180">String.</span><span class="sxs-lookup"><span data-stu-id="3357a-180">String</span></span>|<span data-ttu-id="3357a-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="3357a-181">Notes for the app.</span></span> <span data-ttu-id="3357a-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="3357a-183">uploadState</span></span>|<span data-ttu-id="3357a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3357a-184">Int32</span></span>|<span data-ttu-id="3357a-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="3357a-185">The upload state.</span></span> <span data-ttu-id="3357a-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="3357a-187">publishingState</span></span>|[<span data-ttu-id="3357a-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="3357a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3357a-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="3357a-189">The publishing state for the app.</span></span> <span data-ttu-id="3357a-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="3357a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3357a-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="3357a-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3357a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3357a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3357a-193">isAssigned</span></span>|<span data-ttu-id="3357a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3357a-194">Boolean</span></span>|<span data-ttu-id="3357a-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="3357a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3357a-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3357a-197">roleScopeTagIds</span></span>|<span data-ttu-id="3357a-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3357a-198">String collection</span></span>|<span data-ttu-id="3357a-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="3357a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3357a-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="3357a-201">dependentAppCount</span></span>|<span data-ttu-id="3357a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="3357a-202">Int32</span></span>|<span data-ttu-id="3357a-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="3357a-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="3357a-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3357a-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3357a-205">appUrl</span><span class="sxs-lookup"><span data-stu-id="3357a-205">appUrl</span></span>|<span data-ttu-id="3357a-206">String</span><span class="sxs-lookup"><span data-stu-id="3357a-206">String</span></span>|<span data-ttu-id="3357a-207">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="3357a-207">The web app URL.</span></span>|
|<span data-ttu-id="3357a-208">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="3357a-208">useManagedBrowser</span></span>|<span data-ttu-id="3357a-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="3357a-209">Boolean</span></span>|<span data-ttu-id="3357a-210">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="3357a-210">Whether or not to use managed browser.</span></span> <span data-ttu-id="3357a-211">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="3357a-211">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="3357a-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="3357a-212">Response</span></span>
<span data-ttu-id="3357a-213">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [webApp](../resources/intune-apps-webapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3357a-213">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3357a-214">Пример</span><span class="sxs-lookup"><span data-stu-id="3357a-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="3357a-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="3357a-215">Request</span></span>
<span data-ttu-id="3357a-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3357a-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3357a-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="3357a-217">Response</span></span>
<span data-ttu-id="3357a-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3357a-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




