---
title: Обновление объекта macOSOfficeSuiteApp
description: Обновление свойств объекта macOSOfficeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0cc1378dc39903599387f67a206c90ac478d5531
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780772"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="d80fb-103">Обновление объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="d80fb-103">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="d80fb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d80fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d80fb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d80fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d80fb-106">Обновление свойств объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-106">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d80fb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d80fb-107">Prerequisites</span></span>
<span data-ttu-id="d80fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d80fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d80fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d80fb-110">Permission type</span></span>|<span data-ttu-id="d80fb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d80fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d80fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d80fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d80fb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d80fb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d80fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d80fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d80fb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d80fb-115">Not supported.</span></span>|
|<span data-ttu-id="d80fb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d80fb-116">Application</span></span>|<span data-ttu-id="d80fb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d80fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d80fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d80fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="d80fb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d80fb-119">Request headers</span></span>
|<span data-ttu-id="d80fb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d80fb-120">Header</span></span>|<span data-ttu-id="d80fb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d80fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d80fb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d80fb-122">Authorization</span></span>|<span data-ttu-id="d80fb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d80fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d80fb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d80fb-124">Accept</span></span>|<span data-ttu-id="d80fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d80fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d80fb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d80fb-126">Request body</span></span>
<span data-ttu-id="d80fb-127">В тексте запроса добавьте представление объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d80fb-127">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="d80fb-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-128">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="d80fb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d80fb-129">Property</span></span>|<span data-ttu-id="d80fb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d80fb-130">Type</span></span>|<span data-ttu-id="d80fb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d80fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d80fb-132">id</span><span class="sxs-lookup"><span data-stu-id="d80fb-132">id</span></span>|<span data-ttu-id="d80fb-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d80fb-133">String</span></span>|<span data-ttu-id="d80fb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d80fb-134">Key of the entity.</span></span> <span data-ttu-id="d80fb-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d80fb-136">displayName</span></span>|<span data-ttu-id="d80fb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d80fb-137">String</span></span>|<span data-ttu-id="d80fb-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d80fb-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d80fb-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-140">description</span><span class="sxs-lookup"><span data-stu-id="d80fb-140">description</span></span>|<span data-ttu-id="d80fb-141">String</span><span class="sxs-lookup"><span data-stu-id="d80fb-141">String</span></span>|<span data-ttu-id="d80fb-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d80fb-142">The description of the app.</span></span> <span data-ttu-id="d80fb-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-144">publisher</span><span class="sxs-lookup"><span data-stu-id="d80fb-144">publisher</span></span>|<span data-ttu-id="d80fb-145">String</span><span class="sxs-lookup"><span data-stu-id="d80fb-145">String</span></span>|<span data-ttu-id="d80fb-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d80fb-146">The publisher of the app.</span></span> <span data-ttu-id="d80fb-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d80fb-148">largeIcon</span></span>|[<span data-ttu-id="d80fb-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d80fb-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d80fb-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d80fb-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d80fb-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d80fb-152">createdDateTime</span></span>|<span data-ttu-id="d80fb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d80fb-153">DateTimeOffset</span></span>|<span data-ttu-id="d80fb-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d80fb-154">The date and time the app was created.</span></span> <span data-ttu-id="d80fb-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d80fb-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d80fb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d80fb-157">DateTimeOffset</span></span>|<span data-ttu-id="d80fb-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d80fb-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d80fb-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d80fb-160">isFeatured</span></span>|<span data-ttu-id="d80fb-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80fb-161">Boolean</span></span>|<span data-ttu-id="d80fb-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d80fb-163">privacyInformationUrl</span></span>|<span data-ttu-id="d80fb-164">String</span><span class="sxs-lookup"><span data-stu-id="d80fb-164">String</span></span>|<span data-ttu-id="d80fb-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d80fb-165">The privacy statement Url.</span></span> <span data-ttu-id="d80fb-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d80fb-167">informationUrl</span></span>|<span data-ttu-id="d80fb-168">String</span><span class="sxs-lookup"><span data-stu-id="d80fb-168">String</span></span>|<span data-ttu-id="d80fb-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d80fb-169">The more information Url.</span></span> <span data-ttu-id="d80fb-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-171">owner</span><span class="sxs-lookup"><span data-stu-id="d80fb-171">owner</span></span>|<span data-ttu-id="d80fb-172">String</span><span class="sxs-lookup"><span data-stu-id="d80fb-172">String</span></span>|<span data-ttu-id="d80fb-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d80fb-173">The owner of the app.</span></span> <span data-ttu-id="d80fb-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-175">developer</span><span class="sxs-lookup"><span data-stu-id="d80fb-175">developer</span></span>|<span data-ttu-id="d80fb-176">String</span><span class="sxs-lookup"><span data-stu-id="d80fb-176">String</span></span>|<span data-ttu-id="d80fb-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d80fb-177">The developer of the app.</span></span> <span data-ttu-id="d80fb-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-179">notes</span><span class="sxs-lookup"><span data-stu-id="d80fb-179">notes</span></span>|<span data-ttu-id="d80fb-180">String</span><span class="sxs-lookup"><span data-stu-id="d80fb-180">String</span></span>|<span data-ttu-id="d80fb-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="d80fb-181">Notes for the app.</span></span> <span data-ttu-id="d80fb-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="d80fb-183">uploadState</span></span>|<span data-ttu-id="d80fb-184">Int32</span><span class="sxs-lookup"><span data-stu-id="d80fb-184">Int32</span></span>|<span data-ttu-id="d80fb-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="d80fb-185">The upload state.</span></span> <span data-ttu-id="d80fb-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="d80fb-187">publishingState</span></span>|[<span data-ttu-id="d80fb-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="d80fb-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d80fb-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="d80fb-189">The publishing state for the app.</span></span> <span data-ttu-id="d80fb-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d80fb-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d80fb-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d80fb-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d80fb-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d80fb-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d80fb-193">isAssigned</span></span>|<span data-ttu-id="d80fb-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d80fb-194">Boolean</span></span>|<span data-ttu-id="d80fb-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="d80fb-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d80fb-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d80fb-197">roleScopeTagIds</span></span>|<span data-ttu-id="d80fb-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d80fb-198">String collection</span></span>|<span data-ttu-id="d80fb-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d80fb-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d80fb-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d80fb-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="d80fb-201">dependentAppCount</span></span>|<span data-ttu-id="d80fb-202">Int32</span><span class="sxs-lookup"><span data-stu-id="d80fb-202">Int32</span></span>|<span data-ttu-id="d80fb-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="d80fb-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d80fb-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d80fb-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="d80fb-205">Response</span></span>
<span data-ttu-id="d80fb-206">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d80fb-206">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d80fb-207">Пример</span><span class="sxs-lookup"><span data-stu-id="d80fb-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="d80fb-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="d80fb-208">Request</span></span>
<span data-ttu-id="d80fb-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d80fb-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="d80fb-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="d80fb-210">Response</span></span>
<span data-ttu-id="d80fb-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d80fb-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





