---
title: Update microsoftStoreForBusinessApp
description: Обновление свойств объекта microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b3c10a1e094d5cde2250066da65879352a8fca9a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143439"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="193ee-103">Update microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="193ee-103">Update microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="193ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="193ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="193ee-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="193ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="193ee-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="193ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="193ee-107">Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-107">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="193ee-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="193ee-108">Prerequisites</span></span>
<span data-ttu-id="193ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="193ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="193ee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="193ee-111">Permission type</span></span>|<span data-ttu-id="193ee-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="193ee-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="193ee-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="193ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="193ee-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="193ee-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="193ee-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="193ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="193ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="193ee-116">Not supported.</span></span>|
|<span data-ttu-id="193ee-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="193ee-117">Application</span></span>|<span data-ttu-id="193ee-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="193ee-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="193ee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="193ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="193ee-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="193ee-120">Request headers</span></span>
|<span data-ttu-id="193ee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="193ee-121">Header</span></span>|<span data-ttu-id="193ee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="193ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="193ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="193ee-123">Authorization</span></span>|<span data-ttu-id="193ee-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="193ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="193ee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="193ee-125">Accept</span></span>|<span data-ttu-id="193ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="193ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="193ee-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="193ee-127">Request body</span></span>
<span data-ttu-id="193ee-128">В теле запроса добавьте представление объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="193ee-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="193ee-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="193ee-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="193ee-130">Property</span></span>|<span data-ttu-id="193ee-131">Тип</span><span class="sxs-lookup"><span data-stu-id="193ee-131">Type</span></span>|<span data-ttu-id="193ee-132">Описание</span><span class="sxs-lookup"><span data-stu-id="193ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="193ee-133">id</span><span class="sxs-lookup"><span data-stu-id="193ee-133">id</span></span>|<span data-ttu-id="193ee-134">Строка</span><span class="sxs-lookup"><span data-stu-id="193ee-134">String</span></span>|<span data-ttu-id="193ee-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="193ee-135">Key of the entity.</span></span> <span data-ttu-id="193ee-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-137">displayName</span><span class="sxs-lookup"><span data-stu-id="193ee-137">displayName</span></span>|<span data-ttu-id="193ee-138">Строка</span><span class="sxs-lookup"><span data-stu-id="193ee-138">String</span></span>|<span data-ttu-id="193ee-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="193ee-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="193ee-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-141">description</span><span class="sxs-lookup"><span data-stu-id="193ee-141">description</span></span>|<span data-ttu-id="193ee-142">Строка</span><span class="sxs-lookup"><span data-stu-id="193ee-142">String</span></span>|<span data-ttu-id="193ee-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="193ee-143">The description of the app.</span></span> <span data-ttu-id="193ee-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-145">publisher</span><span class="sxs-lookup"><span data-stu-id="193ee-145">publisher</span></span>|<span data-ttu-id="193ee-146">String</span><span class="sxs-lookup"><span data-stu-id="193ee-146">String</span></span>|<span data-ttu-id="193ee-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="193ee-147">The publisher of the app.</span></span> <span data-ttu-id="193ee-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="193ee-149">largeIcon</span></span>|[<span data-ttu-id="193ee-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="193ee-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="193ee-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="193ee-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="193ee-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="193ee-153">createdDateTime</span></span>|<span data-ttu-id="193ee-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="193ee-154">DateTimeOffset</span></span>|<span data-ttu-id="193ee-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="193ee-155">The date and time the app was created.</span></span> <span data-ttu-id="193ee-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="193ee-157">lastModifiedDateTime</span></span>|<span data-ttu-id="193ee-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="193ee-158">DateTimeOffset</span></span>|<span data-ttu-id="193ee-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="193ee-159">The date and time the app was last modified.</span></span> <span data-ttu-id="193ee-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="193ee-161">isFeatured</span></span>|<span data-ttu-id="193ee-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="193ee-162">Boolean</span></span>|<span data-ttu-id="193ee-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="193ee-164">privacyInformationUrl</span></span>|<span data-ttu-id="193ee-165">String</span><span class="sxs-lookup"><span data-stu-id="193ee-165">String</span></span>|<span data-ttu-id="193ee-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="193ee-166">The privacy statement Url.</span></span> <span data-ttu-id="193ee-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="193ee-168">informationUrl</span></span>|<span data-ttu-id="193ee-169">String</span><span class="sxs-lookup"><span data-stu-id="193ee-169">String</span></span>|<span data-ttu-id="193ee-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="193ee-170">The more information Url.</span></span> <span data-ttu-id="193ee-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-172">owner</span><span class="sxs-lookup"><span data-stu-id="193ee-172">owner</span></span>|<span data-ttu-id="193ee-173">String</span><span class="sxs-lookup"><span data-stu-id="193ee-173">String</span></span>|<span data-ttu-id="193ee-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="193ee-174">The owner of the app.</span></span> <span data-ttu-id="193ee-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-176">developer</span><span class="sxs-lookup"><span data-stu-id="193ee-176">developer</span></span>|<span data-ttu-id="193ee-177">String</span><span class="sxs-lookup"><span data-stu-id="193ee-177">String</span></span>|<span data-ttu-id="193ee-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="193ee-178">The developer of the app.</span></span> <span data-ttu-id="193ee-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-180">notes</span><span class="sxs-lookup"><span data-stu-id="193ee-180">notes</span></span>|<span data-ttu-id="193ee-181">String</span><span class="sxs-lookup"><span data-stu-id="193ee-181">String</span></span>|<span data-ttu-id="193ee-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="193ee-182">Notes for the app.</span></span> <span data-ttu-id="193ee-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="193ee-184">uploadState</span></span>|<span data-ttu-id="193ee-185">Int32</span><span class="sxs-lookup"><span data-stu-id="193ee-185">Int32</span></span>|<span data-ttu-id="193ee-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="193ee-186">The upload state.</span></span> <span data-ttu-id="193ee-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="193ee-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="193ee-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="193ee-189">publishingState</span></span>|[<span data-ttu-id="193ee-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="193ee-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="193ee-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="193ee-191">The publishing state for the app.</span></span> <span data-ttu-id="193ee-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="193ee-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="193ee-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="193ee-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="193ee-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="193ee-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="193ee-195">isAssigned</span></span>|<span data-ttu-id="193ee-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="193ee-196">Boolean</span></span>|<span data-ttu-id="193ee-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="193ee-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="193ee-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="193ee-199">roleScopeTagIds</span></span>|<span data-ttu-id="193ee-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="193ee-200">String collection</span></span>|<span data-ttu-id="193ee-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="193ee-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="193ee-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="193ee-203">dependentAppCount</span></span>|<span data-ttu-id="193ee-204">Int32</span><span class="sxs-lookup"><span data-stu-id="193ee-204">Int32</span></span>|<span data-ttu-id="193ee-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="193ee-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="193ee-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="193ee-207">supersedingAppCount</span></span>|<span data-ttu-id="193ee-208">Int32</span><span class="sxs-lookup"><span data-stu-id="193ee-208">Int32</span></span>|<span data-ttu-id="193ee-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="193ee-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="193ee-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="193ee-211">supersededAppCount</span></span>|<span data-ttu-id="193ee-212">Int32</span><span class="sxs-lookup"><span data-stu-id="193ee-212">Int32</span></span>|<span data-ttu-id="193ee-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="193ee-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="193ee-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="193ee-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="193ee-215">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="193ee-215">usedLicenseCount</span></span>|<span data-ttu-id="193ee-216">Int32</span><span class="sxs-lookup"><span data-stu-id="193ee-216">Int32</span></span>|<span data-ttu-id="193ee-217">Количество используемых лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="193ee-217">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="193ee-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="193ee-218">totalLicenseCount</span></span>|<span data-ttu-id="193ee-219">Int32</span><span class="sxs-lookup"><span data-stu-id="193ee-219">Int32</span></span>|<span data-ttu-id="193ee-220">Общее количество лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="193ee-220">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="193ee-221">productKey</span><span class="sxs-lookup"><span data-stu-id="193ee-221">productKey</span></span>|<span data-ttu-id="193ee-222">String</span><span class="sxs-lookup"><span data-stu-id="193ee-222">String</span></span>|<span data-ttu-id="193ee-223">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="193ee-223">The app product key</span></span>|
|<span data-ttu-id="193ee-224">licenseType</span><span class="sxs-lookup"><span data-stu-id="193ee-224">licenseType</span></span>|[<span data-ttu-id="193ee-225">MicrosoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="193ee-225">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="193ee-226">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="193ee-226">The app license type.</span></span> <span data-ttu-id="193ee-227">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="193ee-227">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="193ee-228">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="193ee-228">packageIdentityName</span></span>|<span data-ttu-id="193ee-229">String</span><span class="sxs-lookup"><span data-stu-id="193ee-229">String</span></span>|<span data-ttu-id="193ee-230">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="193ee-230">The app package identifier</span></span>|
|<span data-ttu-id="193ee-231">licensingType</span><span class="sxs-lookup"><span data-stu-id="193ee-231">licensingType</span></span>|[<span data-ttu-id="193ee-232">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="193ee-232">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="193ee-233">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="193ee-233">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="193ee-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="193ee-234">Response</span></span>
<span data-ttu-id="193ee-235">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="193ee-235">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="193ee-236">Пример</span><span class="sxs-lookup"><span data-stu-id="193ee-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="193ee-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="193ee-237">Request</span></span>
<span data-ttu-id="193ee-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="193ee-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```

### <a name="response"></a><span data-ttu-id="193ee-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="193ee-239">Response</span></span>
<span data-ttu-id="193ee-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="193ee-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```




