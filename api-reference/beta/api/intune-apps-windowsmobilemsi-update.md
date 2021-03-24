---
title: Update windowsMobileMSI
description: Обновление свойств объекта windowsMobileMSI.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c934202d4f0373023a19eb786f21a328a121ba4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138836"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="e8604-103">Update windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="e8604-103">Update windowsMobileMSI</span></span>

<span data-ttu-id="e8604-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8604-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8604-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8604-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8604-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8604-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8604-107">Обновление свойств объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-107">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8604-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e8604-108">Prerequisites</span></span>
<span data-ttu-id="e8604-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8604-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8604-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8604-111">Permission type</span></span>|<span data-ttu-id="e8604-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8604-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8604-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8604-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8604-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8604-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e8604-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8604-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8604-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8604-116">Not supported.</span></span>|
|<span data-ttu-id="e8604-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e8604-117">Application</span></span>|<span data-ttu-id="e8604-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8604-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8604-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8604-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e8604-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e8604-120">Request headers</span></span>
|<span data-ttu-id="e8604-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8604-121">Header</span></span>|<span data-ttu-id="e8604-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e8604-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8604-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8604-123">Authorization</span></span>|<span data-ttu-id="e8604-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8604-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8604-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8604-125">Accept</span></span>|<span data-ttu-id="e8604-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8604-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8604-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8604-127">Request body</span></span>
<span data-ttu-id="e8604-128">В теле запроса добавьте представление объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8604-128">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="e8604-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-129">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="e8604-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8604-130">Property</span></span>|<span data-ttu-id="e8604-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e8604-131">Type</span></span>|<span data-ttu-id="e8604-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e8604-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8604-133">id</span><span class="sxs-lookup"><span data-stu-id="e8604-133">id</span></span>|<span data-ttu-id="e8604-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e8604-134">String</span></span>|<span data-ttu-id="e8604-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e8604-135">Key of the entity.</span></span> <span data-ttu-id="e8604-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e8604-137">displayName</span></span>|<span data-ttu-id="e8604-138">Строка</span><span class="sxs-lookup"><span data-stu-id="e8604-138">String</span></span>|<span data-ttu-id="e8604-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e8604-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e8604-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-141">description</span><span class="sxs-lookup"><span data-stu-id="e8604-141">description</span></span>|<span data-ttu-id="e8604-142">Строка</span><span class="sxs-lookup"><span data-stu-id="e8604-142">String</span></span>|<span data-ttu-id="e8604-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e8604-143">The description of the app.</span></span> <span data-ttu-id="e8604-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e8604-145">publisher</span></span>|<span data-ttu-id="e8604-146">String</span><span class="sxs-lookup"><span data-stu-id="e8604-146">String</span></span>|<span data-ttu-id="e8604-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e8604-147">The publisher of the app.</span></span> <span data-ttu-id="e8604-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e8604-149">largeIcon</span></span>|[<span data-ttu-id="e8604-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e8604-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e8604-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e8604-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e8604-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8604-153">createdDateTime</span></span>|<span data-ttu-id="e8604-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8604-154">DateTimeOffset</span></span>|<span data-ttu-id="e8604-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e8604-155">The date and time the app was created.</span></span> <span data-ttu-id="e8604-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8604-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e8604-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8604-158">DateTimeOffset</span></span>|<span data-ttu-id="e8604-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e8604-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e8604-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e8604-161">isFeatured</span></span>|<span data-ttu-id="e8604-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8604-162">Boolean</span></span>|<span data-ttu-id="e8604-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e8604-164">privacyInformationUrl</span></span>|<span data-ttu-id="e8604-165">String</span><span class="sxs-lookup"><span data-stu-id="e8604-165">String</span></span>|<span data-ttu-id="e8604-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e8604-166">The privacy statement Url.</span></span> <span data-ttu-id="e8604-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e8604-168">informationUrl</span></span>|<span data-ttu-id="e8604-169">String</span><span class="sxs-lookup"><span data-stu-id="e8604-169">String</span></span>|<span data-ttu-id="e8604-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e8604-170">The more information Url.</span></span> <span data-ttu-id="e8604-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-172">owner</span><span class="sxs-lookup"><span data-stu-id="e8604-172">owner</span></span>|<span data-ttu-id="e8604-173">String</span><span class="sxs-lookup"><span data-stu-id="e8604-173">String</span></span>|<span data-ttu-id="e8604-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e8604-174">The owner of the app.</span></span> <span data-ttu-id="e8604-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-176">developer</span><span class="sxs-lookup"><span data-stu-id="e8604-176">developer</span></span>|<span data-ttu-id="e8604-177">String</span><span class="sxs-lookup"><span data-stu-id="e8604-177">String</span></span>|<span data-ttu-id="e8604-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e8604-178">The developer of the app.</span></span> <span data-ttu-id="e8604-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-180">notes</span><span class="sxs-lookup"><span data-stu-id="e8604-180">notes</span></span>|<span data-ttu-id="e8604-181">String</span><span class="sxs-lookup"><span data-stu-id="e8604-181">String</span></span>|<span data-ttu-id="e8604-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="e8604-182">Notes for the app.</span></span> <span data-ttu-id="e8604-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e8604-184">uploadState</span></span>|<span data-ttu-id="e8604-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e8604-185">Int32</span></span>|<span data-ttu-id="e8604-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="e8604-186">The upload state.</span></span> <span data-ttu-id="e8604-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="e8604-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="e8604-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="e8604-189">publishingState</span></span>|[<span data-ttu-id="e8604-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e8604-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e8604-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="e8604-191">The publishing state for the app.</span></span> <span data-ttu-id="e8604-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e8604-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e8604-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e8604-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e8604-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e8604-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e8604-195">isAssigned</span></span>|<span data-ttu-id="e8604-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8604-196">Boolean</span></span>|<span data-ttu-id="e8604-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="e8604-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e8604-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e8604-199">roleScopeTagIds</span></span>|<span data-ttu-id="e8604-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e8604-200">String collection</span></span>|<span data-ttu-id="e8604-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e8604-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e8604-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e8604-203">dependentAppCount</span></span>|<span data-ttu-id="e8604-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e8604-204">Int32</span></span>|<span data-ttu-id="e8604-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="e8604-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e8604-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="e8604-207">supersedingAppCount</span></span>|<span data-ttu-id="e8604-208">Int32</span><span class="sxs-lookup"><span data-stu-id="e8604-208">Int32</span></span>|<span data-ttu-id="e8604-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="e8604-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="e8604-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="e8604-211">supersededAppCount</span></span>|<span data-ttu-id="e8604-212">Int32</span><span class="sxs-lookup"><span data-stu-id="e8604-212">Int32</span></span>|<span data-ttu-id="e8604-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="e8604-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="e8604-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e8604-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e8604-215">committedContentVersion</span></span>|<span data-ttu-id="e8604-216">String</span><span class="sxs-lookup"><span data-stu-id="e8604-216">String</span></span>|<span data-ttu-id="e8604-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="e8604-217">The internal committed content version.</span></span> <span data-ttu-id="e8604-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e8604-219">fileName</span><span class="sxs-lookup"><span data-stu-id="e8604-219">fileName</span></span>|<span data-ttu-id="e8604-220">String</span><span class="sxs-lookup"><span data-stu-id="e8604-220">String</span></span>|<span data-ttu-id="e8604-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="e8604-221">The name of the main Lob application file.</span></span> <span data-ttu-id="e8604-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e8604-223">size</span><span class="sxs-lookup"><span data-stu-id="e8604-223">size</span></span>|<span data-ttu-id="e8604-224">Int64</span><span class="sxs-lookup"><span data-stu-id="e8604-224">Int64</span></span>|<span data-ttu-id="e8604-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="e8604-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="e8604-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e8604-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e8604-227">commandLine</span><span class="sxs-lookup"><span data-stu-id="e8604-227">commandLine</span></span>|<span data-ttu-id="e8604-228">String</span><span class="sxs-lookup"><span data-stu-id="e8604-228">String</span></span>|<span data-ttu-id="e8604-229">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="e8604-229">The command line.</span></span>|
|<span data-ttu-id="e8604-230">productCode</span><span class="sxs-lookup"><span data-stu-id="e8604-230">productCode</span></span>|<span data-ttu-id="e8604-231">String</span><span class="sxs-lookup"><span data-stu-id="e8604-231">String</span></span>|<span data-ttu-id="e8604-232">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="e8604-232">The product code.</span></span>|
|<span data-ttu-id="e8604-233">productVersion</span><span class="sxs-lookup"><span data-stu-id="e8604-233">productVersion</span></span>|<span data-ttu-id="e8604-234">String</span><span class="sxs-lookup"><span data-stu-id="e8604-234">String</span></span>|<span data-ttu-id="e8604-235">Версия бизнес-приложения, к которому применяется MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="e8604-235">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e8604-236">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="e8604-236">ignoreVersionDetection</span></span>|<span data-ttu-id="e8604-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8604-237">Boolean</span></span>|<span data-ttu-id="e8604-238">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="e8604-238">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="e8604-239">Задайте значение true для бизнес-приложений MSI для Windows Mobile с функцией самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="e8604-239">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="e8604-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e8604-240">identityVersion</span></span>|<span data-ttu-id="e8604-241">String</span><span class="sxs-lookup"><span data-stu-id="e8604-241">String</span></span>|<span data-ttu-id="e8604-242">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e8604-242">The identity version.</span></span>|
|<span data-ttu-id="e8604-243">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="e8604-243">useDeviceContext</span></span>|<span data-ttu-id="e8604-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8604-244">Boolean</span></span>|<span data-ttu-id="e8604-245">Указывает, следует ли устанавливать MSI с двойным режимом в контексте устройства.</span><span class="sxs-lookup"><span data-stu-id="e8604-245">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="e8604-246">Если это так, приложение будет установлено для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="e8604-246">If true, app will be installed for all users.</span></span> <span data-ttu-id="e8604-247">Если ложное, приложение будет установлено для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8604-247">If false, app will be installed per-user.</span></span> <span data-ttu-id="e8604-248">Если нет, служба будет использовать контекст установки пакета MSI по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e8604-248">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="e8604-249">В случае MSI с двойным режимом этот по умолчанию будет иметь значение для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8604-249">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="e8604-250">Не удается установить для приложений, не в двух режимах.</span><span class="sxs-lookup"><span data-stu-id="e8604-250">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="e8604-251">Невозможно изменить после первоначального создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e8604-251">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="e8604-252">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8604-252">Response</span></span>
<span data-ttu-id="e8604-253">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e8604-253">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8604-254">Пример</span><span class="sxs-lookup"><span data-stu-id="e8604-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8604-255">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8604-255">Request</span></span>
<span data-ttu-id="e8604-256">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8604-256">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1123

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="e8604-257">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8604-257">Response</span></span>
<span data-ttu-id="e8604-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8604-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1295

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




