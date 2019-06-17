---
title: Создание объекта macOSOfficeSuiteApp
description: Создание объекта macOSOfficeSuiteApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4b84586a79a41adb6a4a9910b66e7e6c2467241
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975282"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="4451f-103">Создание объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="4451f-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="4451f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4451f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4451f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4451f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4451f-106">Создание объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-106">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4451f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4451f-107">Prerequisites</span></span>
<span data-ttu-id="4451f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4451f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4451f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4451f-110">Permission type</span></span>|<span data-ttu-id="4451f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4451f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4451f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4451f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4451f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4451f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4451f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4451f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4451f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4451f-115">Not supported.</span></span>|
|<span data-ttu-id="4451f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4451f-116">Application</span></span>|<span data-ttu-id="4451f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4451f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4451f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4451f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4451f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4451f-119">Request headers</span></span>
|<span data-ttu-id="4451f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4451f-120">Header</span></span>|<span data-ttu-id="4451f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4451f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4451f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4451f-122">Authorization</span></span>|<span data-ttu-id="4451f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4451f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4451f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4451f-124">Accept</span></span>|<span data-ttu-id="4451f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4451f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4451f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4451f-126">Request body</span></span>
<span data-ttu-id="4451f-127">В тексте запроса добавьте представление объекта macOSOfficeSuiteApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4451f-127">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="4451f-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="4451f-128">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="4451f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4451f-129">Property</span></span>|<span data-ttu-id="4451f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4451f-130">Type</span></span>|<span data-ttu-id="4451f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4451f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4451f-132">id</span><span class="sxs-lookup"><span data-stu-id="4451f-132">id</span></span>|<span data-ttu-id="4451f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4451f-133">String</span></span>|<span data-ttu-id="4451f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4451f-134">Key of the entity.</span></span> <span data-ttu-id="4451f-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4451f-136">displayName</span></span>|<span data-ttu-id="4451f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4451f-137">String</span></span>|<span data-ttu-id="4451f-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="4451f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4451f-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-140">description</span><span class="sxs-lookup"><span data-stu-id="4451f-140">description</span></span>|<span data-ttu-id="4451f-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4451f-141">String</span></span>|<span data-ttu-id="4451f-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="4451f-142">The description of the app.</span></span> <span data-ttu-id="4451f-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4451f-144">publisher</span></span>|<span data-ttu-id="4451f-145">String</span><span class="sxs-lookup"><span data-stu-id="4451f-145">String</span></span>|<span data-ttu-id="4451f-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="4451f-146">The publisher of the app.</span></span> <span data-ttu-id="4451f-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4451f-148">largeIcon</span></span>|[<span data-ttu-id="4451f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4451f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4451f-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="4451f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4451f-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4451f-152">createdDateTime</span></span>|<span data-ttu-id="4451f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4451f-153">DateTimeOffset</span></span>|<span data-ttu-id="4451f-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="4451f-154">The date and time the app was created.</span></span> <span data-ttu-id="4451f-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4451f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4451f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4451f-157">DateTimeOffset</span></span>|<span data-ttu-id="4451f-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="4451f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4451f-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4451f-160">isFeatured</span></span>|<span data-ttu-id="4451f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4451f-161">Boolean</span></span>|<span data-ttu-id="4451f-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4451f-163">privacyInformationUrl</span></span>|<span data-ttu-id="4451f-164">String</span><span class="sxs-lookup"><span data-stu-id="4451f-164">String</span></span>|<span data-ttu-id="4451f-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4451f-165">The privacy statement Url.</span></span> <span data-ttu-id="4451f-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4451f-167">informationUrl</span></span>|<span data-ttu-id="4451f-168">String</span><span class="sxs-lookup"><span data-stu-id="4451f-168">String</span></span>|<span data-ttu-id="4451f-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="4451f-169">The more information Url.</span></span> <span data-ttu-id="4451f-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-171">owner</span><span class="sxs-lookup"><span data-stu-id="4451f-171">owner</span></span>|<span data-ttu-id="4451f-172">String</span><span class="sxs-lookup"><span data-stu-id="4451f-172">String</span></span>|<span data-ttu-id="4451f-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="4451f-173">The owner of the app.</span></span> <span data-ttu-id="4451f-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-175">developer</span><span class="sxs-lookup"><span data-stu-id="4451f-175">developer</span></span>|<span data-ttu-id="4451f-176">String</span><span class="sxs-lookup"><span data-stu-id="4451f-176">String</span></span>|<span data-ttu-id="4451f-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="4451f-177">The developer of the app.</span></span> <span data-ttu-id="4451f-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-179">notes</span><span class="sxs-lookup"><span data-stu-id="4451f-179">notes</span></span>|<span data-ttu-id="4451f-180">String</span><span class="sxs-lookup"><span data-stu-id="4451f-180">String</span></span>|<span data-ttu-id="4451f-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="4451f-181">Notes for the app.</span></span> <span data-ttu-id="4451f-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4451f-183">uploadState</span></span>|<span data-ttu-id="4451f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4451f-184">Int32</span></span>|<span data-ttu-id="4451f-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="4451f-185">The upload state.</span></span> <span data-ttu-id="4451f-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4451f-187">publishingState</span></span>|[<span data-ttu-id="4451f-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="4451f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4451f-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="4451f-189">The publishing state for the app.</span></span> <span data-ttu-id="4451f-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="4451f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4451f-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4451f-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4451f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4451f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4451f-193">isAssigned</span></span>|<span data-ttu-id="4451f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4451f-194">Boolean</span></span>|<span data-ttu-id="4451f-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="4451f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4451f-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4451f-197">roleScopeTagIds</span></span>|<span data-ttu-id="4451f-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4451f-198">String collection</span></span>|<span data-ttu-id="4451f-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="4451f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4451f-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4451f-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="4451f-201">dependentAppCount</span></span>|<span data-ttu-id="4451f-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4451f-202">Int32</span></span>|<span data-ttu-id="4451f-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="4451f-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4451f-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4451f-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4451f-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="4451f-205">Response</span></span>
<span data-ttu-id="4451f-206">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4451f-206">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4451f-207">Пример</span><span class="sxs-lookup"><span data-stu-id="4451f-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="4451f-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="4451f-208">Request</span></span>
<span data-ttu-id="4451f-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4451f-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="4451f-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="4451f-210">Response</span></span>
<span data-ttu-id="4451f-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4451f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





