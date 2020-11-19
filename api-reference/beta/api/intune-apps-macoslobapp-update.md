---
title: Обновление Макослобапп
description: Обновление свойств объекта Макослобапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cefac058fd38ac1cc8f45dbb16be01912fd8ae2d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49251523"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="24c6a-103">Обновление Макослобапп</span><span class="sxs-lookup"><span data-stu-id="24c6a-103">Update macOSLobApp</span></span>

<span data-ttu-id="24c6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24c6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24c6a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24c6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24c6a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24c6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24c6a-107">Обновление свойств объекта [макослобапп](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="24c6a-107">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24c6a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24c6a-108">Prerequisites</span></span>
<span data-ttu-id="24c6a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24c6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24c6a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24c6a-111">Permission type</span></span>|<span data-ttu-id="24c6a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24c6a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24c6a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24c6a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24c6a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24c6a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="24c6a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24c6a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24c6a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24c6a-116">Not supported.</span></span>|
|<span data-ttu-id="24c6a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="24c6a-117">Application</span></span>|<span data-ttu-id="24c6a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24c6a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24c6a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24c6a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="24c6a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24c6a-120">Request headers</span></span>
|<span data-ttu-id="24c6a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24c6a-121">Header</span></span>|<span data-ttu-id="24c6a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="24c6a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24c6a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24c6a-123">Authorization</span></span>|<span data-ttu-id="24c6a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24c6a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24c6a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24c6a-125">Accept</span></span>|<span data-ttu-id="24c6a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24c6a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24c6a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24c6a-127">Request body</span></span>
<span data-ttu-id="24c6a-128">В тексте запроса добавьте представление объекта [макослобапп](../resources/intune-apps-macoslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24c6a-128">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="24c6a-129">В следующей таблице приведены свойства, необходимые при создании [макослобапп](../resources/intune-apps-macoslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-129">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="24c6a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="24c6a-130">Property</span></span>|<span data-ttu-id="24c6a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="24c6a-131">Type</span></span>|<span data-ttu-id="24c6a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="24c6a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24c6a-133">id</span><span class="sxs-lookup"><span data-stu-id="24c6a-133">id</span></span>|<span data-ttu-id="24c6a-134">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-134">String</span></span>|<span data-ttu-id="24c6a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="24c6a-135">Key of the entity.</span></span> <span data-ttu-id="24c6a-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="24c6a-137">displayName</span></span>|<span data-ttu-id="24c6a-138">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-138">String</span></span>|<span data-ttu-id="24c6a-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="24c6a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="24c6a-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-141">description</span><span class="sxs-lookup"><span data-stu-id="24c6a-141">description</span></span>|<span data-ttu-id="24c6a-142">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-142">String</span></span>|<span data-ttu-id="24c6a-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="24c6a-143">The description of the app.</span></span> <span data-ttu-id="24c6a-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-145">publisher</span><span class="sxs-lookup"><span data-stu-id="24c6a-145">publisher</span></span>|<span data-ttu-id="24c6a-146">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-146">String</span></span>|<span data-ttu-id="24c6a-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="24c6a-147">The publisher of the app.</span></span> <span data-ttu-id="24c6a-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="24c6a-149">largeIcon</span></span>|[<span data-ttu-id="24c6a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="24c6a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="24c6a-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="24c6a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="24c6a-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24c6a-153">createdDateTime</span></span>|<span data-ttu-id="24c6a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24c6a-154">DateTimeOffset</span></span>|<span data-ttu-id="24c6a-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="24c6a-155">The date and time the app was created.</span></span> <span data-ttu-id="24c6a-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24c6a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="24c6a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24c6a-158">DateTimeOffset</span></span>|<span data-ttu-id="24c6a-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="24c6a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="24c6a-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="24c6a-161">isFeatured</span></span>|<span data-ttu-id="24c6a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="24c6a-162">Boolean</span></span>|<span data-ttu-id="24c6a-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="24c6a-164">privacyInformationUrl</span></span>|<span data-ttu-id="24c6a-165">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-165">String</span></span>|<span data-ttu-id="24c6a-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="24c6a-166">The privacy statement Url.</span></span> <span data-ttu-id="24c6a-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="24c6a-168">informationUrl</span></span>|<span data-ttu-id="24c6a-169">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-169">String</span></span>|<span data-ttu-id="24c6a-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="24c6a-170">The more information Url.</span></span> <span data-ttu-id="24c6a-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-172">owner</span><span class="sxs-lookup"><span data-stu-id="24c6a-172">owner</span></span>|<span data-ttu-id="24c6a-173">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-173">String</span></span>|<span data-ttu-id="24c6a-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="24c6a-174">The owner of the app.</span></span> <span data-ttu-id="24c6a-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-176">developer</span><span class="sxs-lookup"><span data-stu-id="24c6a-176">developer</span></span>|<span data-ttu-id="24c6a-177">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-177">String</span></span>|<span data-ttu-id="24c6a-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="24c6a-178">The developer of the app.</span></span> <span data-ttu-id="24c6a-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-180">notes</span><span class="sxs-lookup"><span data-stu-id="24c6a-180">notes</span></span>|<span data-ttu-id="24c6a-181">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-181">String</span></span>|<span data-ttu-id="24c6a-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="24c6a-182">Notes for the app.</span></span> <span data-ttu-id="24c6a-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="24c6a-184">uploadState</span></span>|<span data-ttu-id="24c6a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="24c6a-185">Int32</span></span>|<span data-ttu-id="24c6a-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="24c6a-186">The upload state.</span></span> <span data-ttu-id="24c6a-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="24c6a-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="24c6a-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="24c6a-189">publishingState</span></span>|[<span data-ttu-id="24c6a-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="24c6a-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="24c6a-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="24c6a-191">The publishing state for the app.</span></span> <span data-ttu-id="24c6a-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="24c6a-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="24c6a-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="24c6a-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="24c6a-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="24c6a-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="24c6a-195">isAssigned</span></span>|<span data-ttu-id="24c6a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="24c6a-196">Boolean</span></span>|<span data-ttu-id="24c6a-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="24c6a-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="24c6a-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="24c6a-199">roleScopeTagIds</span></span>|<span data-ttu-id="24c6a-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="24c6a-200">String collection</span></span>|<span data-ttu-id="24c6a-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="24c6a-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="24c6a-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="24c6a-203">dependentAppCount</span></span>|<span data-ttu-id="24c6a-204">Int32</span><span class="sxs-lookup"><span data-stu-id="24c6a-204">Int32</span></span>|<span data-ttu-id="24c6a-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="24c6a-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="24c6a-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="24c6a-207">supersedingAppCount</span></span>|<span data-ttu-id="24c6a-208">Int32</span><span class="sxs-lookup"><span data-stu-id="24c6a-208">Int32</span></span>|<span data-ttu-id="24c6a-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="24c6a-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="24c6a-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="24c6a-211">supersededAppCount</span></span>|<span data-ttu-id="24c6a-212">Int32</span><span class="sxs-lookup"><span data-stu-id="24c6a-212">Int32</span></span>|<span data-ttu-id="24c6a-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="24c6a-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="24c6a-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="24c6a-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="24c6a-215">committedContentVersion</span></span>|<span data-ttu-id="24c6a-216">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-216">String</span></span>|<span data-ttu-id="24c6a-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="24c6a-217">The internal committed content version.</span></span> <span data-ttu-id="24c6a-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="24c6a-219">fileName</span><span class="sxs-lookup"><span data-stu-id="24c6a-219">fileName</span></span>|<span data-ttu-id="24c6a-220">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-220">String</span></span>|<span data-ttu-id="24c6a-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="24c6a-221">The name of the main Lob application file.</span></span> <span data-ttu-id="24c6a-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="24c6a-223">size</span><span class="sxs-lookup"><span data-stu-id="24c6a-223">size</span></span>|<span data-ttu-id="24c6a-224">Int64</span><span class="sxs-lookup"><span data-stu-id="24c6a-224">Int64</span></span>|<span data-ttu-id="24c6a-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="24c6a-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="24c6a-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="24c6a-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="24c6a-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="24c6a-227">bundleId</span></span>|<span data-ttu-id="24c6a-228">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-228">String</span></span>|<span data-ttu-id="24c6a-229">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="24c6a-229">The bundle id.</span></span>|
|<span data-ttu-id="24c6a-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="24c6a-230">minimumSupportedOperatingSystem</span></span>|<span data-ttu-id="24c6a-231">[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md);</span><span class="sxs-lookup"><span data-stu-id="24c6a-231">[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md)</span></span>|<span data-ttu-id="24c6a-232">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="24c6a-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="24c6a-233">buildNumber</span><span class="sxs-lookup"><span data-stu-id="24c6a-233">buildNumber</span></span>|<span data-ttu-id="24c6a-234">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-234">String</span></span>|<span data-ttu-id="24c6a-235">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="24c6a-235">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="24c6a-236">versionNumber</span><span class="sxs-lookup"><span data-stu-id="24c6a-236">versionNumber</span></span>|<span data-ttu-id="24c6a-237">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-237">String</span></span>|<span data-ttu-id="24c6a-238">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="24c6a-238">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="24c6a-239">чилдаппс</span><span class="sxs-lookup"><span data-stu-id="24c6a-239">childApps</span></span>|<span data-ttu-id="24c6a-240">Коллекция [макослобчилдапп](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="24c6a-240">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="24c6a-241">Список приложений в этом пакете набора</span><span class="sxs-lookup"><span data-stu-id="24c6a-241">The app list in this bundle package</span></span>|
|<span data-ttu-id="24c6a-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="24c6a-242">identityVersion</span></span>|<span data-ttu-id="24c6a-243">String</span><span class="sxs-lookup"><span data-stu-id="24c6a-243">String</span></span>|<span data-ttu-id="24c6a-244">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="24c6a-244">The identity version.</span></span>|
|<span data-ttu-id="24c6a-245">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="24c6a-245">md5HashChunkSize</span></span>|<span data-ttu-id="24c6a-246">Int32</span><span class="sxs-lookup"><span data-stu-id="24c6a-246">Int32</span></span>|<span data-ttu-id="24c6a-247">Размер фрагмента для хеша MD5</span><span class="sxs-lookup"><span data-stu-id="24c6a-247">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="24c6a-248">md5Hash</span><span class="sxs-lookup"><span data-stu-id="24c6a-248">md5Hash</span></span>|<span data-ttu-id="24c6a-249">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="24c6a-249">String collection</span></span>|<span data-ttu-id="24c6a-250">Хэш-коды MD5</span><span class="sxs-lookup"><span data-stu-id="24c6a-250">The MD5 hash codes</span></span>|
|<span data-ttu-id="24c6a-251">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="24c6a-251">ignoreVersionDetection</span></span>|<span data-ttu-id="24c6a-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="24c6a-252">Boolean</span></span>|<span data-ttu-id="24c6a-253">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="24c6a-253">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="24c6a-254">Установите для этого параметра значение true для бизнес-приложений macOS (LoB), использующих функцию самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="24c6a-254">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="24c6a-255">инсталласманажед</span><span class="sxs-lookup"><span data-stu-id="24c6a-255">installAsManaged</span></span>|<span data-ttu-id="24c6a-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="24c6a-256">Boolean</span></span>|<span data-ttu-id="24c6a-257">Логическое значение, определяющее, будет ли приложение устанавливаться как управляемое (требуется macOS 11,0 и другие ограничения PKG).</span><span class="sxs-lookup"><span data-stu-id="24c6a-257">A boolean to control whether the app will be installed as managed (requires macOS 11.0 and other PKG restrictions).</span></span>|



## <a name="response"></a><span data-ttu-id="24c6a-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="24c6a-258">Response</span></span>
<span data-ttu-id="24c6a-259">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макослобапп](../resources/intune-apps-macoslobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24c6a-259">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24c6a-260">Пример</span><span class="sxs-lookup"><span data-stu-id="24c6a-260">Example</span></span>

### <a name="request"></a><span data-ttu-id="24c6a-261">Запрос</span><span class="sxs-lookup"><span data-stu-id="24c6a-261">Request</span></span>
<span data-ttu-id="24c6a-262">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24c6a-262">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1702

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true,
  "installAsManaged": true
}
```

### <a name="response"></a><span data-ttu-id="24c6a-263">Отклик</span><span class="sxs-lookup"><span data-stu-id="24c6a-263">Response</span></span>
<span data-ttu-id="24c6a-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24c6a-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1874

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true,
  "installAsManaged": true
}
```




