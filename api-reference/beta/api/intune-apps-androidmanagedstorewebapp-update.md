---
title: Обновление AndroidManagedStoreWebApp
description: Обновление свойств объекта AndroidManagedStoreWebApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11a011e018211d706f0dd340ac5a32137f2ea55f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144370"
---
# <a name="update-androidmanagedstorewebapp"></a><span data-ttu-id="8a998-103">Обновление AndroidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="8a998-103">Update androidManagedStoreWebApp</span></span>

<span data-ttu-id="8a998-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a998-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a998-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a998-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a998-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a998-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a998-107">Обновление свойств объекта [AndroidManagedStoreWebApp.](../resources/intune-apps-androidmanagedstorewebapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-107">Update the properties of a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a998-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8a998-108">Prerequisites</span></span>
<span data-ttu-id="8a998-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a998-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a998-111">Permission type</span></span>|<span data-ttu-id="8a998-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a998-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a998-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a998-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a998-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a998-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8a998-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a998-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a998-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a998-116">Not supported.</span></span>|
|<span data-ttu-id="8a998-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8a998-117">Application</span></span>|<span data-ttu-id="8a998-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a998-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a998-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a998-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8a998-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8a998-120">Request headers</span></span>
|<span data-ttu-id="8a998-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a998-121">Header</span></span>|<span data-ttu-id="8a998-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8a998-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a998-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a998-123">Authorization</span></span>|<span data-ttu-id="8a998-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a998-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a998-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8a998-125">Accept</span></span>|<span data-ttu-id="8a998-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a998-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a998-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a998-127">Request body</span></span>
<span data-ttu-id="8a998-128">В теле запроса поставляем представление JSON для [объекта AndroidManagedStoreWebApp.](../resources/intune-apps-androidmanagedstorewebapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-128">In the request body, supply a JSON representation for the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

<span data-ttu-id="8a998-129">В следующей таблице показаны свойства, необходимые при создании [androidManagedStoreWebApp.](../resources/intune-apps-androidmanagedstorewebapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-129">The following table shows the properties that are required when you create the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span></span>

|<span data-ttu-id="8a998-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a998-130">Property</span></span>|<span data-ttu-id="8a998-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8a998-131">Type</span></span>|<span data-ttu-id="8a998-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8a998-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a998-133">id</span><span class="sxs-lookup"><span data-stu-id="8a998-133">id</span></span>|<span data-ttu-id="8a998-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8a998-134">String</span></span>|<span data-ttu-id="8a998-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8a998-135">Key of the entity.</span></span> <span data-ttu-id="8a998-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8a998-137">displayName</span></span>|<span data-ttu-id="8a998-138">Строка</span><span class="sxs-lookup"><span data-stu-id="8a998-138">String</span></span>|<span data-ttu-id="8a998-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="8a998-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8a998-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-141">description</span><span class="sxs-lookup"><span data-stu-id="8a998-141">description</span></span>|<span data-ttu-id="8a998-142">Строка</span><span class="sxs-lookup"><span data-stu-id="8a998-142">String</span></span>|<span data-ttu-id="8a998-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="8a998-143">The description of the app.</span></span> <span data-ttu-id="8a998-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8a998-145">publisher</span></span>|<span data-ttu-id="8a998-146">String</span><span class="sxs-lookup"><span data-stu-id="8a998-146">String</span></span>|<span data-ttu-id="8a998-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="8a998-147">The publisher of the app.</span></span> <span data-ttu-id="8a998-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8a998-149">largeIcon</span></span>|[<span data-ttu-id="8a998-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8a998-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8a998-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="8a998-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8a998-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a998-153">createdDateTime</span></span>|<span data-ttu-id="8a998-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a998-154">DateTimeOffset</span></span>|<span data-ttu-id="8a998-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="8a998-155">The date and time the app was created.</span></span> <span data-ttu-id="8a998-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a998-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8a998-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a998-158">DateTimeOffset</span></span>|<span data-ttu-id="8a998-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="8a998-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8a998-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8a998-161">isFeatured</span></span>|<span data-ttu-id="8a998-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a998-162">Boolean</span></span>|<span data-ttu-id="8a998-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8a998-164">privacyInformationUrl</span></span>|<span data-ttu-id="8a998-165">String</span><span class="sxs-lookup"><span data-stu-id="8a998-165">String</span></span>|<span data-ttu-id="8a998-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8a998-166">The privacy statement Url.</span></span> <span data-ttu-id="8a998-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8a998-168">informationUrl</span></span>|<span data-ttu-id="8a998-169">String</span><span class="sxs-lookup"><span data-stu-id="8a998-169">String</span></span>|<span data-ttu-id="8a998-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="8a998-170">The more information Url.</span></span> <span data-ttu-id="8a998-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-172">owner</span><span class="sxs-lookup"><span data-stu-id="8a998-172">owner</span></span>|<span data-ttu-id="8a998-173">String</span><span class="sxs-lookup"><span data-stu-id="8a998-173">String</span></span>|<span data-ttu-id="8a998-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="8a998-174">The owner of the app.</span></span> <span data-ttu-id="8a998-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-176">developer</span><span class="sxs-lookup"><span data-stu-id="8a998-176">developer</span></span>|<span data-ttu-id="8a998-177">String</span><span class="sxs-lookup"><span data-stu-id="8a998-177">String</span></span>|<span data-ttu-id="8a998-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="8a998-178">The developer of the app.</span></span> <span data-ttu-id="8a998-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-180">notes</span><span class="sxs-lookup"><span data-stu-id="8a998-180">notes</span></span>|<span data-ttu-id="8a998-181">String</span><span class="sxs-lookup"><span data-stu-id="8a998-181">String</span></span>|<span data-ttu-id="8a998-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="8a998-182">Notes for the app.</span></span> <span data-ttu-id="8a998-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8a998-184">uploadState</span></span>|<span data-ttu-id="8a998-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8a998-185">Int32</span></span>|<span data-ttu-id="8a998-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="8a998-186">The upload state.</span></span> <span data-ttu-id="8a998-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="8a998-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="8a998-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="8a998-189">publishingState</span></span>|[<span data-ttu-id="8a998-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8a998-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8a998-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="8a998-191">The publishing state for the app.</span></span> <span data-ttu-id="8a998-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="8a998-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8a998-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8a998-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8a998-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8a998-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8a998-195">isAssigned</span></span>|<span data-ttu-id="8a998-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a998-196">Boolean</span></span>|<span data-ttu-id="8a998-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="8a998-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8a998-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8a998-199">roleScopeTagIds</span></span>|<span data-ttu-id="8a998-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8a998-200">String collection</span></span>|<span data-ttu-id="8a998-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="8a998-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8a998-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="8a998-203">dependentAppCount</span></span>|<span data-ttu-id="8a998-204">Int32</span><span class="sxs-lookup"><span data-stu-id="8a998-204">Int32</span></span>|<span data-ttu-id="8a998-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="8a998-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8a998-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="8a998-207">supersedingAppCount</span></span>|<span data-ttu-id="8a998-208">Int32</span><span class="sxs-lookup"><span data-stu-id="8a998-208">Int32</span></span>|<span data-ttu-id="8a998-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="8a998-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="8a998-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="8a998-211">supersededAppCount</span></span>|<span data-ttu-id="8a998-212">Int32</span><span class="sxs-lookup"><span data-stu-id="8a998-212">Int32</span></span>|<span data-ttu-id="8a998-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="8a998-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="8a998-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8a998-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8a998-215">packageId</span><span class="sxs-lookup"><span data-stu-id="8a998-215">packageId</span></span>|<span data-ttu-id="8a998-216">String</span><span class="sxs-lookup"><span data-stu-id="8a998-216">String</span></span>|<span data-ttu-id="8a998-217">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="8a998-217">The package identifier.</span></span> <span data-ttu-id="8a998-218">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-218">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="8a998-219">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="8a998-219">appIdentifier</span></span>|<span data-ttu-id="8a998-220">String</span><span class="sxs-lookup"><span data-stu-id="8a998-220">String</span></span>|<span data-ttu-id="8a998-221">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="8a998-221">The Identity Name.</span></span> <span data-ttu-id="8a998-222">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-222">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="8a998-223">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8a998-223">usedLicenseCount</span></span>|<span data-ttu-id="8a998-224">Int32</span><span class="sxs-lookup"><span data-stu-id="8a998-224">Int32</span></span>|<span data-ttu-id="8a998-225">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="8a998-225">The number of VPP licenses in use.</span></span> <span data-ttu-id="8a998-226">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-226">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="8a998-227">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8a998-227">totalLicenseCount</span></span>|<span data-ttu-id="8a998-228">Int32</span><span class="sxs-lookup"><span data-stu-id="8a998-228">Int32</span></span>|<span data-ttu-id="8a998-229">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="8a998-229">The total number of VPP licenses.</span></span> <span data-ttu-id="8a998-230">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-230">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="8a998-231">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8a998-231">appStoreUrl</span></span>|<span data-ttu-id="8a998-232">String</span><span class="sxs-lookup"><span data-stu-id="8a998-232">String</span></span>|<span data-ttu-id="8a998-233">URL-адрес приложения Play for Work Store.</span><span class="sxs-lookup"><span data-stu-id="8a998-233">The Play for Work Store app URL.</span></span> <span data-ttu-id="8a998-234">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-234">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="8a998-235">isPrivate</span><span class="sxs-lookup"><span data-stu-id="8a998-235">isPrivate</span></span>|<span data-ttu-id="8a998-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a998-236">Boolean</span></span>|<span data-ttu-id="8a998-237">Указывает, доступно ли приложение только пользователям данного предприятия.</span><span class="sxs-lookup"><span data-stu-id="8a998-237">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="8a998-238">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-238">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="8a998-239">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="8a998-239">isSystemApp</span></span>|<span data-ttu-id="8a998-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a998-240">Boolean</span></span>|<span data-ttu-id="8a998-241">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="8a998-241">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="8a998-242">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-242">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="8a998-243">appTracks</span><span class="sxs-lookup"><span data-stu-id="8a998-243">appTracks</span></span>|<span data-ttu-id="8a998-244">[коллекция AndroidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-244">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="8a998-245">Отслеживает, которые видны этому предприятию.</span><span class="sxs-lookup"><span data-stu-id="8a998-245">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="8a998-246">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-246">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="8a998-247">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="8a998-247">supportsOemConfig</span></span>|<span data-ttu-id="8a998-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a998-248">Boolean</span></span>|<span data-ttu-id="8a998-249">Поддерживает ли это приложение политику OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="8a998-249">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="8a998-250">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="8a998-250">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8a998-251">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a998-251">Response</span></span>
<span data-ttu-id="8a998-252">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8a998-252">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a998-253">Пример</span><span class="sxs-lookup"><span data-stu-id="8a998-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a998-254">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a998-254">Request</span></span>
<span data-ttu-id="8a998-255">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a998-255">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1228

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="8a998-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a998-256">Response</span></span>
<span data-ttu-id="8a998-p130">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a998-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1400

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
  "id": "e54aecbd-ecbd-e54a-bdec-4ae5bdec4ae5",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```




