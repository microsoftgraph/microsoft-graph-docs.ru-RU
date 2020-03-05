---
title: Create webApp
description: Создание объекта webApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 425933e759e0c30483c70d7ff29182337266d476
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444870"
---
# <a name="create-webapp"></a><span data-ttu-id="1008b-103">Create webApp</span><span class="sxs-lookup"><span data-stu-id="1008b-103">Create webApp</span></span>

<span data-ttu-id="1008b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1008b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1008b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1008b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1008b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1008b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1008b-107">Создание объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-107">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1008b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1008b-108">Prerequisites</span></span>
<span data-ttu-id="1008b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1008b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1008b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1008b-111">Permission type</span></span>|<span data-ttu-id="1008b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1008b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1008b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1008b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1008b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1008b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1008b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1008b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1008b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1008b-116">Not supported.</span></span>|
|<span data-ttu-id="1008b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1008b-117">Application</span></span>|<span data-ttu-id="1008b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1008b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1008b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1008b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1008b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1008b-120">Request headers</span></span>
|<span data-ttu-id="1008b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1008b-121">Header</span></span>|<span data-ttu-id="1008b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1008b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1008b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1008b-123">Authorization</span></span>|<span data-ttu-id="1008b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1008b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1008b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1008b-125">Accept</span></span>|<span data-ttu-id="1008b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1008b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1008b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1008b-127">Request body</span></span>
<span data-ttu-id="1008b-128">В теле запроса добавьте представление объекта webApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1008b-128">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="1008b-129">Ниже показаны свойства, которые необходимо указывать при создании объекта webApp.</span><span class="sxs-lookup"><span data-stu-id="1008b-129">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="1008b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1008b-130">Property</span></span>|<span data-ttu-id="1008b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1008b-131">Type</span></span>|<span data-ttu-id="1008b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1008b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1008b-133">id</span><span class="sxs-lookup"><span data-stu-id="1008b-133">id</span></span>|<span data-ttu-id="1008b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1008b-134">String</span></span>|<span data-ttu-id="1008b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1008b-135">Key of the entity.</span></span> <span data-ttu-id="1008b-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1008b-137">displayName</span></span>|<span data-ttu-id="1008b-138">Строка</span><span class="sxs-lookup"><span data-stu-id="1008b-138">String</span></span>|<span data-ttu-id="1008b-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="1008b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1008b-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-141">description</span><span class="sxs-lookup"><span data-stu-id="1008b-141">description</span></span>|<span data-ttu-id="1008b-142">Строка</span><span class="sxs-lookup"><span data-stu-id="1008b-142">String</span></span>|<span data-ttu-id="1008b-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="1008b-143">The description of the app.</span></span> <span data-ttu-id="1008b-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-145">publisher</span><span class="sxs-lookup"><span data-stu-id="1008b-145">publisher</span></span>|<span data-ttu-id="1008b-146">String</span><span class="sxs-lookup"><span data-stu-id="1008b-146">String</span></span>|<span data-ttu-id="1008b-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="1008b-147">The publisher of the app.</span></span> <span data-ttu-id="1008b-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1008b-149">largeIcon</span></span>|[<span data-ttu-id="1008b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1008b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1008b-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="1008b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1008b-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1008b-153">createdDateTime</span></span>|<span data-ttu-id="1008b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1008b-154">DateTimeOffset</span></span>|<span data-ttu-id="1008b-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="1008b-155">The date and time the app was created.</span></span> <span data-ttu-id="1008b-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1008b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1008b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1008b-158">DateTimeOffset</span></span>|<span data-ttu-id="1008b-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="1008b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1008b-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1008b-161">isFeatured</span></span>|<span data-ttu-id="1008b-162">Логический</span><span class="sxs-lookup"><span data-stu-id="1008b-162">Boolean</span></span>|<span data-ttu-id="1008b-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1008b-164">privacyInformationUrl</span></span>|<span data-ttu-id="1008b-165">String</span><span class="sxs-lookup"><span data-stu-id="1008b-165">String</span></span>|<span data-ttu-id="1008b-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="1008b-166">The privacy statement Url.</span></span> <span data-ttu-id="1008b-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1008b-168">informationUrl</span></span>|<span data-ttu-id="1008b-169">String</span><span class="sxs-lookup"><span data-stu-id="1008b-169">String</span></span>|<span data-ttu-id="1008b-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="1008b-170">The more information Url.</span></span> <span data-ttu-id="1008b-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-172">owner</span><span class="sxs-lookup"><span data-stu-id="1008b-172">owner</span></span>|<span data-ttu-id="1008b-173">String</span><span class="sxs-lookup"><span data-stu-id="1008b-173">String</span></span>|<span data-ttu-id="1008b-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="1008b-174">The owner of the app.</span></span> <span data-ttu-id="1008b-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-176">developer</span><span class="sxs-lookup"><span data-stu-id="1008b-176">developer</span></span>|<span data-ttu-id="1008b-177">String</span><span class="sxs-lookup"><span data-stu-id="1008b-177">String</span></span>|<span data-ttu-id="1008b-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="1008b-178">The developer of the app.</span></span> <span data-ttu-id="1008b-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-180">notes</span><span class="sxs-lookup"><span data-stu-id="1008b-180">notes</span></span>|<span data-ttu-id="1008b-181">String</span><span class="sxs-lookup"><span data-stu-id="1008b-181">String</span></span>|<span data-ttu-id="1008b-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="1008b-182">Notes for the app.</span></span> <span data-ttu-id="1008b-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1008b-184">uploadState</span></span>|<span data-ttu-id="1008b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1008b-185">Int32</span></span>|<span data-ttu-id="1008b-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="1008b-186">The upload state.</span></span> <span data-ttu-id="1008b-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1008b-188">publishingState</span></span>|[<span data-ttu-id="1008b-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="1008b-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1008b-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="1008b-190">The publishing state for the app.</span></span> <span data-ttu-id="1008b-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="1008b-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1008b-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="1008b-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1008b-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1008b-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1008b-194">isAssigned</span></span>|<span data-ttu-id="1008b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1008b-195">Boolean</span></span>|<span data-ttu-id="1008b-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="1008b-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1008b-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1008b-198">roleScopeTagIds</span></span>|<span data-ttu-id="1008b-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1008b-199">String collection</span></span>|<span data-ttu-id="1008b-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="1008b-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1008b-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="1008b-202">dependentAppCount</span></span>|<span data-ttu-id="1008b-203">Int32</span><span class="sxs-lookup"><span data-stu-id="1008b-203">Int32</span></span>|<span data-ttu-id="1008b-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="1008b-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="1008b-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1008b-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1008b-206">appUrl</span><span class="sxs-lookup"><span data-stu-id="1008b-206">appUrl</span></span>|<span data-ttu-id="1008b-207">String</span><span class="sxs-lookup"><span data-stu-id="1008b-207">String</span></span>|<span data-ttu-id="1008b-208">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="1008b-208">The web app URL.</span></span>|
|<span data-ttu-id="1008b-209">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="1008b-209">useManagedBrowser</span></span>|<span data-ttu-id="1008b-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="1008b-210">Boolean</span></span>|<span data-ttu-id="1008b-211">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="1008b-211">Whether or not to use managed browser.</span></span> <span data-ttu-id="1008b-212">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="1008b-212">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="1008b-213">Ответ</span><span class="sxs-lookup"><span data-stu-id="1008b-213">Response</span></span>
<span data-ttu-id="1008b-214">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [webApp](../resources/intune-apps-webapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1008b-214">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1008b-215">Пример</span><span class="sxs-lookup"><span data-stu-id="1008b-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="1008b-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="1008b-216">Request</span></span>
<span data-ttu-id="1008b-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1008b-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1008b-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="1008b-218">Response</span></span>
<span data-ttu-id="1008b-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1008b-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





