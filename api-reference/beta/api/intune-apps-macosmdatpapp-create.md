---
title: Создание Макосмдатпапп
description: Создание нового объекта Макосмдатпапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d35e57aea572ec1a603283b49210763a6b93ba6
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792095"
---
# <a name="create-macosmdatpapp"></a><span data-ttu-id="47c43-103">Создание Макосмдатпапп</span><span class="sxs-lookup"><span data-stu-id="47c43-103">Create macOSMdatpApp</span></span>

<span data-ttu-id="47c43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47c43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47c43-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47c43-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47c43-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47c43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47c43-107">Создание нового объекта [макосмдатпапп](../resources/intune-apps-macosmdatpapp.md) .</span><span class="sxs-lookup"><span data-stu-id="47c43-107">Create a new [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47c43-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="47c43-108">Prerequisites</span></span>
<span data-ttu-id="47c43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47c43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47c43-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47c43-111">Permission type</span></span>|<span data-ttu-id="47c43-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47c43-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47c43-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47c43-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47c43-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c43-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="47c43-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47c43-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47c43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47c43-116">Not supported.</span></span>|
|<span data-ttu-id="47c43-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="47c43-117">Application</span></span>|<span data-ttu-id="47c43-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c43-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47c43-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47c43-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="47c43-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="47c43-120">Request headers</span></span>
|<span data-ttu-id="47c43-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47c43-121">Header</span></span>|<span data-ttu-id="47c43-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47c43-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47c43-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47c43-123">Authorization</span></span>|<span data-ttu-id="47c43-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47c43-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47c43-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47c43-125">Accept</span></span>|<span data-ttu-id="47c43-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47c43-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47c43-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47c43-127">Request body</span></span>
<span data-ttu-id="47c43-128">В тексте запроса добавьте представление объекта Макосмдатпапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47c43-128">In the request body, supply a JSON representation for the macOSMdatpApp object.</span></span>

<span data-ttu-id="47c43-129">В следующей таблице приведены свойства, необходимые при создании Макосмдатпапп.</span><span class="sxs-lookup"><span data-stu-id="47c43-129">The following table shows the properties that are required when you create the macOSMdatpApp.</span></span>

|<span data-ttu-id="47c43-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="47c43-130">Property</span></span>|<span data-ttu-id="47c43-131">Тип</span><span class="sxs-lookup"><span data-stu-id="47c43-131">Type</span></span>|<span data-ttu-id="47c43-132">Описание</span><span class="sxs-lookup"><span data-stu-id="47c43-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47c43-133">id</span><span class="sxs-lookup"><span data-stu-id="47c43-133">id</span></span>|<span data-ttu-id="47c43-134">String</span><span class="sxs-lookup"><span data-stu-id="47c43-134">String</span></span>|<span data-ttu-id="47c43-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47c43-135">Key of the entity.</span></span> <span data-ttu-id="47c43-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-137">displayName</span><span class="sxs-lookup"><span data-stu-id="47c43-137">displayName</span></span>|<span data-ttu-id="47c43-138">String</span><span class="sxs-lookup"><span data-stu-id="47c43-138">String</span></span>|<span data-ttu-id="47c43-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="47c43-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="47c43-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-141">description</span><span class="sxs-lookup"><span data-stu-id="47c43-141">description</span></span>|<span data-ttu-id="47c43-142">String</span><span class="sxs-lookup"><span data-stu-id="47c43-142">String</span></span>|<span data-ttu-id="47c43-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="47c43-143">The description of the app.</span></span> <span data-ttu-id="47c43-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-145">publisher</span><span class="sxs-lookup"><span data-stu-id="47c43-145">publisher</span></span>|<span data-ttu-id="47c43-146">String</span><span class="sxs-lookup"><span data-stu-id="47c43-146">String</span></span>|<span data-ttu-id="47c43-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="47c43-147">The publisher of the app.</span></span> <span data-ttu-id="47c43-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="47c43-149">largeIcon</span></span>|[<span data-ttu-id="47c43-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="47c43-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="47c43-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="47c43-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="47c43-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47c43-153">createdDateTime</span></span>|<span data-ttu-id="47c43-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47c43-154">DateTimeOffset</span></span>|<span data-ttu-id="47c43-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="47c43-155">The date and time the app was created.</span></span> <span data-ttu-id="47c43-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47c43-157">lastModifiedDateTime</span></span>|<span data-ttu-id="47c43-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47c43-158">DateTimeOffset</span></span>|<span data-ttu-id="47c43-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="47c43-159">The date and time the app was last modified.</span></span> <span data-ttu-id="47c43-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="47c43-161">isFeatured</span></span>|<span data-ttu-id="47c43-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="47c43-162">Boolean</span></span>|<span data-ttu-id="47c43-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="47c43-164">privacyInformationUrl</span></span>|<span data-ttu-id="47c43-165">String</span><span class="sxs-lookup"><span data-stu-id="47c43-165">String</span></span>|<span data-ttu-id="47c43-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="47c43-166">The privacy statement Url.</span></span> <span data-ttu-id="47c43-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="47c43-168">informationUrl</span></span>|<span data-ttu-id="47c43-169">String</span><span class="sxs-lookup"><span data-stu-id="47c43-169">String</span></span>|<span data-ttu-id="47c43-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="47c43-170">The more information Url.</span></span> <span data-ttu-id="47c43-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-172">owner</span><span class="sxs-lookup"><span data-stu-id="47c43-172">owner</span></span>|<span data-ttu-id="47c43-173">String</span><span class="sxs-lookup"><span data-stu-id="47c43-173">String</span></span>|<span data-ttu-id="47c43-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="47c43-174">The owner of the app.</span></span> <span data-ttu-id="47c43-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-176">developer</span><span class="sxs-lookup"><span data-stu-id="47c43-176">developer</span></span>|<span data-ttu-id="47c43-177">String</span><span class="sxs-lookup"><span data-stu-id="47c43-177">String</span></span>|<span data-ttu-id="47c43-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="47c43-178">The developer of the app.</span></span> <span data-ttu-id="47c43-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-180">notes</span><span class="sxs-lookup"><span data-stu-id="47c43-180">notes</span></span>|<span data-ttu-id="47c43-181">String</span><span class="sxs-lookup"><span data-stu-id="47c43-181">String</span></span>|<span data-ttu-id="47c43-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="47c43-182">Notes for the app.</span></span> <span data-ttu-id="47c43-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="47c43-184">uploadState</span></span>|<span data-ttu-id="47c43-185">Int32</span><span class="sxs-lookup"><span data-stu-id="47c43-185">Int32</span></span>|<span data-ttu-id="47c43-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="47c43-186">The upload state.</span></span> <span data-ttu-id="47c43-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="47c43-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="47c43-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="47c43-189">publishingState</span></span>|[<span data-ttu-id="47c43-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="47c43-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="47c43-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="47c43-191">The publishing state for the app.</span></span> <span data-ttu-id="47c43-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="47c43-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="47c43-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="47c43-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="47c43-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="47c43-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="47c43-195">isAssigned</span></span>|<span data-ttu-id="47c43-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="47c43-196">Boolean</span></span>|<span data-ttu-id="47c43-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="47c43-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="47c43-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47c43-199">roleScopeTagIds</span></span>|<span data-ttu-id="47c43-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="47c43-200">String collection</span></span>|<span data-ttu-id="47c43-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="47c43-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="47c43-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="47c43-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="47c43-203">dependentAppCount</span></span>|<span data-ttu-id="47c43-204">Int32</span><span class="sxs-lookup"><span data-stu-id="47c43-204">Int32</span></span>|<span data-ttu-id="47c43-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="47c43-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="47c43-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="47c43-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="47c43-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="47c43-207">Response</span></span>
<span data-ttu-id="47c43-208">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосмдатпапп](../resources/intune-apps-macosmdatpapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47c43-208">If successful, this method returns a `201 Created` response code and a [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47c43-209">Пример</span><span class="sxs-lookup"><span data-stu-id="47c43-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="47c43-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="47c43-210">Request</span></span>
<span data-ttu-id="47c43-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47c43-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 712

{
  "@odata.type": "#microsoft.graph.macOSMdatpApp",
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

### <a name="response"></a><span data-ttu-id="47c43-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="47c43-212">Response</span></span>
<span data-ttu-id="47c43-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47c43-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 884

{
  "@odata.type": "#microsoft.graph.macOSMdatpApp",
  "id": "2963b007-b007-2963-07b0-632907b06329",
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



