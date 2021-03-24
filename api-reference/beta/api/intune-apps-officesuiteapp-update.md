---
title: Обновление officeSuiteApp
description: Обновление свойств объекта officeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e121543f821620271ed0eb2731b4b9406b5c25f5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139407"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="90c98-103">Обновление officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="90c98-103">Update officeSuiteApp</span></span>

<span data-ttu-id="90c98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90c98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90c98-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90c98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90c98-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90c98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90c98-107">Обновление свойств объекта [officeSuiteApp.](../resources/intune-apps-officesuiteapp.md)</span><span class="sxs-lookup"><span data-stu-id="90c98-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90c98-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="90c98-108">Prerequisites</span></span>
<span data-ttu-id="90c98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90c98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90c98-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90c98-111">Permission type</span></span>|<span data-ttu-id="90c98-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90c98-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90c98-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90c98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90c98-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90c98-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="90c98-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90c98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90c98-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90c98-116">Not supported.</span></span>|
|<span data-ttu-id="90c98-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="90c98-117">Application</span></span>|<span data-ttu-id="90c98-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90c98-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90c98-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90c98-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="90c98-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="90c98-120">Request headers</span></span>
|<span data-ttu-id="90c98-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90c98-121">Header</span></span>|<span data-ttu-id="90c98-122">Значение</span><span class="sxs-lookup"><span data-stu-id="90c98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90c98-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90c98-123">Authorization</span></span>|<span data-ttu-id="90c98-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90c98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90c98-125">Accept</span><span class="sxs-lookup"><span data-stu-id="90c98-125">Accept</span></span>|<span data-ttu-id="90c98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90c98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90c98-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90c98-127">Request body</span></span>
<span data-ttu-id="90c98-128">В теле запроса поставляем представление JSON для [объекта officeSuiteApp.](../resources/intune-apps-officesuiteapp.md)</span><span class="sxs-lookup"><span data-stu-id="90c98-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="90c98-129">В следующей таблице показаны свойства, необходимые при создании [officeSuiteApp.](../resources/intune-apps-officesuiteapp.md)</span><span class="sxs-lookup"><span data-stu-id="90c98-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="90c98-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="90c98-130">Property</span></span>|<span data-ttu-id="90c98-131">Тип</span><span class="sxs-lookup"><span data-stu-id="90c98-131">Type</span></span>|<span data-ttu-id="90c98-132">Описание</span><span class="sxs-lookup"><span data-stu-id="90c98-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90c98-133">id</span><span class="sxs-lookup"><span data-stu-id="90c98-133">id</span></span>|<span data-ttu-id="90c98-134">Строка</span><span class="sxs-lookup"><span data-stu-id="90c98-134">String</span></span>|<span data-ttu-id="90c98-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="90c98-135">Key of the entity.</span></span> <span data-ttu-id="90c98-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-137">displayName</span><span class="sxs-lookup"><span data-stu-id="90c98-137">displayName</span></span>|<span data-ttu-id="90c98-138">Строка</span><span class="sxs-lookup"><span data-stu-id="90c98-138">String</span></span>|<span data-ttu-id="90c98-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="90c98-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="90c98-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-141">description</span><span class="sxs-lookup"><span data-stu-id="90c98-141">description</span></span>|<span data-ttu-id="90c98-142">Строка</span><span class="sxs-lookup"><span data-stu-id="90c98-142">String</span></span>|<span data-ttu-id="90c98-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="90c98-143">The description of the app.</span></span> <span data-ttu-id="90c98-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-145">publisher</span><span class="sxs-lookup"><span data-stu-id="90c98-145">publisher</span></span>|<span data-ttu-id="90c98-146">String</span><span class="sxs-lookup"><span data-stu-id="90c98-146">String</span></span>|<span data-ttu-id="90c98-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="90c98-147">The publisher of the app.</span></span> <span data-ttu-id="90c98-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="90c98-149">largeIcon</span></span>|[<span data-ttu-id="90c98-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="90c98-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="90c98-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="90c98-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="90c98-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90c98-153">createdDateTime</span></span>|<span data-ttu-id="90c98-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90c98-154">DateTimeOffset</span></span>|<span data-ttu-id="90c98-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="90c98-155">The date and time the app was created.</span></span> <span data-ttu-id="90c98-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90c98-157">lastModifiedDateTime</span></span>|<span data-ttu-id="90c98-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90c98-158">DateTimeOffset</span></span>|<span data-ttu-id="90c98-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="90c98-159">The date and time the app was last modified.</span></span> <span data-ttu-id="90c98-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="90c98-161">isFeatured</span></span>|<span data-ttu-id="90c98-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="90c98-162">Boolean</span></span>|<span data-ttu-id="90c98-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="90c98-164">privacyInformationUrl</span></span>|<span data-ttu-id="90c98-165">String</span><span class="sxs-lookup"><span data-stu-id="90c98-165">String</span></span>|<span data-ttu-id="90c98-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="90c98-166">The privacy statement Url.</span></span> <span data-ttu-id="90c98-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="90c98-168">informationUrl</span></span>|<span data-ttu-id="90c98-169">String</span><span class="sxs-lookup"><span data-stu-id="90c98-169">String</span></span>|<span data-ttu-id="90c98-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="90c98-170">The more information Url.</span></span> <span data-ttu-id="90c98-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-172">owner</span><span class="sxs-lookup"><span data-stu-id="90c98-172">owner</span></span>|<span data-ttu-id="90c98-173">String</span><span class="sxs-lookup"><span data-stu-id="90c98-173">String</span></span>|<span data-ttu-id="90c98-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="90c98-174">The owner of the app.</span></span> <span data-ttu-id="90c98-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-176">developer</span><span class="sxs-lookup"><span data-stu-id="90c98-176">developer</span></span>|<span data-ttu-id="90c98-177">String</span><span class="sxs-lookup"><span data-stu-id="90c98-177">String</span></span>|<span data-ttu-id="90c98-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="90c98-178">The developer of the app.</span></span> <span data-ttu-id="90c98-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-180">notes</span><span class="sxs-lookup"><span data-stu-id="90c98-180">notes</span></span>|<span data-ttu-id="90c98-181">String</span><span class="sxs-lookup"><span data-stu-id="90c98-181">String</span></span>|<span data-ttu-id="90c98-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="90c98-182">Notes for the app.</span></span> <span data-ttu-id="90c98-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="90c98-184">uploadState</span></span>|<span data-ttu-id="90c98-185">Int32</span><span class="sxs-lookup"><span data-stu-id="90c98-185">Int32</span></span>|<span data-ttu-id="90c98-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="90c98-186">The upload state.</span></span> <span data-ttu-id="90c98-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="90c98-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="90c98-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="90c98-189">publishingState</span></span>|[<span data-ttu-id="90c98-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="90c98-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="90c98-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="90c98-191">The publishing state for the app.</span></span> <span data-ttu-id="90c98-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="90c98-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="90c98-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="90c98-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="90c98-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="90c98-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="90c98-195">isAssigned</span></span>|<span data-ttu-id="90c98-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="90c98-196">Boolean</span></span>|<span data-ttu-id="90c98-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="90c98-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="90c98-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="90c98-199">roleScopeTagIds</span></span>|<span data-ttu-id="90c98-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="90c98-200">String collection</span></span>|<span data-ttu-id="90c98-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="90c98-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="90c98-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="90c98-203">dependentAppCount</span></span>|<span data-ttu-id="90c98-204">Int32</span><span class="sxs-lookup"><span data-stu-id="90c98-204">Int32</span></span>|<span data-ttu-id="90c98-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="90c98-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="90c98-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="90c98-207">supersedingAppCount</span></span>|<span data-ttu-id="90c98-208">Int32</span><span class="sxs-lookup"><span data-stu-id="90c98-208">Int32</span></span>|<span data-ttu-id="90c98-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="90c98-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="90c98-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="90c98-211">supersededAppCount</span></span>|<span data-ttu-id="90c98-212">Int32</span><span class="sxs-lookup"><span data-stu-id="90c98-212">Int32</span></span>|<span data-ttu-id="90c98-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="90c98-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="90c98-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="90c98-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="90c98-215">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="90c98-215">autoAcceptEula</span></span>|<span data-ttu-id="90c98-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="90c98-216">Boolean</span></span>|<span data-ttu-id="90c98-217">Значение, которое необходимо автоматически принимать EULA на устройстве enduser.</span><span class="sxs-lookup"><span data-stu-id="90c98-217">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="90c98-218">productIds</span><span class="sxs-lookup"><span data-stu-id="90c98-218">productIds</span></span>|<span data-ttu-id="90c98-219">[коллекция officeProductId](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="90c98-219">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="90c98-220">Ids продукта, которые представляют SKU Пакета Office365.</span><span class="sxs-lookup"><span data-stu-id="90c98-220">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="90c98-221">Возможные значения: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="90c98-221">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="90c98-222">excludedApps</span><span class="sxs-lookup"><span data-stu-id="90c98-222">excludedApps</span></span>|<span data-ttu-id="90c98-223">[excludedApps](../resources/intune-apps-excludedapps.md);</span><span class="sxs-lookup"><span data-stu-id="90c98-223">[excludedApps](../resources/intune-apps-excludedapps.md)</span></span>|<span data-ttu-id="90c98-224">Свойство, которое представляет приложения, исключенные из выбранного Id продукта Office365.</span><span class="sxs-lookup"><span data-stu-id="90c98-224">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="90c98-225">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="90c98-225">useSharedComputerActivation</span></span>|<span data-ttu-id="90c98-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="90c98-226">Boolean</span></span>|<span data-ttu-id="90c98-227">Свойство, которое представляет, используется ли активация общего компьютера не для пакета приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="90c98-227">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="90c98-228">updateChannel</span><span class="sxs-lookup"><span data-stu-id="90c98-228">updateChannel</span></span>|[<span data-ttu-id="90c98-229">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="90c98-229">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="90c98-230">Свойство, представляюное канал обновления Office365.</span><span class="sxs-lookup"><span data-stu-id="90c98-230">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="90c98-231">Возможные значения: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="90c98-231">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.</span></span>|
|<span data-ttu-id="90c98-232">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="90c98-232">officePlatformArchitecture</span></span>|[<span data-ttu-id="90c98-233">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="90c98-233">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="90c98-234">Свойство для представления версии пакета приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="90c98-234">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="90c98-235">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="90c98-235">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="90c98-236">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="90c98-236">localesToInstall</span></span>|<span data-ttu-id="90c98-237">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="90c98-237">String collection</span></span>|<span data-ttu-id="90c98-238">Свойство, которое будет представлять локальные органы, установленные при установке приложений из Office365.</span><span class="sxs-lookup"><span data-stu-id="90c98-238">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="90c98-239">Он использует стандартный RFC 6033.</span><span class="sxs-lookup"><span data-stu-id="90c98-239">It uses standard RFC 6033.</span></span> <span data-ttu-id="90c98-240">Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="90c98-240">Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="90c98-241">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="90c98-241">installProgressDisplayLevel</span></span>|[<span data-ttu-id="90c98-242">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="90c98-242">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="90c98-243">Чтобы указать уровень отображения пользовательского интерфейса установки установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="90c98-243">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="90c98-244">Возможные значения: `none`, `full`.</span><span class="sxs-lookup"><span data-stu-id="90c98-244">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="90c98-245">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="90c98-245">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="90c98-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="90c98-246">Boolean</span></span>|<span data-ttu-id="90c98-247">Свойство, определяющее, следует ли удалить существующие MSI Office, если набор приложений Office365 развернут на устройстве или нет.</span><span class="sxs-lookup"><span data-stu-id="90c98-247">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="90c98-248">targetVersion</span><span class="sxs-lookup"><span data-stu-id="90c98-248">targetVersion</span></span>|<span data-ttu-id="90c98-249">Строка</span><span class="sxs-lookup"><span data-stu-id="90c98-249">String</span></span>|<span data-ttu-id="90c98-250">Свойство, которое должно представлять конкретную целевую версию пакета приложений Office365, которая должна быть развернута на устройствах.</span><span class="sxs-lookup"><span data-stu-id="90c98-250">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="90c98-251">updateVersion</span><span class="sxs-lookup"><span data-stu-id="90c98-251">updateVersion</span></span>|<span data-ttu-id="90c98-252">Строка</span><span class="sxs-lookup"><span data-stu-id="90c98-252">String</span></span>|<span data-ttu-id="90c98-253">Свойство, которое представляет версию обновления, в которой конкретная целевая версия доступна для пакета приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="90c98-253">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="90c98-254">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="90c98-254">officeConfigurationXml</span></span>|<span data-ttu-id="90c98-255">Binary</span><span class="sxs-lookup"><span data-stu-id="90c98-255">Binary</span></span>|<span data-ttu-id="90c98-256">Свойство, которое представляет XML-файл конфигурации, который может быть указан для Приложений Office ProPlus.</span><span class="sxs-lookup"><span data-stu-id="90c98-256">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="90c98-257">Имеет приоритет над всеми другими свойствами.</span><span class="sxs-lookup"><span data-stu-id="90c98-257">Takes precedence over all other properties.</span></span> <span data-ttu-id="90c98-258">В настоящее время для создания приложения будет использоваться XML-файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="90c98-258">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="90c98-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="90c98-259">Response</span></span>
<span data-ttu-id="90c98-260">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="90c98-260">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90c98-261">Пример</span><span class="sxs-lookup"><span data-stu-id="90c98-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="90c98-262">Запрос</span><span class="sxs-lookup"><span data-stu-id="90c98-262">Request</span></span>
<span data-ttu-id="90c98-263">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90c98-263">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1675

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "bing": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="90c98-264">Отклик</span><span class="sxs-lookup"><span data-stu-id="90c98-264">Response</span></span>
<span data-ttu-id="90c98-p127">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90c98-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1847

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "bing": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```




