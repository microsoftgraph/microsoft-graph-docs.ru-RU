---
title: Обновление windowsPhone81AppXBundle
description: Обновление свойств объекта windowsPhone81AppXBundle.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 320015c29fa42ca63a1addaf7c3a8fbf3224052d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976328"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="adbff-103">Обновление windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="adbff-103">Update windowsPhone81AppXBundle</span></span>

<span data-ttu-id="adbff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adbff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="adbff-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adbff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adbff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="adbff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adbff-107">Обновление свойств объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="adbff-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adbff-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="adbff-108">Prerequisites</span></span>
<span data-ttu-id="adbff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adbff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adbff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adbff-111">Permission type</span></span>|<span data-ttu-id="adbff-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="adbff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adbff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adbff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adbff-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adbff-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="adbff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adbff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adbff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adbff-116">Not supported.</span></span>|
|<span data-ttu-id="adbff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adbff-117">Application</span></span>|<span data-ttu-id="adbff-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adbff-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="adbff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adbff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="adbff-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="adbff-120">Request headers</span></span>
|<span data-ttu-id="adbff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="adbff-121">Header</span></span>|<span data-ttu-id="adbff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="adbff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adbff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="adbff-123">Authorization</span></span>|<span data-ttu-id="adbff-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="adbff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adbff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="adbff-125">Accept</span></span>|<span data-ttu-id="adbff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="adbff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adbff-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="adbff-127">Request body</span></span>
<span data-ttu-id="adbff-128">В тексте запроса добавьте представление объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adbff-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="adbff-129">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="adbff-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="adbff-130">Property</span></span>|<span data-ttu-id="adbff-131">Тип</span><span class="sxs-lookup"><span data-stu-id="adbff-131">Type</span></span>|<span data-ttu-id="adbff-132">Описание</span><span class="sxs-lookup"><span data-stu-id="adbff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adbff-133">id</span><span class="sxs-lookup"><span data-stu-id="adbff-133">id</span></span>|<span data-ttu-id="adbff-134">String</span><span class="sxs-lookup"><span data-stu-id="adbff-134">String</span></span>|<span data-ttu-id="adbff-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="adbff-135">Key of the entity.</span></span> <span data-ttu-id="adbff-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-137">displayName</span><span class="sxs-lookup"><span data-stu-id="adbff-137">displayName</span></span>|<span data-ttu-id="adbff-138">String</span><span class="sxs-lookup"><span data-stu-id="adbff-138">String</span></span>|<span data-ttu-id="adbff-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="adbff-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="adbff-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-141">description</span><span class="sxs-lookup"><span data-stu-id="adbff-141">description</span></span>|<span data-ttu-id="adbff-142">String</span><span class="sxs-lookup"><span data-stu-id="adbff-142">String</span></span>|<span data-ttu-id="adbff-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="adbff-143">The description of the app.</span></span> <span data-ttu-id="adbff-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-145">publisher</span><span class="sxs-lookup"><span data-stu-id="adbff-145">publisher</span></span>|<span data-ttu-id="adbff-146">String</span><span class="sxs-lookup"><span data-stu-id="adbff-146">String</span></span>|<span data-ttu-id="adbff-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="adbff-147">The publisher of the app.</span></span> <span data-ttu-id="adbff-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="adbff-149">largeIcon</span></span>|[<span data-ttu-id="adbff-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="adbff-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="adbff-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="adbff-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="adbff-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="adbff-153">createdDateTime</span></span>|<span data-ttu-id="adbff-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adbff-154">DateTimeOffset</span></span>|<span data-ttu-id="adbff-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="adbff-155">The date and time the app was created.</span></span> <span data-ttu-id="adbff-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="adbff-157">lastModifiedDateTime</span></span>|<span data-ttu-id="adbff-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adbff-158">DateTimeOffset</span></span>|<span data-ttu-id="adbff-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="adbff-159">The date and time the app was last modified.</span></span> <span data-ttu-id="adbff-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="adbff-161">isFeatured</span></span>|<span data-ttu-id="adbff-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="adbff-162">Boolean</span></span>|<span data-ttu-id="adbff-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="adbff-164">privacyInformationUrl</span></span>|<span data-ttu-id="adbff-165">String</span><span class="sxs-lookup"><span data-stu-id="adbff-165">String</span></span>|<span data-ttu-id="adbff-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="adbff-166">The privacy statement Url.</span></span> <span data-ttu-id="adbff-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="adbff-168">informationUrl</span></span>|<span data-ttu-id="adbff-169">String</span><span class="sxs-lookup"><span data-stu-id="adbff-169">String</span></span>|<span data-ttu-id="adbff-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="adbff-170">The more information Url.</span></span> <span data-ttu-id="adbff-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-172">owner</span><span class="sxs-lookup"><span data-stu-id="adbff-172">owner</span></span>|<span data-ttu-id="adbff-173">String</span><span class="sxs-lookup"><span data-stu-id="adbff-173">String</span></span>|<span data-ttu-id="adbff-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="adbff-174">The owner of the app.</span></span> <span data-ttu-id="adbff-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-176">developer</span><span class="sxs-lookup"><span data-stu-id="adbff-176">developer</span></span>|<span data-ttu-id="adbff-177">String</span><span class="sxs-lookup"><span data-stu-id="adbff-177">String</span></span>|<span data-ttu-id="adbff-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="adbff-178">The developer of the app.</span></span> <span data-ttu-id="adbff-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-180">notes</span><span class="sxs-lookup"><span data-stu-id="adbff-180">notes</span></span>|<span data-ttu-id="adbff-181">String</span><span class="sxs-lookup"><span data-stu-id="adbff-181">String</span></span>|<span data-ttu-id="adbff-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="adbff-182">Notes for the app.</span></span> <span data-ttu-id="adbff-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="adbff-184">uploadState</span></span>|<span data-ttu-id="adbff-185">Int32</span><span class="sxs-lookup"><span data-stu-id="adbff-185">Int32</span></span>|<span data-ttu-id="adbff-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="adbff-186">The upload state.</span></span> <span data-ttu-id="adbff-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="adbff-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="adbff-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="adbff-189">publishingState</span></span>|[<span data-ttu-id="adbff-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="adbff-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="adbff-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="adbff-191">The publishing state for the app.</span></span> <span data-ttu-id="adbff-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="adbff-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="adbff-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="adbff-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="adbff-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="adbff-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="adbff-195">isAssigned</span></span>|<span data-ttu-id="adbff-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="adbff-196">Boolean</span></span>|<span data-ttu-id="adbff-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="adbff-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="adbff-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="adbff-199">roleScopeTagIds</span></span>|<span data-ttu-id="adbff-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="adbff-200">String collection</span></span>|<span data-ttu-id="adbff-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="adbff-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="adbff-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="adbff-203">dependentAppCount</span></span>|<span data-ttu-id="adbff-204">Int32</span><span class="sxs-lookup"><span data-stu-id="adbff-204">Int32</span></span>|<span data-ttu-id="adbff-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="adbff-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="adbff-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="adbff-207">supersedingAppCount</span></span>|<span data-ttu-id="adbff-208">Int32</span><span class="sxs-lookup"><span data-stu-id="adbff-208">Int32</span></span>|<span data-ttu-id="adbff-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="adbff-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="adbff-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="adbff-211">supersededAppCount</span></span>|<span data-ttu-id="adbff-212">Int32</span><span class="sxs-lookup"><span data-stu-id="adbff-212">Int32</span></span>|<span data-ttu-id="adbff-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="adbff-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="adbff-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="adbff-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="adbff-215">committedContentVersion</span></span>|<span data-ttu-id="adbff-216">String</span><span class="sxs-lookup"><span data-stu-id="adbff-216">String</span></span>|<span data-ttu-id="adbff-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="adbff-217">The internal committed content version.</span></span> <span data-ttu-id="adbff-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="adbff-219">fileName</span><span class="sxs-lookup"><span data-stu-id="adbff-219">fileName</span></span>|<span data-ttu-id="adbff-220">String</span><span class="sxs-lookup"><span data-stu-id="adbff-220">String</span></span>|<span data-ttu-id="adbff-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="adbff-221">The name of the main Lob application file.</span></span> <span data-ttu-id="adbff-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="adbff-223">size</span><span class="sxs-lookup"><span data-stu-id="adbff-223">size</span></span>|<span data-ttu-id="adbff-224">Int64</span><span class="sxs-lookup"><span data-stu-id="adbff-224">Int64</span></span>|<span data-ttu-id="adbff-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="adbff-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="adbff-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="adbff-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="adbff-227">applicableArchitectures</span></span>|[<span data-ttu-id="adbff-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="adbff-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="adbff-229">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="adbff-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="adbff-230">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="adbff-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="adbff-231">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="adbff-231">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="adbff-232">identityName</span><span class="sxs-lookup"><span data-stu-id="adbff-232">identityName</span></span>|<span data-ttu-id="adbff-233">String</span><span class="sxs-lookup"><span data-stu-id="adbff-233">String</span></span>|<span data-ttu-id="adbff-234">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="adbff-234">The Identity Name.</span></span> <span data-ttu-id="adbff-235">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="adbff-235">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="adbff-236">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="adbff-236">identityPublisherHash</span></span>|<span data-ttu-id="adbff-237">String</span><span class="sxs-lookup"><span data-stu-id="adbff-237">String</span></span>|<span data-ttu-id="adbff-238">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="adbff-238">The Identity Publisher Hash.</span></span> <span data-ttu-id="adbff-239">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="adbff-239">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="adbff-240">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="adbff-240">identityResourceIdentifier</span></span>|<span data-ttu-id="adbff-241">String</span><span class="sxs-lookup"><span data-stu-id="adbff-241">String</span></span>|<span data-ttu-id="adbff-242">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="adbff-242">The Identity Resource Identifier.</span></span> <span data-ttu-id="adbff-243">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="adbff-243">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="adbff-244">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="adbff-244">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="adbff-245">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="adbff-245">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="adbff-246">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="adbff-246">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="adbff-247">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="adbff-247">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="adbff-248">фонепродуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="adbff-248">phoneProductIdentifier</span></span>|<span data-ttu-id="adbff-249">String</span><span class="sxs-lookup"><span data-stu-id="adbff-249">String</span></span>|<span data-ttu-id="adbff-250">Идентификатор телефонного продукта.</span><span class="sxs-lookup"><span data-stu-id="adbff-250">The Phone Product Identifier.</span></span> <span data-ttu-id="adbff-251">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="adbff-251">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="adbff-252">фонепублишерид</span><span class="sxs-lookup"><span data-stu-id="adbff-252">phonePublisherId</span></span>|<span data-ttu-id="adbff-253">String</span><span class="sxs-lookup"><span data-stu-id="adbff-253">String</span></span>|<span data-ttu-id="adbff-254">Идентификатор издателя телефона. наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="adbff-254">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="adbff-255">identityVersion</span><span class="sxs-lookup"><span data-stu-id="adbff-255">identityVersion</span></span>|<span data-ttu-id="adbff-256">String</span><span class="sxs-lookup"><span data-stu-id="adbff-256">String</span></span>|<span data-ttu-id="adbff-257">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="adbff-257">The identity version.</span></span> <span data-ttu-id="adbff-258">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="adbff-258">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="adbff-259">аппкспаккажеинформатионлист</span><span class="sxs-lookup"><span data-stu-id="adbff-259">appXPackageInformationList</span></span>|<span data-ttu-id="adbff-260">Коллекция [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="adbff-260">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="adbff-261">Список сведений о пакете AppX.</span><span class="sxs-lookup"><span data-stu-id="adbff-261">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="adbff-262">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbff-262">Response</span></span>
<span data-ttu-id="adbff-263">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="adbff-263">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adbff-264">Пример</span><span class="sxs-lookup"><span data-stu-id="adbff-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="adbff-265">Запрос</span><span class="sxs-lookup"><span data-stu-id="adbff-265">Request</span></span>
<span data-ttu-id="adbff-266">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adbff-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2368

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="adbff-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbff-267">Response</span></span>
<span data-ttu-id="adbff-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adbff-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2540

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
      }
    }
  ]
}
```






