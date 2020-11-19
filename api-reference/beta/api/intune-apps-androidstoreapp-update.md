---
title: Update androidStoreApp
description: Обновление свойств объекта androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8ceb1f10fdc48881f077519aa62d0e0d8a15e58
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49253231"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="3b047-103">Update androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="3b047-103">Update androidStoreApp</span></span>

<span data-ttu-id="3b047-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b047-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b047-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b047-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b047-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b047-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b047-107">Обновление свойств объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-107">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b047-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3b047-108">Prerequisites</span></span>
<span data-ttu-id="3b047-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b047-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b047-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b047-111">Permission type</span></span>|<span data-ttu-id="3b047-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b047-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b047-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b047-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b047-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b047-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3b047-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b047-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b047-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b047-116">Not supported.</span></span>|
|<span data-ttu-id="3b047-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3b047-117">Application</span></span>|<span data-ttu-id="3b047-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b047-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b047-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b047-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="3b047-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3b047-120">Request headers</span></span>
|<span data-ttu-id="3b047-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b047-121">Header</span></span>|<span data-ttu-id="3b047-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3b047-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b047-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b047-123">Authorization</span></span>|<span data-ttu-id="3b047-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b047-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b047-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b047-125">Accept</span></span>|<span data-ttu-id="3b047-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b047-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b047-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b047-127">Request body</span></span>
<span data-ttu-id="3b047-128">В теле запроса добавьте представление объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b047-128">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="3b047-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-129">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="3b047-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b047-130">Property</span></span>|<span data-ttu-id="3b047-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3b047-131">Type</span></span>|<span data-ttu-id="3b047-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3b047-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b047-133">id</span><span class="sxs-lookup"><span data-stu-id="3b047-133">id</span></span>|<span data-ttu-id="3b047-134">String</span><span class="sxs-lookup"><span data-stu-id="3b047-134">String</span></span>|<span data-ttu-id="3b047-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3b047-135">Key of the entity.</span></span> <span data-ttu-id="3b047-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3b047-137">displayName</span></span>|<span data-ttu-id="3b047-138">String</span><span class="sxs-lookup"><span data-stu-id="3b047-138">String</span></span>|<span data-ttu-id="3b047-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="3b047-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3b047-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-141">description</span><span class="sxs-lookup"><span data-stu-id="3b047-141">description</span></span>|<span data-ttu-id="3b047-142">String</span><span class="sxs-lookup"><span data-stu-id="3b047-142">String</span></span>|<span data-ttu-id="3b047-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="3b047-143">The description of the app.</span></span> <span data-ttu-id="3b047-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3b047-145">publisher</span></span>|<span data-ttu-id="3b047-146">String</span><span class="sxs-lookup"><span data-stu-id="3b047-146">String</span></span>|<span data-ttu-id="3b047-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="3b047-147">The publisher of the app.</span></span> <span data-ttu-id="3b047-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3b047-149">largeIcon</span></span>|[<span data-ttu-id="3b047-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3b047-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3b047-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="3b047-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3b047-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b047-153">createdDateTime</span></span>|<span data-ttu-id="3b047-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b047-154">DateTimeOffset</span></span>|<span data-ttu-id="3b047-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="3b047-155">The date and time the app was created.</span></span> <span data-ttu-id="3b047-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b047-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3b047-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b047-158">DateTimeOffset</span></span>|<span data-ttu-id="3b047-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="3b047-159">The date and time the app was last modified.</span></span> <span data-ttu-id="3b047-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3b047-161">isFeatured</span></span>|<span data-ttu-id="3b047-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b047-162">Boolean</span></span>|<span data-ttu-id="3b047-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3b047-164">privacyInformationUrl</span></span>|<span data-ttu-id="3b047-165">String</span><span class="sxs-lookup"><span data-stu-id="3b047-165">String</span></span>|<span data-ttu-id="3b047-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3b047-166">The privacy statement Url.</span></span> <span data-ttu-id="3b047-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3b047-168">informationUrl</span></span>|<span data-ttu-id="3b047-169">String</span><span class="sxs-lookup"><span data-stu-id="3b047-169">String</span></span>|<span data-ttu-id="3b047-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3b047-170">The more information Url.</span></span> <span data-ttu-id="3b047-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-172">owner</span><span class="sxs-lookup"><span data-stu-id="3b047-172">owner</span></span>|<span data-ttu-id="3b047-173">String</span><span class="sxs-lookup"><span data-stu-id="3b047-173">String</span></span>|<span data-ttu-id="3b047-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="3b047-174">The owner of the app.</span></span> <span data-ttu-id="3b047-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-176">developer</span><span class="sxs-lookup"><span data-stu-id="3b047-176">developer</span></span>|<span data-ttu-id="3b047-177">String</span><span class="sxs-lookup"><span data-stu-id="3b047-177">String</span></span>|<span data-ttu-id="3b047-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="3b047-178">The developer of the app.</span></span> <span data-ttu-id="3b047-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-180">notes</span><span class="sxs-lookup"><span data-stu-id="3b047-180">notes</span></span>|<span data-ttu-id="3b047-181">String</span><span class="sxs-lookup"><span data-stu-id="3b047-181">String</span></span>|<span data-ttu-id="3b047-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="3b047-182">Notes for the app.</span></span> <span data-ttu-id="3b047-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="3b047-184">uploadState</span></span>|<span data-ttu-id="3b047-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3b047-185">Int32</span></span>|<span data-ttu-id="3b047-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="3b047-186">The upload state.</span></span> <span data-ttu-id="3b047-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="3b047-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="3b047-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="3b047-189">publishingState</span></span>|[<span data-ttu-id="3b047-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="3b047-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3b047-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="3b047-191">The publishing state for the app.</span></span> <span data-ttu-id="3b047-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="3b047-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3b047-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="3b047-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3b047-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3b047-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3b047-195">isAssigned</span></span>|<span data-ttu-id="3b047-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b047-196">Boolean</span></span>|<span data-ttu-id="3b047-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="3b047-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3b047-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3b047-199">roleScopeTagIds</span></span>|<span data-ttu-id="3b047-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3b047-200">String collection</span></span>|<span data-ttu-id="3b047-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="3b047-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3b047-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="3b047-203">dependentAppCount</span></span>|<span data-ttu-id="3b047-204">Int32</span><span class="sxs-lookup"><span data-stu-id="3b047-204">Int32</span></span>|<span data-ttu-id="3b047-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="3b047-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="3b047-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="3b047-207">supersedingAppCount</span></span>|<span data-ttu-id="3b047-208">Int32</span><span class="sxs-lookup"><span data-stu-id="3b047-208">Int32</span></span>|<span data-ttu-id="3b047-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="3b047-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="3b047-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="3b047-211">supersededAppCount</span></span>|<span data-ttu-id="3b047-212">Int32</span><span class="sxs-lookup"><span data-stu-id="3b047-212">Int32</span></span>|<span data-ttu-id="3b047-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="3b047-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="3b047-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b047-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3b047-215">packageId</span><span class="sxs-lookup"><span data-stu-id="3b047-215">packageId</span></span>|<span data-ttu-id="3b047-216">String</span><span class="sxs-lookup"><span data-stu-id="3b047-216">String</span></span>|<span data-ttu-id="3b047-217">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="3b047-217">The package identifier.</span></span>|
|<span data-ttu-id="3b047-218">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="3b047-218">appIdentifier</span></span>|<span data-ttu-id="3b047-219">String</span><span class="sxs-lookup"><span data-stu-id="3b047-219">String</span></span>|<span data-ttu-id="3b047-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3b047-220">The Identity Name.</span></span>|
|<span data-ttu-id="3b047-221">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3b047-221">appStoreUrl</span></span>|<span data-ttu-id="3b047-222">String</span><span class="sxs-lookup"><span data-stu-id="3b047-222">String</span></span>|<span data-ttu-id="3b047-223">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="3b047-223">The Android app store URL.</span></span>|
|<span data-ttu-id="3b047-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3b047-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3b047-225">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3b047-225">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="3b047-226">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="3b047-226">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="3b047-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b047-227">Response</span></span>
<span data-ttu-id="3b047-228">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3b047-228">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b047-229">Пример</span><span class="sxs-lookup"><span data-stu-id="3b047-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b047-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b047-230">Request</span></span>
<span data-ttu-id="3b047-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b047-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="3b047-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b047-232">Response</span></span>
<span data-ttu-id="3b047-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b047-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1459

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```




