---
title: Обновление Виндовсстореапп
description: Обновление свойств объекта Виндовсстореапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9bf99d5c84fcf942fd978d105e1b6e95bc608ff
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972755"
---
# <a name="update-windowsstoreapp"></a><span data-ttu-id="4feef-103">Обновление Виндовсстореапп</span><span class="sxs-lookup"><span data-stu-id="4feef-103">Update windowsStoreApp</span></span>

> <span data-ttu-id="4feef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4feef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4feef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4feef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4feef-106">Обновление свойств объекта [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="4feef-106">Update the properties of a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4feef-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4feef-107">Prerequisites</span></span>
<span data-ttu-id="4feef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4feef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4feef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4feef-110">Permission type</span></span>|<span data-ttu-id="4feef-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4feef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4feef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4feef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4feef-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4feef-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4feef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4feef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4feef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4feef-115">Not supported.</span></span>|
|<span data-ttu-id="4feef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4feef-116">Application</span></span>|<span data-ttu-id="4feef-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4feef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4feef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4feef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4feef-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4feef-119">Request headers</span></span>
|<span data-ttu-id="4feef-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4feef-120">Header</span></span>|<span data-ttu-id="4feef-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4feef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4feef-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4feef-122">Authorization</span></span>|<span data-ttu-id="4feef-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4feef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4feef-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4feef-124">Accept</span></span>|<span data-ttu-id="4feef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4feef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4feef-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4feef-126">Request body</span></span>
<span data-ttu-id="4feef-127">В тексте запроса добавьте представление объекта [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4feef-127">In the request body, supply a JSON representation for the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

<span data-ttu-id="4feef-128">В следующей таблице приведены свойства, необходимые при создании [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-128">The following table shows the properties that are required when you create the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span></span>

|<span data-ttu-id="4feef-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4feef-129">Property</span></span>|<span data-ttu-id="4feef-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4feef-130">Type</span></span>|<span data-ttu-id="4feef-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4feef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4feef-132">id</span><span class="sxs-lookup"><span data-stu-id="4feef-132">id</span></span>|<span data-ttu-id="4feef-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4feef-133">String</span></span>|<span data-ttu-id="4feef-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4feef-134">Key of the entity.</span></span> <span data-ttu-id="4feef-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4feef-136">displayName</span></span>|<span data-ttu-id="4feef-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4feef-137">String</span></span>|<span data-ttu-id="4feef-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="4feef-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4feef-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-140">description</span><span class="sxs-lookup"><span data-stu-id="4feef-140">description</span></span>|<span data-ttu-id="4feef-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4feef-141">String</span></span>|<span data-ttu-id="4feef-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="4feef-142">The description of the app.</span></span> <span data-ttu-id="4feef-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4feef-144">publisher</span></span>|<span data-ttu-id="4feef-145">String</span><span class="sxs-lookup"><span data-stu-id="4feef-145">String</span></span>|<span data-ttu-id="4feef-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="4feef-146">The publisher of the app.</span></span> <span data-ttu-id="4feef-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4feef-148">largeIcon</span></span>|[<span data-ttu-id="4feef-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4feef-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4feef-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="4feef-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4feef-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4feef-152">createdDateTime</span></span>|<span data-ttu-id="4feef-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4feef-153">DateTimeOffset</span></span>|<span data-ttu-id="4feef-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="4feef-154">The date and time the app was created.</span></span> <span data-ttu-id="4feef-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4feef-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4feef-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4feef-157">DateTimeOffset</span></span>|<span data-ttu-id="4feef-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="4feef-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4feef-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4feef-160">isFeatured</span></span>|<span data-ttu-id="4feef-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4feef-161">Boolean</span></span>|<span data-ttu-id="4feef-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4feef-163">privacyInformationUrl</span></span>|<span data-ttu-id="4feef-164">String</span><span class="sxs-lookup"><span data-stu-id="4feef-164">String</span></span>|<span data-ttu-id="4feef-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4feef-165">The privacy statement Url.</span></span> <span data-ttu-id="4feef-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4feef-167">informationUrl</span></span>|<span data-ttu-id="4feef-168">String</span><span class="sxs-lookup"><span data-stu-id="4feef-168">String</span></span>|<span data-ttu-id="4feef-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="4feef-169">The more information Url.</span></span> <span data-ttu-id="4feef-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-171">owner</span><span class="sxs-lookup"><span data-stu-id="4feef-171">owner</span></span>|<span data-ttu-id="4feef-172">String</span><span class="sxs-lookup"><span data-stu-id="4feef-172">String</span></span>|<span data-ttu-id="4feef-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="4feef-173">The owner of the app.</span></span> <span data-ttu-id="4feef-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-175">developer</span><span class="sxs-lookup"><span data-stu-id="4feef-175">developer</span></span>|<span data-ttu-id="4feef-176">String</span><span class="sxs-lookup"><span data-stu-id="4feef-176">String</span></span>|<span data-ttu-id="4feef-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="4feef-177">The developer of the app.</span></span> <span data-ttu-id="4feef-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-179">notes</span><span class="sxs-lookup"><span data-stu-id="4feef-179">notes</span></span>|<span data-ttu-id="4feef-180">String</span><span class="sxs-lookup"><span data-stu-id="4feef-180">String</span></span>|<span data-ttu-id="4feef-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="4feef-181">Notes for the app.</span></span> <span data-ttu-id="4feef-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4feef-183">uploadState</span></span>|<span data-ttu-id="4feef-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4feef-184">Int32</span></span>|<span data-ttu-id="4feef-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="4feef-185">The upload state.</span></span> <span data-ttu-id="4feef-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4feef-187">publishingState</span></span>|[<span data-ttu-id="4feef-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="4feef-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4feef-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="4feef-189">The publishing state for the app.</span></span> <span data-ttu-id="4feef-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="4feef-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4feef-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4feef-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4feef-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4feef-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4feef-193">isAssigned</span></span>|<span data-ttu-id="4feef-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4feef-194">Boolean</span></span>|<span data-ttu-id="4feef-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="4feef-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4feef-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4feef-197">roleScopeTagIds</span></span>|<span data-ttu-id="4feef-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4feef-198">String collection</span></span>|<span data-ttu-id="4feef-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="4feef-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4feef-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="4feef-201">dependentAppCount</span></span>|<span data-ttu-id="4feef-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4feef-202">Int32</span></span>|<span data-ttu-id="4feef-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="4feef-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4feef-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4feef-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4feef-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4feef-205">appStoreUrl</span></span>|<span data-ttu-id="4feef-206">String</span><span class="sxs-lookup"><span data-stu-id="4feef-206">String</span></span>|<span data-ttu-id="4feef-207">URL-адрес хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="4feef-207">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="4feef-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="4feef-208">Response</span></span>
<span data-ttu-id="4feef-209">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4feef-209">If successful, this method returns a `200 OK` response code and an updated [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4feef-210">Пример</span><span class="sxs-lookup"><span data-stu-id="4feef-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="4feef-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="4feef-211">Request</span></span>
<span data-ttu-id="4feef-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4feef-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="4feef-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="4feef-213">Response</span></span>
<span data-ttu-id="4feef-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4feef-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





