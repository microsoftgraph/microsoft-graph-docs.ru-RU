---
title: Обновление win32LobApp
description: Обновление свойств объекта win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7a07b2264d4c3d6cf6e180e210d4937a5422b46
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247274"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="8dbae-103">Обновление win32LobApp</span><span class="sxs-lookup"><span data-stu-id="8dbae-103">Update win32LobApp</span></span>

<span data-ttu-id="8dbae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dbae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8dbae-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dbae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dbae-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8dbae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dbae-107">Обновление свойств объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8dbae-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8dbae-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8dbae-108">Prerequisites</span></span>
<span data-ttu-id="8dbae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dbae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dbae-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dbae-111">Permission type</span></span>|<span data-ttu-id="8dbae-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dbae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dbae-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dbae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8dbae-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dbae-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8dbae-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dbae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dbae-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dbae-116">Not supported.</span></span>|
|<span data-ttu-id="8dbae-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8dbae-117">Application</span></span>|<span data-ttu-id="8dbae-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dbae-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dbae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dbae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8dbae-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8dbae-120">Request headers</span></span>
|<span data-ttu-id="8dbae-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8dbae-121">Header</span></span>|<span data-ttu-id="8dbae-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8dbae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8dbae-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dbae-123">Authorization</span></span>|<span data-ttu-id="8dbae-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dbae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8dbae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8dbae-125">Accept</span></span>|<span data-ttu-id="8dbae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8dbae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dbae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dbae-127">Request body</span></span>
<span data-ttu-id="8dbae-128">В тексте запроса добавьте представление объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8dbae-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="8dbae-129">В следующей таблице приведены свойства, необходимые при создании [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="8dbae-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dbae-130">Property</span></span>|<span data-ttu-id="8dbae-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8dbae-131">Type</span></span>|<span data-ttu-id="8dbae-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8dbae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dbae-133">id</span><span class="sxs-lookup"><span data-stu-id="8dbae-133">id</span></span>|<span data-ttu-id="8dbae-134">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-134">String</span></span>|<span data-ttu-id="8dbae-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8dbae-135">Key of the entity.</span></span> <span data-ttu-id="8dbae-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8dbae-137">displayName</span></span>|<span data-ttu-id="8dbae-138">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-138">String</span></span>|<span data-ttu-id="8dbae-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="8dbae-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8dbae-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-141">description</span><span class="sxs-lookup"><span data-stu-id="8dbae-141">description</span></span>|<span data-ttu-id="8dbae-142">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-142">String</span></span>|<span data-ttu-id="8dbae-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-143">The description of the app.</span></span> <span data-ttu-id="8dbae-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8dbae-145">publisher</span></span>|<span data-ttu-id="8dbae-146">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-146">String</span></span>|<span data-ttu-id="8dbae-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-147">The publisher of the app.</span></span> <span data-ttu-id="8dbae-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8dbae-149">largeIcon</span></span>|[<span data-ttu-id="8dbae-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8dbae-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8dbae-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="8dbae-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8dbae-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8dbae-153">createdDateTime</span></span>|<span data-ttu-id="8dbae-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dbae-154">DateTimeOffset</span></span>|<span data-ttu-id="8dbae-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-155">The date and time the app was created.</span></span> <span data-ttu-id="8dbae-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8dbae-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8dbae-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dbae-158">DateTimeOffset</span></span>|<span data-ttu-id="8dbae-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8dbae-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8dbae-161">isFeatured</span></span>|<span data-ttu-id="8dbae-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dbae-162">Boolean</span></span>|<span data-ttu-id="8dbae-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8dbae-164">privacyInformationUrl</span></span>|<span data-ttu-id="8dbae-165">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-165">String</span></span>|<span data-ttu-id="8dbae-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8dbae-166">The privacy statement Url.</span></span> <span data-ttu-id="8dbae-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8dbae-168">informationUrl</span></span>|<span data-ttu-id="8dbae-169">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-169">String</span></span>|<span data-ttu-id="8dbae-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="8dbae-170">The more information Url.</span></span> <span data-ttu-id="8dbae-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-172">owner</span><span class="sxs-lookup"><span data-stu-id="8dbae-172">owner</span></span>|<span data-ttu-id="8dbae-173">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-173">String</span></span>|<span data-ttu-id="8dbae-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-174">The owner of the app.</span></span> <span data-ttu-id="8dbae-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-176">developer</span><span class="sxs-lookup"><span data-stu-id="8dbae-176">developer</span></span>|<span data-ttu-id="8dbae-177">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-177">String</span></span>|<span data-ttu-id="8dbae-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-178">The developer of the app.</span></span> <span data-ttu-id="8dbae-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-180">notes</span><span class="sxs-lookup"><span data-stu-id="8dbae-180">notes</span></span>|<span data-ttu-id="8dbae-181">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-181">String</span></span>|<span data-ttu-id="8dbae-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-182">Notes for the app.</span></span> <span data-ttu-id="8dbae-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8dbae-184">uploadState</span></span>|<span data-ttu-id="8dbae-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8dbae-185">Int32</span></span>|<span data-ttu-id="8dbae-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="8dbae-186">The upload state.</span></span> <span data-ttu-id="8dbae-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="8dbae-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="8dbae-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="8dbae-189">publishingState</span></span>|[<span data-ttu-id="8dbae-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="8dbae-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8dbae-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-191">The publishing state for the app.</span></span> <span data-ttu-id="8dbae-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="8dbae-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8dbae-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8dbae-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8dbae-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8dbae-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8dbae-195">isAssigned</span></span>|<span data-ttu-id="8dbae-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dbae-196">Boolean</span></span>|<span data-ttu-id="8dbae-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="8dbae-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8dbae-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8dbae-199">roleScopeTagIds</span></span>|<span data-ttu-id="8dbae-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8dbae-200">String collection</span></span>|<span data-ttu-id="8dbae-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8dbae-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="8dbae-203">dependentAppCount</span></span>|<span data-ttu-id="8dbae-204">Int32</span><span class="sxs-lookup"><span data-stu-id="8dbae-204">Int32</span></span>|<span data-ttu-id="8dbae-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8dbae-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="8dbae-207">supersedingAppCount</span></span>|<span data-ttu-id="8dbae-208">Int32</span><span class="sxs-lookup"><span data-stu-id="8dbae-208">Int32</span></span>|<span data-ttu-id="8dbae-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="8dbae-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="8dbae-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="8dbae-211">supersededAppCount</span></span>|<span data-ttu-id="8dbae-212">Int32</span><span class="sxs-lookup"><span data-stu-id="8dbae-212">Int32</span></span>|<span data-ttu-id="8dbae-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="8dbae-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="8dbae-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dbae-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8dbae-215">committedContentVersion</span></span>|<span data-ttu-id="8dbae-216">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-216">String</span></span>|<span data-ttu-id="8dbae-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="8dbae-217">The internal committed content version.</span></span> <span data-ttu-id="8dbae-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8dbae-219">fileName</span><span class="sxs-lookup"><span data-stu-id="8dbae-219">fileName</span></span>|<span data-ttu-id="8dbae-220">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-220">String</span></span>|<span data-ttu-id="8dbae-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-221">The name of the main Lob application file.</span></span> <span data-ttu-id="8dbae-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8dbae-223">size</span><span class="sxs-lookup"><span data-stu-id="8dbae-223">size</span></span>|<span data-ttu-id="8dbae-224">Int64</span><span class="sxs-lookup"><span data-stu-id="8dbae-224">Int64</span></span>|<span data-ttu-id="8dbae-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="8dbae-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="8dbae-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dbae-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8dbae-227">инсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="8dbae-227">installCommandLine</span></span>|<span data-ttu-id="8dbae-228">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-228">String</span></span>|<span data-ttu-id="8dbae-229">Командная строка для установки приложения</span><span class="sxs-lookup"><span data-stu-id="8dbae-229">The command line to install this app</span></span>|
|<span data-ttu-id="8dbae-230">унинсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="8dbae-230">uninstallCommandLine</span></span>|<span data-ttu-id="8dbae-231">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-231">String</span></span>|<span data-ttu-id="8dbae-232">Командная строка для удаления приложения</span><span class="sxs-lookup"><span data-stu-id="8dbae-232">The command line to uninstall this app</span></span>|
|<span data-ttu-id="8dbae-233">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="8dbae-233">applicableArchitectures</span></span>|[<span data-ttu-id="8dbae-234">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="8dbae-234">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="8dbae-235">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="8dbae-235">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="8dbae-236">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="8dbae-236">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="8dbae-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8dbae-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8dbae-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8dbae-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="8dbae-239">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="8dbae-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8dbae-240">минимумфридискспацеинмб</span><span class="sxs-lookup"><span data-stu-id="8dbae-240">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="8dbae-241">Int32</span><span class="sxs-lookup"><span data-stu-id="8dbae-241">Int32</span></span>|<span data-ttu-id="8dbae-242">Минимальное свободное место на диске, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-242">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="8dbae-243">минимуммеморинмб</span><span class="sxs-lookup"><span data-stu-id="8dbae-243">minimumMemoryInMB</span></span>|<span data-ttu-id="8dbae-244">Int32</span><span class="sxs-lookup"><span data-stu-id="8dbae-244">Int32</span></span>|<span data-ttu-id="8dbae-245">Значение минимальной физической памяти, необходимой для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-245">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="8dbae-246">минимумнумберофпроцессорс</span><span class="sxs-lookup"><span data-stu-id="8dbae-246">minimumNumberOfProcessors</span></span>|<span data-ttu-id="8dbae-247">Int32</span><span class="sxs-lookup"><span data-stu-id="8dbae-247">Int32</span></span>|<span data-ttu-id="8dbae-248">Значение минимального числа процессоров, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-248">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="8dbae-249">минимумкпуспидинмхз</span><span class="sxs-lookup"><span data-stu-id="8dbae-249">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="8dbae-250">Int32</span><span class="sxs-lookup"><span data-stu-id="8dbae-250">Int32</span></span>|<span data-ttu-id="8dbae-251">Значение минимальной скорости ЦП, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-251">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="8dbae-252">детектионрулес</span><span class="sxs-lookup"><span data-stu-id="8dbae-252">detectionRules</span></span>|<span data-ttu-id="8dbae-253">Коллекция [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="8dbae-253">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="8dbae-254">Правила обнаружения для определения бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="8dbae-254">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8dbae-255">рекуирементрулес</span><span class="sxs-lookup"><span data-stu-id="8dbae-255">requirementRules</span></span>|<span data-ttu-id="8dbae-256">Коллекция [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="8dbae-256">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="8dbae-257">Правила требований для обнаружения бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="8dbae-257">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8dbae-258">правила</span><span class="sxs-lookup"><span data-stu-id="8dbae-258">rules</span></span>|<span data-ttu-id="8dbae-259">Коллекция [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="8dbae-259">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="8dbae-260">Правила обнаружения и требований для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-260">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="8dbae-261">инсталлекспериенце</span><span class="sxs-lookup"><span data-stu-id="8dbae-261">installExperience</span></span>|[<span data-ttu-id="8dbae-262">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="8dbae-262">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="8dbae-263">Установка приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-263">The install experience for this app.</span></span>|
|<span data-ttu-id="8dbae-264">ретурнкодес</span><span class="sxs-lookup"><span data-stu-id="8dbae-264">returnCodes</span></span>|<span data-ttu-id="8dbae-265">Коллекция [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="8dbae-265">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="8dbae-266">Коды возврата для поведения после установки.</span><span class="sxs-lookup"><span data-stu-id="8dbae-266">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="8dbae-267">мсиинформатион</span><span class="sxs-lookup"><span data-stu-id="8dbae-267">msiInformation</span></span>|[<span data-ttu-id="8dbae-268">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="8dbae-268">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="8dbae-269">Сведения о MSI, если это приложение Win32 является приложением MSI.</span><span class="sxs-lookup"><span data-stu-id="8dbae-269">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="8dbae-270">сетупфилепас</span><span class="sxs-lookup"><span data-stu-id="8dbae-270">setupFilePath</span></span>|<span data-ttu-id="8dbae-271">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-271">String</span></span>|<span data-ttu-id="8dbae-272">Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="8dbae-272">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="8dbae-273">минимумсуппортедвиндовсрелеасе</span><span class="sxs-lookup"><span data-stu-id="8dbae-273">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="8dbae-274">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-274">String</span></span>|<span data-ttu-id="8dbae-275">Значение минимального поддерживаемого выпуска Windows.</span><span class="sxs-lookup"><span data-stu-id="8dbae-275">The value for the minimum supported windows release.</span></span>|
|<span data-ttu-id="8dbae-276">дисплайверсион</span><span class="sxs-lookup"><span data-stu-id="8dbae-276">displayVersion</span></span>|<span data-ttu-id="8dbae-277">String</span><span class="sxs-lookup"><span data-stu-id="8dbae-277">String</span></span>|<span data-ttu-id="8dbae-278">Версия, отображаемая в UX для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="8dbae-278">The version displayed in the UX for this app.</span></span>|



## <a name="response"></a><span data-ttu-id="8dbae-279">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dbae-279">Response</span></span>
<span data-ttu-id="8dbae-280">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8dbae-280">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dbae-281">Пример</span><span class="sxs-lookup"><span data-stu-id="8dbae-281">Example</span></span>

### <a name="request"></a><span data-ttu-id="8dbae-282">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dbae-282">Request</span></span>
<span data-ttu-id="8dbae-283">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dbae-283">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 3359

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="8dbae-284">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dbae-284">Response</span></span>
<span data-ttu-id="8dbae-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8dbae-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3531

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value",
  "displayVersion": "Display Version value"
}
```




