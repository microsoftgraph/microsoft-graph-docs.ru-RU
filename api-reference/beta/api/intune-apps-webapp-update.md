---
title: Update webApp
description: Обновление свойств объекта webApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a65ab5ba1b08ea99841636bc4f72f8c7594511a8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435072"
---
# <a name="update-webapp"></a><span data-ttu-id="ce84e-103">Update webApp</span><span class="sxs-lookup"><span data-stu-id="ce84e-103">Update webApp</span></span>

<span data-ttu-id="ce84e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce84e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce84e-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce84e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce84e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce84e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce84e-107">Обновление свойств объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-107">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce84e-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ce84e-108">Prerequisites</span></span>
<span data-ttu-id="ce84e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce84e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce84e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce84e-111">Permission type</span></span>|<span data-ttu-id="ce84e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce84e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce84e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce84e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce84e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce84e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce84e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce84e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce84e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce84e-116">Not supported.</span></span>|
|<span data-ttu-id="ce84e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ce84e-117">Application</span></span>|<span data-ttu-id="ce84e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce84e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce84e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce84e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ce84e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ce84e-120">Request headers</span></span>
|<span data-ttu-id="ce84e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce84e-121">Header</span></span>|<span data-ttu-id="ce84e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ce84e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce84e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce84e-123">Authorization</span></span>|<span data-ttu-id="ce84e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce84e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce84e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce84e-125">Accept</span></span>|<span data-ttu-id="ce84e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce84e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce84e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ce84e-127">Request body</span></span>
<span data-ttu-id="ce84e-128">В тексте запроса добавьте представление объекта [webApp](../resources/intune-apps-webapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce84e-128">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="ce84e-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-129">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="ce84e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce84e-130">Property</span></span>|<span data-ttu-id="ce84e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ce84e-131">Type</span></span>|<span data-ttu-id="ce84e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ce84e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce84e-133">id</span><span class="sxs-lookup"><span data-stu-id="ce84e-133">id</span></span>|<span data-ttu-id="ce84e-134">String</span><span class="sxs-lookup"><span data-stu-id="ce84e-134">String</span></span>|<span data-ttu-id="ce84e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ce84e-135">Key of the entity.</span></span> <span data-ttu-id="ce84e-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ce84e-137">displayName</span></span>|<span data-ttu-id="ce84e-138">String</span><span class="sxs-lookup"><span data-stu-id="ce84e-138">String</span></span>|<span data-ttu-id="ce84e-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ce84e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ce84e-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-141">description</span><span class="sxs-lookup"><span data-stu-id="ce84e-141">description</span></span>|<span data-ttu-id="ce84e-142">String</span><span class="sxs-lookup"><span data-stu-id="ce84e-142">String</span></span>|<span data-ttu-id="ce84e-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ce84e-143">The description of the app.</span></span> <span data-ttu-id="ce84e-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ce84e-145">publisher</span></span>|<span data-ttu-id="ce84e-146">String</span><span class="sxs-lookup"><span data-stu-id="ce84e-146">String</span></span>|<span data-ttu-id="ce84e-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ce84e-147">The publisher of the app.</span></span> <span data-ttu-id="ce84e-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ce84e-149">largeIcon</span></span>|[<span data-ttu-id="ce84e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ce84e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ce84e-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ce84e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ce84e-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce84e-153">createdDateTime</span></span>|<span data-ttu-id="ce84e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce84e-154">DateTimeOffset</span></span>|<span data-ttu-id="ce84e-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ce84e-155">The date and time the app was created.</span></span> <span data-ttu-id="ce84e-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce84e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ce84e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce84e-158">DateTimeOffset</span></span>|<span data-ttu-id="ce84e-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ce84e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ce84e-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ce84e-161">isFeatured</span></span>|<span data-ttu-id="ce84e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce84e-162">Boolean</span></span>|<span data-ttu-id="ce84e-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ce84e-164">privacyInformationUrl</span></span>|<span data-ttu-id="ce84e-165">String</span><span class="sxs-lookup"><span data-stu-id="ce84e-165">String</span></span>|<span data-ttu-id="ce84e-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ce84e-166">The privacy statement Url.</span></span> <span data-ttu-id="ce84e-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ce84e-168">informationUrl</span></span>|<span data-ttu-id="ce84e-169">String</span><span class="sxs-lookup"><span data-stu-id="ce84e-169">String</span></span>|<span data-ttu-id="ce84e-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ce84e-170">The more information Url.</span></span> <span data-ttu-id="ce84e-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-172">owner</span><span class="sxs-lookup"><span data-stu-id="ce84e-172">owner</span></span>|<span data-ttu-id="ce84e-173">String</span><span class="sxs-lookup"><span data-stu-id="ce84e-173">String</span></span>|<span data-ttu-id="ce84e-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ce84e-174">The owner of the app.</span></span> <span data-ttu-id="ce84e-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-176">developer</span><span class="sxs-lookup"><span data-stu-id="ce84e-176">developer</span></span>|<span data-ttu-id="ce84e-177">String</span><span class="sxs-lookup"><span data-stu-id="ce84e-177">String</span></span>|<span data-ttu-id="ce84e-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ce84e-178">The developer of the app.</span></span> <span data-ttu-id="ce84e-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-180">notes</span><span class="sxs-lookup"><span data-stu-id="ce84e-180">notes</span></span>|<span data-ttu-id="ce84e-181">String</span><span class="sxs-lookup"><span data-stu-id="ce84e-181">String</span></span>|<span data-ttu-id="ce84e-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ce84e-182">Notes for the app.</span></span> <span data-ttu-id="ce84e-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ce84e-184">uploadState</span></span>|<span data-ttu-id="ce84e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ce84e-185">Int32</span></span>|<span data-ttu-id="ce84e-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="ce84e-186">The upload state.</span></span> <span data-ttu-id="ce84e-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="ce84e-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ce84e-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ce84e-189">publishingState</span></span>|[<span data-ttu-id="ce84e-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ce84e-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ce84e-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ce84e-191">The publishing state for the app.</span></span> <span data-ttu-id="ce84e-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ce84e-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ce84e-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ce84e-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ce84e-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ce84e-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ce84e-195">isAssigned</span></span>|<span data-ttu-id="ce84e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce84e-196">Boolean</span></span>|<span data-ttu-id="ce84e-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="ce84e-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ce84e-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce84e-199">roleScopeTagIds</span></span>|<span data-ttu-id="ce84e-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ce84e-200">String collection</span></span>|<span data-ttu-id="ce84e-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ce84e-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ce84e-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ce84e-203">dependentAppCount</span></span>|<span data-ttu-id="ce84e-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ce84e-204">Int32</span></span>|<span data-ttu-id="ce84e-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="ce84e-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ce84e-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="ce84e-207">supersedingAppCount</span></span>|<span data-ttu-id="ce84e-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ce84e-208">Int32</span></span>|<span data-ttu-id="ce84e-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="ce84e-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="ce84e-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="ce84e-211">supersededAppCount</span></span>|<span data-ttu-id="ce84e-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ce84e-212">Int32</span></span>|<span data-ttu-id="ce84e-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="ce84e-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="ce84e-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce84e-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce84e-215">appUrl</span><span class="sxs-lookup"><span data-stu-id="ce84e-215">appUrl</span></span>|<span data-ttu-id="ce84e-216">String</span><span class="sxs-lookup"><span data-stu-id="ce84e-216">String</span></span>|<span data-ttu-id="ce84e-217">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="ce84e-217">The web app URL.</span></span> <span data-ttu-id="ce84e-218">Это свойство не может быть PATCHed.</span><span class="sxs-lookup"><span data-stu-id="ce84e-218">This property cannot be PATCHed.</span></span>|
|<span data-ttu-id="ce84e-219">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="ce84e-219">useManagedBrowser</span></span>|<span data-ttu-id="ce84e-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce84e-220">Boolean</span></span>|<span data-ttu-id="ce84e-221">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="ce84e-221">Whether or not to use managed browser.</span></span> <span data-ttu-id="ce84e-222">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="ce84e-222">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="ce84e-223">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce84e-223">Response</span></span>
<span data-ttu-id="ce84e-224">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [webApp](../resources/intune-apps-webapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ce84e-224">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce84e-225">Пример</span><span class="sxs-lookup"><span data-stu-id="ce84e-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce84e-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce84e-226">Request</span></span>
<span data-ttu-id="ce84e-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce84e-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 836

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="ce84e-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce84e-228">Response</span></span>
<span data-ttu-id="ce84e-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce84e-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1008

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```




