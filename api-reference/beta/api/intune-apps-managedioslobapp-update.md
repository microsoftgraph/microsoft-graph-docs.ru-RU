---
title: Update managedIOSLobApp
description: Обновление свойств объекта managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2fbf159f0b9b8acc65218ce60263cb2e277001d0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143523"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="ae853-103">Update managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="ae853-103">Update managedIOSLobApp</span></span>

<span data-ttu-id="ae853-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae853-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae853-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae853-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae853-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae853-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae853-107">Обновление свойств объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae853-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ae853-108">Prerequisites</span></span>
<span data-ttu-id="ae853-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae853-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae853-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae853-111">Permission type</span></span>|<span data-ttu-id="ae853-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae853-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae853-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae853-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae853-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae853-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ae853-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae853-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae853-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae853-116">Not supported.</span></span>|
|<span data-ttu-id="ae853-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ae853-117">Application</span></span>|<span data-ttu-id="ae853-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae853-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae853-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae853-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ae853-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ae853-120">Request headers</span></span>
|<span data-ttu-id="ae853-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae853-121">Header</span></span>|<span data-ttu-id="ae853-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ae853-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae853-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae853-123">Authorization</span></span>|<span data-ttu-id="ae853-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae853-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae853-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ae853-125">Accept</span></span>|<span data-ttu-id="ae853-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae853-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae853-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae853-127">Request body</span></span>
<span data-ttu-id="ae853-128">В теле запроса добавьте представление объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae853-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="ae853-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="ae853-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae853-130">Property</span></span>|<span data-ttu-id="ae853-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ae853-131">Type</span></span>|<span data-ttu-id="ae853-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ae853-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae853-133">id</span><span class="sxs-lookup"><span data-stu-id="ae853-133">id</span></span>|<span data-ttu-id="ae853-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ae853-134">String</span></span>|<span data-ttu-id="ae853-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ae853-135">Key of the entity.</span></span> <span data-ttu-id="ae853-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ae853-137">displayName</span></span>|<span data-ttu-id="ae853-138">Строка</span><span class="sxs-lookup"><span data-stu-id="ae853-138">String</span></span>|<span data-ttu-id="ae853-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ae853-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ae853-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-141">description</span><span class="sxs-lookup"><span data-stu-id="ae853-141">description</span></span>|<span data-ttu-id="ae853-142">Строка</span><span class="sxs-lookup"><span data-stu-id="ae853-142">String</span></span>|<span data-ttu-id="ae853-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ae853-143">The description of the app.</span></span> <span data-ttu-id="ae853-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ae853-145">publisher</span></span>|<span data-ttu-id="ae853-146">String</span><span class="sxs-lookup"><span data-stu-id="ae853-146">String</span></span>|<span data-ttu-id="ae853-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ae853-147">The publisher of the app.</span></span> <span data-ttu-id="ae853-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ae853-149">largeIcon</span></span>|[<span data-ttu-id="ae853-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ae853-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ae853-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ae853-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ae853-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae853-153">createdDateTime</span></span>|<span data-ttu-id="ae853-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae853-154">DateTimeOffset</span></span>|<span data-ttu-id="ae853-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ae853-155">The date and time the app was created.</span></span> <span data-ttu-id="ae853-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae853-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ae853-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae853-158">DateTimeOffset</span></span>|<span data-ttu-id="ae853-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ae853-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ae853-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ae853-161">isFeatured</span></span>|<span data-ttu-id="ae853-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae853-162">Boolean</span></span>|<span data-ttu-id="ae853-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ae853-164">privacyInformationUrl</span></span>|<span data-ttu-id="ae853-165">String</span><span class="sxs-lookup"><span data-stu-id="ae853-165">String</span></span>|<span data-ttu-id="ae853-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ae853-166">The privacy statement Url.</span></span> <span data-ttu-id="ae853-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ae853-168">informationUrl</span></span>|<span data-ttu-id="ae853-169">String</span><span class="sxs-lookup"><span data-stu-id="ae853-169">String</span></span>|<span data-ttu-id="ae853-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ae853-170">The more information Url.</span></span> <span data-ttu-id="ae853-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-172">owner</span><span class="sxs-lookup"><span data-stu-id="ae853-172">owner</span></span>|<span data-ttu-id="ae853-173">String</span><span class="sxs-lookup"><span data-stu-id="ae853-173">String</span></span>|<span data-ttu-id="ae853-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ae853-174">The owner of the app.</span></span> <span data-ttu-id="ae853-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-176">developer</span><span class="sxs-lookup"><span data-stu-id="ae853-176">developer</span></span>|<span data-ttu-id="ae853-177">String</span><span class="sxs-lookup"><span data-stu-id="ae853-177">String</span></span>|<span data-ttu-id="ae853-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ae853-178">The developer of the app.</span></span> <span data-ttu-id="ae853-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-180">notes</span><span class="sxs-lookup"><span data-stu-id="ae853-180">notes</span></span>|<span data-ttu-id="ae853-181">String</span><span class="sxs-lookup"><span data-stu-id="ae853-181">String</span></span>|<span data-ttu-id="ae853-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ae853-182">Notes for the app.</span></span> <span data-ttu-id="ae853-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ae853-184">uploadState</span></span>|<span data-ttu-id="ae853-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ae853-185">Int32</span></span>|<span data-ttu-id="ae853-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="ae853-186">The upload state.</span></span> <span data-ttu-id="ae853-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="ae853-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ae853-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ae853-189">publishingState</span></span>|[<span data-ttu-id="ae853-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ae853-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ae853-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ae853-191">The publishing state for the app.</span></span> <span data-ttu-id="ae853-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ae853-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ae853-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ae853-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ae853-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ae853-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ae853-195">isAssigned</span></span>|<span data-ttu-id="ae853-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae853-196">Boolean</span></span>|<span data-ttu-id="ae853-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="ae853-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ae853-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ae853-199">roleScopeTagIds</span></span>|<span data-ttu-id="ae853-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ae853-200">String collection</span></span>|<span data-ttu-id="ae853-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ae853-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ae853-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ae853-203">dependentAppCount</span></span>|<span data-ttu-id="ae853-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ae853-204">Int32</span></span>|<span data-ttu-id="ae853-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="ae853-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ae853-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="ae853-207">supersedingAppCount</span></span>|<span data-ttu-id="ae853-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ae853-208">Int32</span></span>|<span data-ttu-id="ae853-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="ae853-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="ae853-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="ae853-211">supersededAppCount</span></span>|<span data-ttu-id="ae853-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ae853-212">Int32</span></span>|<span data-ttu-id="ae853-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="ae853-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="ae853-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ae853-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="ae853-215">appAvailability</span></span>|[<span data-ttu-id="ae853-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="ae853-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="ae853-217">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="ae853-217">The Application's availability.</span></span> <span data-ttu-id="ae853-218">Унаследованный от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="ae853-219">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="ae853-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="ae853-220">version</span><span class="sxs-lookup"><span data-stu-id="ae853-220">version</span></span>|<span data-ttu-id="ae853-221">String</span><span class="sxs-lookup"><span data-stu-id="ae853-221">String</span></span>|<span data-ttu-id="ae853-222">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="ae853-222">The Application's version.</span></span> <span data-ttu-id="ae853-223">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="ae853-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ae853-224">committedContentVersion</span></span>|<span data-ttu-id="ae853-225">String</span><span class="sxs-lookup"><span data-stu-id="ae853-225">String</span></span>|<span data-ttu-id="ae853-226">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="ae853-226">The internal committed content version.</span></span> <span data-ttu-id="ae853-227">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ae853-228">fileName</span><span class="sxs-lookup"><span data-stu-id="ae853-228">fileName</span></span>|<span data-ttu-id="ae853-229">String</span><span class="sxs-lookup"><span data-stu-id="ae853-229">String</span></span>|<span data-ttu-id="ae853-230">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ae853-230">The name of the main Lob application file.</span></span> <span data-ttu-id="ae853-231">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ae853-232">size</span><span class="sxs-lookup"><span data-stu-id="ae853-232">size</span></span>|<span data-ttu-id="ae853-233">Int64</span><span class="sxs-lookup"><span data-stu-id="ae853-233">Int64</span></span>|<span data-ttu-id="ae853-234">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="ae853-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="ae853-235">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ae853-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ae853-236">bundleId</span><span class="sxs-lookup"><span data-stu-id="ae853-236">bundleId</span></span>|<span data-ttu-id="ae853-237">String</span><span class="sxs-lookup"><span data-stu-id="ae853-237">String</span></span>|<span data-ttu-id="ae853-238">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ae853-238">The Identity Name.</span></span>|
|<span data-ttu-id="ae853-239">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ae853-239">applicableDeviceType</span></span>|[<span data-ttu-id="ae853-240">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ae853-240">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="ae853-241">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ae853-241">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="ae853-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ae853-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ae853-243">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ae853-243">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="ae853-244">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ae853-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ae853-245">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ae853-245">expirationDateTime</span></span>|<span data-ttu-id="ae853-246">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae853-246">DateTimeOffset</span></span>|<span data-ttu-id="ae853-247">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="ae853-247">The expiration time.</span></span>|
|<span data-ttu-id="ae853-248">versionNumber</span><span class="sxs-lookup"><span data-stu-id="ae853-248">versionNumber</span></span>|<span data-ttu-id="ae853-249">String</span><span class="sxs-lookup"><span data-stu-id="ae853-249">String</span></span>|<span data-ttu-id="ae853-250">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="ae853-250">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ae853-251">buildNumber</span><span class="sxs-lookup"><span data-stu-id="ae853-251">buildNumber</span></span>|<span data-ttu-id="ae853-252">String</span><span class="sxs-lookup"><span data-stu-id="ae853-252">String</span></span>|<span data-ttu-id="ae853-253">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="ae853-253">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ae853-254">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ae853-254">identityVersion</span></span>|<span data-ttu-id="ae853-255">String</span><span class="sxs-lookup"><span data-stu-id="ae853-255">String</span></span>|<span data-ttu-id="ae853-256">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ae853-256">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ae853-257">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae853-257">Response</span></span>
<span data-ttu-id="ae853-258">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ae853-258">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae853-259">Пример</span><span class="sxs-lookup"><span data-stu-id="ae853-259">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae853-260">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae853-260">Request</span></span>
<span data-ttu-id="ae853-261">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae853-261">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1566

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="ae853-262">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae853-262">Response</span></span>
<span data-ttu-id="ae853-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae853-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1738

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




