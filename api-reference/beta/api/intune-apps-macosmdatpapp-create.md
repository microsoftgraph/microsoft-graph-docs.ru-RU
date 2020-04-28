---
title: Создание Макосмдатпапп
description: Создание нового объекта Макосмдатпапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ebdb3cf7892c8e268695d4df1f721a96078e655
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394153"
---
# <a name="create-macosmdatpapp"></a><span data-ttu-id="9d442-103">Создание Макосмдатпапп</span><span class="sxs-lookup"><span data-stu-id="9d442-103">Create macOSMdatpApp</span></span>

<span data-ttu-id="9d442-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d442-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d442-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d442-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d442-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d442-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d442-107">Создание нового объекта [макосмдатпапп](../resources/intune-apps-macosmdatpapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9d442-107">Create a new [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d442-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9d442-108">Prerequisites</span></span>
<span data-ttu-id="9d442-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d442-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d442-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d442-111">Permission type</span></span>|<span data-ttu-id="9d442-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d442-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d442-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d442-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d442-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d442-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9d442-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d442-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d442-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d442-116">Not supported.</span></span>|
|<span data-ttu-id="9d442-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d442-117">Application</span></span>|<span data-ttu-id="9d442-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d442-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d442-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d442-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9d442-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9d442-120">Request headers</span></span>
|<span data-ttu-id="9d442-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d442-121">Header</span></span>|<span data-ttu-id="9d442-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9d442-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d442-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d442-123">Authorization</span></span>|<span data-ttu-id="9d442-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d442-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d442-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d442-125">Accept</span></span>|<span data-ttu-id="9d442-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d442-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d442-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9d442-127">Request body</span></span>
<span data-ttu-id="9d442-128">В тексте запроса добавьте представление объекта Макосмдатпапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d442-128">In the request body, supply a JSON representation for the macOSMdatpApp object.</span></span>

<span data-ttu-id="9d442-129">В следующей таблице приведены свойства, необходимые при создании Макосмдатпапп.</span><span class="sxs-lookup"><span data-stu-id="9d442-129">The following table shows the properties that are required when you create the macOSMdatpApp.</span></span>

|<span data-ttu-id="9d442-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d442-130">Property</span></span>|<span data-ttu-id="9d442-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9d442-131">Type</span></span>|<span data-ttu-id="9d442-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9d442-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d442-133">id</span><span class="sxs-lookup"><span data-stu-id="9d442-133">id</span></span>|<span data-ttu-id="9d442-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9d442-134">String</span></span>|<span data-ttu-id="9d442-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9d442-135">Key of the entity.</span></span> <span data-ttu-id="9d442-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9d442-137">displayName</span></span>|<span data-ttu-id="9d442-138">Строка</span><span class="sxs-lookup"><span data-stu-id="9d442-138">String</span></span>|<span data-ttu-id="9d442-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9d442-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9d442-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-141">description</span><span class="sxs-lookup"><span data-stu-id="9d442-141">description</span></span>|<span data-ttu-id="9d442-142">Строка</span><span class="sxs-lookup"><span data-stu-id="9d442-142">String</span></span>|<span data-ttu-id="9d442-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9d442-143">The description of the app.</span></span> <span data-ttu-id="9d442-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-145">publisher</span><span class="sxs-lookup"><span data-stu-id="9d442-145">publisher</span></span>|<span data-ttu-id="9d442-146">String</span><span class="sxs-lookup"><span data-stu-id="9d442-146">String</span></span>|<span data-ttu-id="9d442-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9d442-147">The publisher of the app.</span></span> <span data-ttu-id="9d442-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9d442-149">largeIcon</span></span>|[<span data-ttu-id="9d442-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9d442-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9d442-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9d442-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9d442-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d442-153">createdDateTime</span></span>|<span data-ttu-id="9d442-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d442-154">DateTimeOffset</span></span>|<span data-ttu-id="9d442-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9d442-155">The date and time the app was created.</span></span> <span data-ttu-id="9d442-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d442-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9d442-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d442-158">DateTimeOffset</span></span>|<span data-ttu-id="9d442-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9d442-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9d442-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9d442-161">isFeatured</span></span>|<span data-ttu-id="9d442-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d442-162">Boolean</span></span>|<span data-ttu-id="9d442-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9d442-164">privacyInformationUrl</span></span>|<span data-ttu-id="9d442-165">String</span><span class="sxs-lookup"><span data-stu-id="9d442-165">String</span></span>|<span data-ttu-id="9d442-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9d442-166">The privacy statement Url.</span></span> <span data-ttu-id="9d442-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9d442-168">informationUrl</span></span>|<span data-ttu-id="9d442-169">String</span><span class="sxs-lookup"><span data-stu-id="9d442-169">String</span></span>|<span data-ttu-id="9d442-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9d442-170">The more information Url.</span></span> <span data-ttu-id="9d442-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-172">owner</span><span class="sxs-lookup"><span data-stu-id="9d442-172">owner</span></span>|<span data-ttu-id="9d442-173">String</span><span class="sxs-lookup"><span data-stu-id="9d442-173">String</span></span>|<span data-ttu-id="9d442-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9d442-174">The owner of the app.</span></span> <span data-ttu-id="9d442-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-176">developer</span><span class="sxs-lookup"><span data-stu-id="9d442-176">developer</span></span>|<span data-ttu-id="9d442-177">String</span><span class="sxs-lookup"><span data-stu-id="9d442-177">String</span></span>|<span data-ttu-id="9d442-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9d442-178">The developer of the app.</span></span> <span data-ttu-id="9d442-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-180">notes</span><span class="sxs-lookup"><span data-stu-id="9d442-180">notes</span></span>|<span data-ttu-id="9d442-181">String</span><span class="sxs-lookup"><span data-stu-id="9d442-181">String</span></span>|<span data-ttu-id="9d442-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9d442-182">Notes for the app.</span></span> <span data-ttu-id="9d442-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9d442-184">uploadState</span></span>|<span data-ttu-id="9d442-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9d442-185">Int32</span></span>|<span data-ttu-id="9d442-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="9d442-186">The upload state.</span></span> <span data-ttu-id="9d442-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="9d442-188">publishingState</span></span>|[<span data-ttu-id="9d442-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9d442-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9d442-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="9d442-190">The publishing state for the app.</span></span> <span data-ttu-id="9d442-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9d442-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9d442-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="9d442-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9d442-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9d442-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9d442-194">isAssigned</span></span>|<span data-ttu-id="9d442-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d442-195">Boolean</span></span>|<span data-ttu-id="9d442-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="9d442-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9d442-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9d442-198">roleScopeTagIds</span></span>|<span data-ttu-id="9d442-199">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="9d442-199">String collection</span></span>|<span data-ttu-id="9d442-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9d442-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9d442-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9d442-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="9d442-202">dependentAppCount</span></span>|<span data-ttu-id="9d442-203">Int32</span><span class="sxs-lookup"><span data-stu-id="9d442-203">Int32</span></span>|<span data-ttu-id="9d442-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="9d442-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9d442-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d442-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9d442-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d442-206">Response</span></span>
<span data-ttu-id="9d442-207">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосмдатпапп](../resources/intune-apps-macosmdatpapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d442-207">If successful, this method returns a `201 Created` response code and a [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d442-208">Пример</span><span class="sxs-lookup"><span data-stu-id="9d442-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d442-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d442-209">Request</span></span>
<span data-ttu-id="9d442-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d442-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9d442-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d442-211">Response</span></span>
<span data-ttu-id="9d442-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d442-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



