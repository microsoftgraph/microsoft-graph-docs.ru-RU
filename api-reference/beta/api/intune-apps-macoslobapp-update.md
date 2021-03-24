---
title: Обновление macOSLobApp
description: Обновление свойств объекта macOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e2edf66f0e4cd68103b7a41d1de36f983ee0d66
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143957"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="326d7-103">Обновление macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="326d7-103">Update macOSLobApp</span></span>

<span data-ttu-id="326d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="326d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="326d7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="326d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="326d7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="326d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="326d7-107">Обновление свойств объекта [macOSLobApp.](../resources/intune-apps-macoslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="326d7-107">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="326d7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="326d7-108">Prerequisites</span></span>
<span data-ttu-id="326d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="326d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="326d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="326d7-111">Permission type</span></span>|<span data-ttu-id="326d7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="326d7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="326d7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="326d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="326d7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="326d7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="326d7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="326d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="326d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="326d7-116">Not supported.</span></span>|
|<span data-ttu-id="326d7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="326d7-117">Application</span></span>|<span data-ttu-id="326d7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="326d7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="326d7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="326d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="326d7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="326d7-120">Request headers</span></span>
|<span data-ttu-id="326d7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="326d7-121">Header</span></span>|<span data-ttu-id="326d7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="326d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="326d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="326d7-123">Authorization</span></span>|<span data-ttu-id="326d7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="326d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="326d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="326d7-125">Accept</span></span>|<span data-ttu-id="326d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="326d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="326d7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="326d7-127">Request body</span></span>
<span data-ttu-id="326d7-128">В теле запроса поставляем представление JSON для [объекта macOSLobApp.](../resources/intune-apps-macoslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="326d7-128">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="326d7-129">В следующей таблице показаны свойства, необходимые при создании [macOSLobApp.](../resources/intune-apps-macoslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="326d7-129">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="326d7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="326d7-130">Property</span></span>|<span data-ttu-id="326d7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="326d7-131">Type</span></span>|<span data-ttu-id="326d7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="326d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="326d7-133">id</span><span class="sxs-lookup"><span data-stu-id="326d7-133">id</span></span>|<span data-ttu-id="326d7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="326d7-134">String</span></span>|<span data-ttu-id="326d7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="326d7-135">Key of the entity.</span></span> <span data-ttu-id="326d7-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="326d7-137">displayName</span></span>|<span data-ttu-id="326d7-138">Строка</span><span class="sxs-lookup"><span data-stu-id="326d7-138">String</span></span>|<span data-ttu-id="326d7-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="326d7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="326d7-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-141">description</span><span class="sxs-lookup"><span data-stu-id="326d7-141">description</span></span>|<span data-ttu-id="326d7-142">Строка</span><span class="sxs-lookup"><span data-stu-id="326d7-142">String</span></span>|<span data-ttu-id="326d7-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="326d7-143">The description of the app.</span></span> <span data-ttu-id="326d7-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="326d7-145">publisher</span></span>|<span data-ttu-id="326d7-146">String</span><span class="sxs-lookup"><span data-stu-id="326d7-146">String</span></span>|<span data-ttu-id="326d7-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="326d7-147">The publisher of the app.</span></span> <span data-ttu-id="326d7-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="326d7-149">largeIcon</span></span>|[<span data-ttu-id="326d7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="326d7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="326d7-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="326d7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="326d7-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="326d7-153">createdDateTime</span></span>|<span data-ttu-id="326d7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="326d7-154">DateTimeOffset</span></span>|<span data-ttu-id="326d7-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="326d7-155">The date and time the app was created.</span></span> <span data-ttu-id="326d7-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="326d7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="326d7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="326d7-158">DateTimeOffset</span></span>|<span data-ttu-id="326d7-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="326d7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="326d7-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="326d7-161">isFeatured</span></span>|<span data-ttu-id="326d7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="326d7-162">Boolean</span></span>|<span data-ttu-id="326d7-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="326d7-164">privacyInformationUrl</span></span>|<span data-ttu-id="326d7-165">String</span><span class="sxs-lookup"><span data-stu-id="326d7-165">String</span></span>|<span data-ttu-id="326d7-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="326d7-166">The privacy statement Url.</span></span> <span data-ttu-id="326d7-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="326d7-168">informationUrl</span></span>|<span data-ttu-id="326d7-169">String</span><span class="sxs-lookup"><span data-stu-id="326d7-169">String</span></span>|<span data-ttu-id="326d7-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="326d7-170">The more information Url.</span></span> <span data-ttu-id="326d7-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-172">owner</span><span class="sxs-lookup"><span data-stu-id="326d7-172">owner</span></span>|<span data-ttu-id="326d7-173">String</span><span class="sxs-lookup"><span data-stu-id="326d7-173">String</span></span>|<span data-ttu-id="326d7-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="326d7-174">The owner of the app.</span></span> <span data-ttu-id="326d7-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-176">developer</span><span class="sxs-lookup"><span data-stu-id="326d7-176">developer</span></span>|<span data-ttu-id="326d7-177">String</span><span class="sxs-lookup"><span data-stu-id="326d7-177">String</span></span>|<span data-ttu-id="326d7-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="326d7-178">The developer of the app.</span></span> <span data-ttu-id="326d7-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-180">notes</span><span class="sxs-lookup"><span data-stu-id="326d7-180">notes</span></span>|<span data-ttu-id="326d7-181">String</span><span class="sxs-lookup"><span data-stu-id="326d7-181">String</span></span>|<span data-ttu-id="326d7-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="326d7-182">Notes for the app.</span></span> <span data-ttu-id="326d7-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="326d7-184">uploadState</span></span>|<span data-ttu-id="326d7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="326d7-185">Int32</span></span>|<span data-ttu-id="326d7-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="326d7-186">The upload state.</span></span> <span data-ttu-id="326d7-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="326d7-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="326d7-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="326d7-189">publishingState</span></span>|[<span data-ttu-id="326d7-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="326d7-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="326d7-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="326d7-191">The publishing state for the app.</span></span> <span data-ttu-id="326d7-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="326d7-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="326d7-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="326d7-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="326d7-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="326d7-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="326d7-195">isAssigned</span></span>|<span data-ttu-id="326d7-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="326d7-196">Boolean</span></span>|<span data-ttu-id="326d7-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="326d7-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="326d7-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="326d7-199">roleScopeTagIds</span></span>|<span data-ttu-id="326d7-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="326d7-200">String collection</span></span>|<span data-ttu-id="326d7-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="326d7-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="326d7-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="326d7-203">dependentAppCount</span></span>|<span data-ttu-id="326d7-204">Int32</span><span class="sxs-lookup"><span data-stu-id="326d7-204">Int32</span></span>|<span data-ttu-id="326d7-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="326d7-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="326d7-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="326d7-207">supersedingAppCount</span></span>|<span data-ttu-id="326d7-208">Int32</span><span class="sxs-lookup"><span data-stu-id="326d7-208">Int32</span></span>|<span data-ttu-id="326d7-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="326d7-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="326d7-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="326d7-211">supersededAppCount</span></span>|<span data-ttu-id="326d7-212">Int32</span><span class="sxs-lookup"><span data-stu-id="326d7-212">Int32</span></span>|<span data-ttu-id="326d7-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="326d7-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="326d7-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="326d7-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="326d7-215">committedContentVersion</span></span>|<span data-ttu-id="326d7-216">String</span><span class="sxs-lookup"><span data-stu-id="326d7-216">String</span></span>|<span data-ttu-id="326d7-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="326d7-217">The internal committed content version.</span></span> <span data-ttu-id="326d7-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="326d7-219">fileName</span><span class="sxs-lookup"><span data-stu-id="326d7-219">fileName</span></span>|<span data-ttu-id="326d7-220">String</span><span class="sxs-lookup"><span data-stu-id="326d7-220">String</span></span>|<span data-ttu-id="326d7-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="326d7-221">The name of the main Lob application file.</span></span> <span data-ttu-id="326d7-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="326d7-223">size</span><span class="sxs-lookup"><span data-stu-id="326d7-223">size</span></span>|<span data-ttu-id="326d7-224">Int64</span><span class="sxs-lookup"><span data-stu-id="326d7-224">Int64</span></span>|<span data-ttu-id="326d7-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="326d7-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="326d7-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="326d7-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="326d7-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="326d7-227">bundleId</span></span>|<span data-ttu-id="326d7-228">String</span><span class="sxs-lookup"><span data-stu-id="326d7-228">String</span></span>|<span data-ttu-id="326d7-229">ID пакета.</span><span class="sxs-lookup"><span data-stu-id="326d7-229">The bundle id.</span></span>|
|<span data-ttu-id="326d7-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="326d7-230">minimumSupportedOperatingSystem</span></span>|<span data-ttu-id="326d7-231">[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md);</span><span class="sxs-lookup"><span data-stu-id="326d7-231">[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md)</span></span>|<span data-ttu-id="326d7-232">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="326d7-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="326d7-233">buildNumber</span><span class="sxs-lookup"><span data-stu-id="326d7-233">buildNumber</span></span>|<span data-ttu-id="326d7-234">String</span><span class="sxs-lookup"><span data-stu-id="326d7-234">String</span></span>|<span data-ttu-id="326d7-235">Число сборки приложения MacOS Line of Business (LoB).</span><span class="sxs-lookup"><span data-stu-id="326d7-235">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="326d7-236">versionNumber</span><span class="sxs-lookup"><span data-stu-id="326d7-236">versionNumber</span></span>|<span data-ttu-id="326d7-237">String</span><span class="sxs-lookup"><span data-stu-id="326d7-237">String</span></span>|<span data-ttu-id="326d7-238">Номер версии приложения MacOS Line of Business (LoB).</span><span class="sxs-lookup"><span data-stu-id="326d7-238">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="326d7-239">childApps</span><span class="sxs-lookup"><span data-stu-id="326d7-239">childApps</span></span>|<span data-ttu-id="326d7-240">[коллекция macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="326d7-240">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="326d7-241">Список приложений в этом пакете пакетов</span><span class="sxs-lookup"><span data-stu-id="326d7-241">The app list in this bundle package</span></span>|
|<span data-ttu-id="326d7-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="326d7-242">identityVersion</span></span>|<span data-ttu-id="326d7-243">String</span><span class="sxs-lookup"><span data-stu-id="326d7-243">String</span></span>|<span data-ttu-id="326d7-244">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="326d7-244">The identity version.</span></span>|
|<span data-ttu-id="326d7-245">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="326d7-245">md5HashChunkSize</span></span>|<span data-ttu-id="326d7-246">Int32</span><span class="sxs-lookup"><span data-stu-id="326d7-246">Int32</span></span>|<span data-ttu-id="326d7-247">Размер куска для hash MD5</span><span class="sxs-lookup"><span data-stu-id="326d7-247">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="326d7-248">md5Hash</span><span class="sxs-lookup"><span data-stu-id="326d7-248">md5Hash</span></span>|<span data-ttu-id="326d7-249">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="326d7-249">String collection</span></span>|<span data-ttu-id="326d7-250">Коды hash MD5</span><span class="sxs-lookup"><span data-stu-id="326d7-250">The MD5 hash codes</span></span>|
|<span data-ttu-id="326d7-251">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="326d7-251">ignoreVersionDetection</span></span>|<span data-ttu-id="326d7-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="326d7-252">Boolean</span></span>|<span data-ttu-id="326d7-253">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="326d7-253">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="326d7-254">Установите это для приложений macOS Line of Business (LoB), которые используют функцию самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="326d7-254">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="326d7-255">installAsManaged</span><span class="sxs-lookup"><span data-stu-id="326d7-255">installAsManaged</span></span>|<span data-ttu-id="326d7-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="326d7-256">Boolean</span></span>|<span data-ttu-id="326d7-257">A boolean to control whether the app will be installed as managed (requires macOS 11.0 and other PKG restrictions).</span><span class="sxs-lookup"><span data-stu-id="326d7-257">A boolean to control whether the app will be installed as managed (requires macOS 11.0 and other PKG restrictions).</span></span>|



## <a name="response"></a><span data-ttu-id="326d7-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="326d7-258">Response</span></span>
<span data-ttu-id="326d7-259">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект macOSLobApp](../resources/intune-apps-macoslobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="326d7-259">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="326d7-260">Пример</span><span class="sxs-lookup"><span data-stu-id="326d7-260">Example</span></span>

### <a name="request"></a><span data-ttu-id="326d7-261">Запрос</span><span class="sxs-lookup"><span data-stu-id="326d7-261">Request</span></span>
<span data-ttu-id="326d7-262">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="326d7-262">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="326d7-263">Отклик</span><span class="sxs-lookup"><span data-stu-id="326d7-263">Response</span></span>
<span data-ttu-id="326d7-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="326d7-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




