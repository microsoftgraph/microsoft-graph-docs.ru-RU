---
title: Обновление Виндовсстореапп
description: Обновление свойств объекта Виндовсстореапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 101c89634f75dd8d81b85dbfb8ba7bd879674c6c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43393394"
---
# <a name="update-windowsstoreapp"></a><span data-ttu-id="b3924-103">Обновление Виндовсстореапп</span><span class="sxs-lookup"><span data-stu-id="b3924-103">Update windowsStoreApp</span></span>

<span data-ttu-id="b3924-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3924-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3924-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3924-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3924-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3924-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3924-107">Обновление свойств объекта [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b3924-107">Update the properties of a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3924-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b3924-108">Prerequisites</span></span>
<span data-ttu-id="b3924-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3924-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3924-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3924-111">Permission type</span></span>|<span data-ttu-id="b3924-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3924-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3924-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3924-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3924-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3924-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b3924-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3924-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3924-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3924-116">Not supported.</span></span>|
|<span data-ttu-id="b3924-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="b3924-117">Application</span></span>|<span data-ttu-id="b3924-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3924-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3924-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3924-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b3924-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b3924-120">Request headers</span></span>
|<span data-ttu-id="b3924-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3924-121">Header</span></span>|<span data-ttu-id="b3924-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b3924-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3924-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3924-123">Authorization</span></span>|<span data-ttu-id="b3924-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3924-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3924-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3924-125">Accept</span></span>|<span data-ttu-id="b3924-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3924-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3924-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3924-127">Request body</span></span>
<span data-ttu-id="b3924-128">В тексте запроса добавьте представление объекта [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3924-128">In the request body, supply a JSON representation for the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

<span data-ttu-id="b3924-129">В следующей таблице приведены свойства, необходимые при создании [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-129">The following table shows the properties that are required when you create the [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md).</span></span>

|<span data-ttu-id="b3924-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3924-130">Property</span></span>|<span data-ttu-id="b3924-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b3924-131">Type</span></span>|<span data-ttu-id="b3924-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b3924-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3924-133">id</span><span class="sxs-lookup"><span data-stu-id="b3924-133">id</span></span>|<span data-ttu-id="b3924-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b3924-134">String</span></span>|<span data-ttu-id="b3924-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b3924-135">Key of the entity.</span></span> <span data-ttu-id="b3924-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b3924-137">displayName</span></span>|<span data-ttu-id="b3924-138">Строка</span><span class="sxs-lookup"><span data-stu-id="b3924-138">String</span></span>|<span data-ttu-id="b3924-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b3924-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b3924-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-141">description</span><span class="sxs-lookup"><span data-stu-id="b3924-141">description</span></span>|<span data-ttu-id="b3924-142">Строка</span><span class="sxs-lookup"><span data-stu-id="b3924-142">String</span></span>|<span data-ttu-id="b3924-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b3924-143">The description of the app.</span></span> <span data-ttu-id="b3924-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-145">publisher</span><span class="sxs-lookup"><span data-stu-id="b3924-145">publisher</span></span>|<span data-ttu-id="b3924-146">String</span><span class="sxs-lookup"><span data-stu-id="b3924-146">String</span></span>|<span data-ttu-id="b3924-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b3924-147">The publisher of the app.</span></span> <span data-ttu-id="b3924-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b3924-149">largeIcon</span></span>|[<span data-ttu-id="b3924-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b3924-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b3924-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b3924-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b3924-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3924-153">createdDateTime</span></span>|<span data-ttu-id="b3924-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3924-154">DateTimeOffset</span></span>|<span data-ttu-id="b3924-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b3924-155">The date and time the app was created.</span></span> <span data-ttu-id="b3924-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3924-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b3924-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3924-158">DateTimeOffset</span></span>|<span data-ttu-id="b3924-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b3924-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b3924-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b3924-161">isFeatured</span></span>|<span data-ttu-id="b3924-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3924-162">Boolean</span></span>|<span data-ttu-id="b3924-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b3924-164">privacyInformationUrl</span></span>|<span data-ttu-id="b3924-165">String</span><span class="sxs-lookup"><span data-stu-id="b3924-165">String</span></span>|<span data-ttu-id="b3924-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b3924-166">The privacy statement Url.</span></span> <span data-ttu-id="b3924-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b3924-168">informationUrl</span></span>|<span data-ttu-id="b3924-169">String</span><span class="sxs-lookup"><span data-stu-id="b3924-169">String</span></span>|<span data-ttu-id="b3924-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b3924-170">The more information Url.</span></span> <span data-ttu-id="b3924-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-172">owner</span><span class="sxs-lookup"><span data-stu-id="b3924-172">owner</span></span>|<span data-ttu-id="b3924-173">String</span><span class="sxs-lookup"><span data-stu-id="b3924-173">String</span></span>|<span data-ttu-id="b3924-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b3924-174">The owner of the app.</span></span> <span data-ttu-id="b3924-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-176">developer</span><span class="sxs-lookup"><span data-stu-id="b3924-176">developer</span></span>|<span data-ttu-id="b3924-177">String</span><span class="sxs-lookup"><span data-stu-id="b3924-177">String</span></span>|<span data-ttu-id="b3924-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b3924-178">The developer of the app.</span></span> <span data-ttu-id="b3924-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-180">notes</span><span class="sxs-lookup"><span data-stu-id="b3924-180">notes</span></span>|<span data-ttu-id="b3924-181">String</span><span class="sxs-lookup"><span data-stu-id="b3924-181">String</span></span>|<span data-ttu-id="b3924-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="b3924-182">Notes for the app.</span></span> <span data-ttu-id="b3924-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b3924-184">uploadState</span></span>|<span data-ttu-id="b3924-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b3924-185">Int32</span></span>|<span data-ttu-id="b3924-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="b3924-186">The upload state.</span></span> <span data-ttu-id="b3924-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="b3924-188">publishingState</span></span>|[<span data-ttu-id="b3924-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="b3924-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b3924-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="b3924-190">The publishing state for the app.</span></span> <span data-ttu-id="b3924-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b3924-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b3924-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="b3924-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b3924-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b3924-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b3924-194">isAssigned</span></span>|<span data-ttu-id="b3924-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3924-195">Boolean</span></span>|<span data-ttu-id="b3924-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="b3924-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b3924-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3924-198">roleScopeTagIds</span></span>|<span data-ttu-id="b3924-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b3924-199">String collection</span></span>|<span data-ttu-id="b3924-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b3924-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b3924-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="b3924-202">dependentAppCount</span></span>|<span data-ttu-id="b3924-203">Int32</span><span class="sxs-lookup"><span data-stu-id="b3924-203">Int32</span></span>|<span data-ttu-id="b3924-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="b3924-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b3924-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b3924-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b3924-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b3924-206">appStoreUrl</span></span>|<span data-ttu-id="b3924-207">String</span><span class="sxs-lookup"><span data-stu-id="b3924-207">String</span></span>|<span data-ttu-id="b3924-208">URL-адрес хранилища приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="b3924-208">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="b3924-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3924-209">Response</span></span>
<span data-ttu-id="b3924-210">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсстореапп](../resources/intune-apps-windowsstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3924-210">If successful, this method returns a `200 OK` response code and an updated [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3924-211">Пример</span><span class="sxs-lookup"><span data-stu-id="b3924-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3924-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3924-212">Request</span></span>
<span data-ttu-id="b3924-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3924-213">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b3924-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3924-214">Response</span></span>
<span data-ttu-id="b3924-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3924-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



