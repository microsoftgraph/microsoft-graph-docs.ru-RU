---
title: Обновление win32LobApp
description: Обновление свойств объекта win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0ec59ffe1ef88ebb508d8ba4b614906948d892a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694769"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="924f0-103">Обновление win32LobApp</span><span class="sxs-lookup"><span data-stu-id="924f0-103">Update win32LobApp</span></span>

<span data-ttu-id="924f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="924f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="924f0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="924f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="924f0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="924f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="924f0-107">Обновление свойств объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="924f0-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="924f0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="924f0-108">Prerequisites</span></span>
<span data-ttu-id="924f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="924f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="924f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="924f0-111">Permission type</span></span>|<span data-ttu-id="924f0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="924f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="924f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="924f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="924f0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="924f0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="924f0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="924f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="924f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="924f0-116">Not supported.</span></span>|
|<span data-ttu-id="924f0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="924f0-117">Application</span></span>|<span data-ttu-id="924f0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="924f0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="924f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="924f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="924f0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="924f0-120">Request headers</span></span>
|<span data-ttu-id="924f0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="924f0-121">Header</span></span>|<span data-ttu-id="924f0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="924f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="924f0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="924f0-123">Authorization</span></span>|<span data-ttu-id="924f0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="924f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="924f0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="924f0-125">Accept</span></span>|<span data-ttu-id="924f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="924f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="924f0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="924f0-127">Request body</span></span>
<span data-ttu-id="924f0-128">В тексте запроса добавьте представление объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="924f0-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="924f0-129">В следующей таблице приведены свойства, необходимые при создании [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="924f0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="924f0-130">Property</span></span>|<span data-ttu-id="924f0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="924f0-131">Type</span></span>|<span data-ttu-id="924f0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="924f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="924f0-133">id</span><span class="sxs-lookup"><span data-stu-id="924f0-133">id</span></span>|<span data-ttu-id="924f0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="924f0-134">String</span></span>|<span data-ttu-id="924f0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="924f0-135">Key of the entity.</span></span> <span data-ttu-id="924f0-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="924f0-137">displayName</span></span>|<span data-ttu-id="924f0-138">Строка</span><span class="sxs-lookup"><span data-stu-id="924f0-138">String</span></span>|<span data-ttu-id="924f0-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="924f0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="924f0-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-141">description</span><span class="sxs-lookup"><span data-stu-id="924f0-141">description</span></span>|<span data-ttu-id="924f0-142">Строка</span><span class="sxs-lookup"><span data-stu-id="924f0-142">String</span></span>|<span data-ttu-id="924f0-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-143">The description of the app.</span></span> <span data-ttu-id="924f0-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-145">publisher</span><span class="sxs-lookup"><span data-stu-id="924f0-145">publisher</span></span>|<span data-ttu-id="924f0-146">String</span><span class="sxs-lookup"><span data-stu-id="924f0-146">String</span></span>|<span data-ttu-id="924f0-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-147">The publisher of the app.</span></span> <span data-ttu-id="924f0-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="924f0-149">largeIcon</span></span>|[<span data-ttu-id="924f0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="924f0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="924f0-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="924f0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="924f0-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="924f0-153">createdDateTime</span></span>|<span data-ttu-id="924f0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="924f0-154">DateTimeOffset</span></span>|<span data-ttu-id="924f0-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-155">The date and time the app was created.</span></span> <span data-ttu-id="924f0-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="924f0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="924f0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="924f0-158">DateTimeOffset</span></span>|<span data-ttu-id="924f0-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="924f0-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="924f0-161">isFeatured</span></span>|<span data-ttu-id="924f0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="924f0-162">Boolean</span></span>|<span data-ttu-id="924f0-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="924f0-164">privacyInformationUrl</span></span>|<span data-ttu-id="924f0-165">String</span><span class="sxs-lookup"><span data-stu-id="924f0-165">String</span></span>|<span data-ttu-id="924f0-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="924f0-166">The privacy statement Url.</span></span> <span data-ttu-id="924f0-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="924f0-168">informationUrl</span></span>|<span data-ttu-id="924f0-169">String</span><span class="sxs-lookup"><span data-stu-id="924f0-169">String</span></span>|<span data-ttu-id="924f0-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="924f0-170">The more information Url.</span></span> <span data-ttu-id="924f0-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-172">owner</span><span class="sxs-lookup"><span data-stu-id="924f0-172">owner</span></span>|<span data-ttu-id="924f0-173">String</span><span class="sxs-lookup"><span data-stu-id="924f0-173">String</span></span>|<span data-ttu-id="924f0-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-174">The owner of the app.</span></span> <span data-ttu-id="924f0-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-176">developer</span><span class="sxs-lookup"><span data-stu-id="924f0-176">developer</span></span>|<span data-ttu-id="924f0-177">String</span><span class="sxs-lookup"><span data-stu-id="924f0-177">String</span></span>|<span data-ttu-id="924f0-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-178">The developer of the app.</span></span> <span data-ttu-id="924f0-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-180">notes</span><span class="sxs-lookup"><span data-stu-id="924f0-180">notes</span></span>|<span data-ttu-id="924f0-181">String</span><span class="sxs-lookup"><span data-stu-id="924f0-181">String</span></span>|<span data-ttu-id="924f0-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-182">Notes for the app.</span></span> <span data-ttu-id="924f0-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="924f0-184">uploadState</span></span>|<span data-ttu-id="924f0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="924f0-185">Int32</span></span>|<span data-ttu-id="924f0-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="924f0-186">The upload state.</span></span> <span data-ttu-id="924f0-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="924f0-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="924f0-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="924f0-189">publishingState</span></span>|[<span data-ttu-id="924f0-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="924f0-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="924f0-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-191">The publishing state for the app.</span></span> <span data-ttu-id="924f0-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="924f0-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="924f0-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="924f0-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="924f0-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="924f0-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="924f0-195">isAssigned</span></span>|<span data-ttu-id="924f0-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="924f0-196">Boolean</span></span>|<span data-ttu-id="924f0-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="924f0-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="924f0-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="924f0-199">roleScopeTagIds</span></span>|<span data-ttu-id="924f0-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="924f0-200">String collection</span></span>|<span data-ttu-id="924f0-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="924f0-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="924f0-203">dependentAppCount</span></span>|<span data-ttu-id="924f0-204">Int32</span><span class="sxs-lookup"><span data-stu-id="924f0-204">Int32</span></span>|<span data-ttu-id="924f0-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="924f0-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="924f0-207">supersedingAppCount</span></span>|<span data-ttu-id="924f0-208">Int32</span><span class="sxs-lookup"><span data-stu-id="924f0-208">Int32</span></span>|<span data-ttu-id="924f0-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="924f0-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="924f0-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="924f0-211">supersededAppCount</span></span>|<span data-ttu-id="924f0-212">Int32</span><span class="sxs-lookup"><span data-stu-id="924f0-212">Int32</span></span>|<span data-ttu-id="924f0-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="924f0-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="924f0-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="924f0-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="924f0-215">committedContentVersion</span></span>|<span data-ttu-id="924f0-216">String</span><span class="sxs-lookup"><span data-stu-id="924f0-216">String</span></span>|<span data-ttu-id="924f0-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="924f0-217">The internal committed content version.</span></span> <span data-ttu-id="924f0-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="924f0-219">fileName</span><span class="sxs-lookup"><span data-stu-id="924f0-219">fileName</span></span>|<span data-ttu-id="924f0-220">String</span><span class="sxs-lookup"><span data-stu-id="924f0-220">String</span></span>|<span data-ttu-id="924f0-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-221">The name of the main Lob application file.</span></span> <span data-ttu-id="924f0-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="924f0-223">size</span><span class="sxs-lookup"><span data-stu-id="924f0-223">size</span></span>|<span data-ttu-id="924f0-224">Int64</span><span class="sxs-lookup"><span data-stu-id="924f0-224">Int64</span></span>|<span data-ttu-id="924f0-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="924f0-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="924f0-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="924f0-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="924f0-227">инсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="924f0-227">installCommandLine</span></span>|<span data-ttu-id="924f0-228">Строка</span><span class="sxs-lookup"><span data-stu-id="924f0-228">String</span></span>|<span data-ttu-id="924f0-229">Командная строка для установки приложения</span><span class="sxs-lookup"><span data-stu-id="924f0-229">The command line to install this app</span></span>|
|<span data-ttu-id="924f0-230">унинсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="924f0-230">uninstallCommandLine</span></span>|<span data-ttu-id="924f0-231">Строка</span><span class="sxs-lookup"><span data-stu-id="924f0-231">String</span></span>|<span data-ttu-id="924f0-232">Командная строка для удаления приложения</span><span class="sxs-lookup"><span data-stu-id="924f0-232">The command line to uninstall this app</span></span>|
|<span data-ttu-id="924f0-233">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="924f0-233">applicableArchitectures</span></span>|[<span data-ttu-id="924f0-234">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="924f0-234">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="924f0-235">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="924f0-235">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="924f0-236">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="924f0-236">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="924f0-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="924f0-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="924f0-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="924f0-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="924f0-239">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="924f0-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="924f0-240">минимумфридискспацеинмб</span><span class="sxs-lookup"><span data-stu-id="924f0-240">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="924f0-241">Int32</span><span class="sxs-lookup"><span data-stu-id="924f0-241">Int32</span></span>|<span data-ttu-id="924f0-242">Минимальное свободное место на диске, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-242">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="924f0-243">минимуммеморинмб</span><span class="sxs-lookup"><span data-stu-id="924f0-243">minimumMemoryInMB</span></span>|<span data-ttu-id="924f0-244">Int32</span><span class="sxs-lookup"><span data-stu-id="924f0-244">Int32</span></span>|<span data-ttu-id="924f0-245">Значение минимальной физической памяти, необходимой для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-245">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="924f0-246">минимумнумберофпроцессорс</span><span class="sxs-lookup"><span data-stu-id="924f0-246">minimumNumberOfProcessors</span></span>|<span data-ttu-id="924f0-247">Int32</span><span class="sxs-lookup"><span data-stu-id="924f0-247">Int32</span></span>|<span data-ttu-id="924f0-248">Значение минимального числа процессоров, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-248">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="924f0-249">минимумкпуспидинмхз</span><span class="sxs-lookup"><span data-stu-id="924f0-249">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="924f0-250">Int32</span><span class="sxs-lookup"><span data-stu-id="924f0-250">Int32</span></span>|<span data-ttu-id="924f0-251">Значение минимальной скорости ЦП, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-251">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="924f0-252">детектионрулес</span><span class="sxs-lookup"><span data-stu-id="924f0-252">detectionRules</span></span>|<span data-ttu-id="924f0-253">Коллекция [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="924f0-253">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="924f0-254">Правила обнаружения для определения бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="924f0-254">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="924f0-255">рекуирементрулес</span><span class="sxs-lookup"><span data-stu-id="924f0-255">requirementRules</span></span>|<span data-ttu-id="924f0-256">Коллекция [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="924f0-256">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="924f0-257">Правила требований для обнаружения бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="924f0-257">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="924f0-258">правила</span><span class="sxs-lookup"><span data-stu-id="924f0-258">rules</span></span>|<span data-ttu-id="924f0-259">Коллекция [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="924f0-259">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="924f0-260">Правила обнаружения и требований для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-260">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="924f0-261">инсталлекспериенце</span><span class="sxs-lookup"><span data-stu-id="924f0-261">installExperience</span></span>|[<span data-ttu-id="924f0-262">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="924f0-262">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="924f0-263">Установка приложения.</span><span class="sxs-lookup"><span data-stu-id="924f0-263">The install experience for this app.</span></span>|
|<span data-ttu-id="924f0-264">ретурнкодес</span><span class="sxs-lookup"><span data-stu-id="924f0-264">returnCodes</span></span>|<span data-ttu-id="924f0-265">Коллекция [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="924f0-265">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="924f0-266">Коды возврата для поведения после установки.</span><span class="sxs-lookup"><span data-stu-id="924f0-266">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="924f0-267">мсиинформатион</span><span class="sxs-lookup"><span data-stu-id="924f0-267">msiInformation</span></span>|[<span data-ttu-id="924f0-268">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="924f0-268">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="924f0-269">Сведения о MSI, если это приложение Win32 является приложением MSI.</span><span class="sxs-lookup"><span data-stu-id="924f0-269">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="924f0-270">сетупфилепас</span><span class="sxs-lookup"><span data-stu-id="924f0-270">setupFilePath</span></span>|<span data-ttu-id="924f0-271">Строка</span><span class="sxs-lookup"><span data-stu-id="924f0-271">String</span></span>|<span data-ttu-id="924f0-272">Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="924f0-272">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="924f0-273">минимумсуппортедвиндовсрелеасе</span><span class="sxs-lookup"><span data-stu-id="924f0-273">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="924f0-274">Строка</span><span class="sxs-lookup"><span data-stu-id="924f0-274">String</span></span>|<span data-ttu-id="924f0-275">Значение минимального поддерживаемого выпуска Windows.</span><span class="sxs-lookup"><span data-stu-id="924f0-275">The value for the minimum supported windows release.</span></span>|



## <a name="response"></a><span data-ttu-id="924f0-276">Ответ</span><span class="sxs-lookup"><span data-stu-id="924f0-276">Response</span></span>
<span data-ttu-id="924f0-277">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="924f0-277">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="924f0-278">Пример</span><span class="sxs-lookup"><span data-stu-id="924f0-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="924f0-279">Запрос</span><span class="sxs-lookup"><span data-stu-id="924f0-279">Request</span></span>
<span data-ttu-id="924f0-280">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="924f0-280">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 3313

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
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```

### <a name="response"></a><span data-ttu-id="924f0-281">Отклик</span><span class="sxs-lookup"><span data-stu-id="924f0-281">Response</span></span>
<span data-ttu-id="924f0-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="924f0-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3485

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
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```





