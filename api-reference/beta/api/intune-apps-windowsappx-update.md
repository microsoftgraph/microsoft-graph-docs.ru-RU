---
title: Обновление windowsAppX
description: Обновление свойств объекта windowsAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 10ea9854ac8e9720f06393943e798224e91adf28
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976601"
---
# <a name="update-windowsappx"></a><span data-ttu-id="4deb6-103">Обновление windowsAppX</span><span class="sxs-lookup"><span data-stu-id="4deb6-103">Update windowsAppX</span></span>

<span data-ttu-id="4deb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4deb6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4deb6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4deb6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4deb6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4deb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4deb6-107">Обновление свойств объекта [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="4deb6-107">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4deb6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4deb6-108">Prerequisites</span></span>
<span data-ttu-id="4deb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4deb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4deb6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4deb6-111">Permission type</span></span>|<span data-ttu-id="4deb6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4deb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4deb6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4deb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4deb6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4deb6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4deb6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4deb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4deb6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4deb6-116">Not supported.</span></span>|
|<span data-ttu-id="4deb6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4deb6-117">Application</span></span>|<span data-ttu-id="4deb6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4deb6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4deb6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4deb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4deb6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4deb6-120">Request headers</span></span>
|<span data-ttu-id="4deb6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4deb6-121">Header</span></span>|<span data-ttu-id="4deb6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4deb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4deb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4deb6-123">Authorization</span></span>|<span data-ttu-id="4deb6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4deb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4deb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4deb6-125">Accept</span></span>|<span data-ttu-id="4deb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4deb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4deb6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4deb6-127">Request body</span></span>
<span data-ttu-id="4deb6-128">В тексте запроса добавьте представление объекта [windowsAppX](../resources/intune-apps-windowsappx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4deb6-128">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="4deb6-129">В следующей таблице приведены свойства, необходимые при создании [windowsAppX](../resources/intune-apps-windowsappx.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-129">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="4deb6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4deb6-130">Property</span></span>|<span data-ttu-id="4deb6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4deb6-131">Type</span></span>|<span data-ttu-id="4deb6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4deb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4deb6-133">id</span><span class="sxs-lookup"><span data-stu-id="4deb6-133">id</span></span>|<span data-ttu-id="4deb6-134">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-134">String</span></span>|<span data-ttu-id="4deb6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4deb6-135">Key of the entity.</span></span> <span data-ttu-id="4deb6-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4deb6-137">displayName</span></span>|<span data-ttu-id="4deb6-138">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-138">String</span></span>|<span data-ttu-id="4deb6-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="4deb6-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4deb6-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-141">description</span><span class="sxs-lookup"><span data-stu-id="4deb6-141">description</span></span>|<span data-ttu-id="4deb6-142">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-142">String</span></span>|<span data-ttu-id="4deb6-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-143">The description of the app.</span></span> <span data-ttu-id="4deb6-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-145">publisher</span><span class="sxs-lookup"><span data-stu-id="4deb6-145">publisher</span></span>|<span data-ttu-id="4deb6-146">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-146">String</span></span>|<span data-ttu-id="4deb6-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-147">The publisher of the app.</span></span> <span data-ttu-id="4deb6-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4deb6-149">largeIcon</span></span>|[<span data-ttu-id="4deb6-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4deb6-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4deb6-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="4deb6-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4deb6-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4deb6-153">createdDateTime</span></span>|<span data-ttu-id="4deb6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4deb6-154">DateTimeOffset</span></span>|<span data-ttu-id="4deb6-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-155">The date and time the app was created.</span></span> <span data-ttu-id="4deb6-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4deb6-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4deb6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4deb6-158">DateTimeOffset</span></span>|<span data-ttu-id="4deb6-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4deb6-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4deb6-161">isFeatured</span></span>|<span data-ttu-id="4deb6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4deb6-162">Boolean</span></span>|<span data-ttu-id="4deb6-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4deb6-164">privacyInformationUrl</span></span>|<span data-ttu-id="4deb6-165">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-165">String</span></span>|<span data-ttu-id="4deb6-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4deb6-166">The privacy statement Url.</span></span> <span data-ttu-id="4deb6-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4deb6-168">informationUrl</span></span>|<span data-ttu-id="4deb6-169">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-169">String</span></span>|<span data-ttu-id="4deb6-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="4deb6-170">The more information Url.</span></span> <span data-ttu-id="4deb6-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-172">owner</span><span class="sxs-lookup"><span data-stu-id="4deb6-172">owner</span></span>|<span data-ttu-id="4deb6-173">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-173">String</span></span>|<span data-ttu-id="4deb6-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-174">The owner of the app.</span></span> <span data-ttu-id="4deb6-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-176">developer</span><span class="sxs-lookup"><span data-stu-id="4deb6-176">developer</span></span>|<span data-ttu-id="4deb6-177">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-177">String</span></span>|<span data-ttu-id="4deb6-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-178">The developer of the app.</span></span> <span data-ttu-id="4deb6-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-180">notes</span><span class="sxs-lookup"><span data-stu-id="4deb6-180">notes</span></span>|<span data-ttu-id="4deb6-181">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-181">String</span></span>|<span data-ttu-id="4deb6-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-182">Notes for the app.</span></span> <span data-ttu-id="4deb6-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4deb6-184">uploadState</span></span>|<span data-ttu-id="4deb6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4deb6-185">Int32</span></span>|<span data-ttu-id="4deb6-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="4deb6-186">The upload state.</span></span> <span data-ttu-id="4deb6-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="4deb6-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="4deb6-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="4deb6-189">publishingState</span></span>|[<span data-ttu-id="4deb6-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="4deb6-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4deb6-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-191">The publishing state for the app.</span></span> <span data-ttu-id="4deb6-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="4deb6-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4deb6-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4deb6-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4deb6-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4deb6-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4deb6-195">isAssigned</span></span>|<span data-ttu-id="4deb6-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="4deb6-196">Boolean</span></span>|<span data-ttu-id="4deb6-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="4deb6-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4deb6-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4deb6-199">roleScopeTagIds</span></span>|<span data-ttu-id="4deb6-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4deb6-200">String collection</span></span>|<span data-ttu-id="4deb6-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4deb6-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="4deb6-203">dependentAppCount</span></span>|<span data-ttu-id="4deb6-204">Int32</span><span class="sxs-lookup"><span data-stu-id="4deb6-204">Int32</span></span>|<span data-ttu-id="4deb6-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4deb6-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="4deb6-207">supersedingAppCount</span></span>|<span data-ttu-id="4deb6-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4deb6-208">Int32</span></span>|<span data-ttu-id="4deb6-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="4deb6-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="4deb6-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="4deb6-211">supersededAppCount</span></span>|<span data-ttu-id="4deb6-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4deb6-212">Int32</span></span>|<span data-ttu-id="4deb6-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="4deb6-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="4deb6-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4deb6-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4deb6-215">committedContentVersion</span></span>|<span data-ttu-id="4deb6-216">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-216">String</span></span>|<span data-ttu-id="4deb6-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="4deb6-217">The internal committed content version.</span></span> <span data-ttu-id="4deb6-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4deb6-219">fileName</span><span class="sxs-lookup"><span data-stu-id="4deb6-219">fileName</span></span>|<span data-ttu-id="4deb6-220">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-220">String</span></span>|<span data-ttu-id="4deb6-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-221">The name of the main Lob application file.</span></span> <span data-ttu-id="4deb6-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4deb6-223">size</span><span class="sxs-lookup"><span data-stu-id="4deb6-223">size</span></span>|<span data-ttu-id="4deb6-224">Int64</span><span class="sxs-lookup"><span data-stu-id="4deb6-224">Int64</span></span>|<span data-ttu-id="4deb6-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="4deb6-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="4deb6-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4deb6-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4deb6-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="4deb6-227">applicableArchitectures</span></span>|[<span data-ttu-id="4deb6-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="4deb6-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="4deb6-229">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="4deb6-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="4deb6-230">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="4deb6-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="4deb6-231">identityName</span><span class="sxs-lookup"><span data-stu-id="4deb6-231">identityName</span></span>|<span data-ttu-id="4deb6-232">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-232">String</span></span>|<span data-ttu-id="4deb6-233">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-233">The Identity Name.</span></span>|
|<span data-ttu-id="4deb6-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="4deb6-234">identityPublisherHash</span></span>|<span data-ttu-id="4deb6-235">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-235">String</span></span>|<span data-ttu-id="4deb6-236">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="4deb6-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="4deb6-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4deb6-237">identityResourceIdentifier</span></span>|<span data-ttu-id="4deb6-238">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-238">String</span></span>|<span data-ttu-id="4deb6-239">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="4deb6-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="4deb6-240">isBundle</span><span class="sxs-lookup"><span data-stu-id="4deb6-240">isBundle</span></span>|<span data-ttu-id="4deb6-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="4deb6-241">Boolean</span></span>|<span data-ttu-id="4deb6-242">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="4deb6-242">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="4deb6-243">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4deb6-243">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4deb6-244">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4deb6-244">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="4deb6-245">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="4deb6-245">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4deb6-246">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4deb6-246">identityVersion</span></span>|<span data-ttu-id="4deb6-247">String</span><span class="sxs-lookup"><span data-stu-id="4deb6-247">String</span></span>|<span data-ttu-id="4deb6-248">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4deb6-248">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="4deb6-249">Ответ</span><span class="sxs-lookup"><span data-stu-id="4deb6-249">Response</span></span>
<span data-ttu-id="4deb6-250">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsAppX](../resources/intune-apps-windowsappx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4deb6-250">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4deb6-251">Пример</span><span class="sxs-lookup"><span data-stu-id="4deb6-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="4deb6-252">Запрос</span><span class="sxs-lookup"><span data-stu-id="4deb6-252">Request</span></span>
<span data-ttu-id="4deb6-253">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4deb6-253">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1470

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="4deb6-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="4deb6-254">Response</span></span>
<span data-ttu-id="4deb6-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4deb6-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1642

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```






