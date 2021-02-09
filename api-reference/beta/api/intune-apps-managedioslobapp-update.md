---
title: Update managedIOSLobApp
description: Обновление свойств объекта managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4de8289ce0ee128acc8c2c12622bbc098412b3ef
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157241"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="ccae5-103">Update managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="ccae5-103">Update managedIOSLobApp</span></span>

<span data-ttu-id="ccae5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccae5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccae5-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccae5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccae5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccae5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccae5-107">Обновление свойств объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccae5-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ccae5-108">Prerequisites</span></span>
<span data-ttu-id="ccae5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccae5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccae5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccae5-111">Permission type</span></span>|<span data-ttu-id="ccae5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccae5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccae5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccae5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ccae5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccae5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ccae5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccae5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccae5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccae5-116">Not supported.</span></span>|
|<span data-ttu-id="ccae5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccae5-117">Application</span></span>|<span data-ttu-id="ccae5-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccae5-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccae5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccae5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ccae5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ccae5-120">Request headers</span></span>
|<span data-ttu-id="ccae5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccae5-121">Header</span></span>|<span data-ttu-id="ccae5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ccae5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccae5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccae5-123">Authorization</span></span>|<span data-ttu-id="ccae5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccae5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccae5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ccae5-125">Accept</span></span>|<span data-ttu-id="ccae5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ccae5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccae5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ccae5-127">Request body</span></span>
<span data-ttu-id="ccae5-128">В теле запроса добавьте представление объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccae5-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="ccae5-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="ccae5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccae5-130">Property</span></span>|<span data-ttu-id="ccae5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ccae5-131">Type</span></span>|<span data-ttu-id="ccae5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ccae5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccae5-133">id</span><span class="sxs-lookup"><span data-stu-id="ccae5-133">id</span></span>|<span data-ttu-id="ccae5-134">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-134">String</span></span>|<span data-ttu-id="ccae5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ccae5-135">Key of the entity.</span></span> <span data-ttu-id="ccae5-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ccae5-137">displayName</span></span>|<span data-ttu-id="ccae5-138">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-138">String</span></span>|<span data-ttu-id="ccae5-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ccae5-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ccae5-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-141">description</span><span class="sxs-lookup"><span data-stu-id="ccae5-141">description</span></span>|<span data-ttu-id="ccae5-142">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-142">String</span></span>|<span data-ttu-id="ccae5-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-143">The description of the app.</span></span> <span data-ttu-id="ccae5-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ccae5-145">publisher</span></span>|<span data-ttu-id="ccae5-146">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-146">String</span></span>|<span data-ttu-id="ccae5-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-147">The publisher of the app.</span></span> <span data-ttu-id="ccae5-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ccae5-149">largeIcon</span></span>|[<span data-ttu-id="ccae5-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ccae5-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ccae5-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ccae5-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ccae5-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ccae5-153">createdDateTime</span></span>|<span data-ttu-id="ccae5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccae5-154">DateTimeOffset</span></span>|<span data-ttu-id="ccae5-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-155">The date and time the app was created.</span></span> <span data-ttu-id="ccae5-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ccae5-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ccae5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccae5-158">DateTimeOffset</span></span>|<span data-ttu-id="ccae5-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ccae5-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ccae5-161">isFeatured</span></span>|<span data-ttu-id="ccae5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccae5-162">Boolean</span></span>|<span data-ttu-id="ccae5-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ccae5-164">privacyInformationUrl</span></span>|<span data-ttu-id="ccae5-165">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-165">String</span></span>|<span data-ttu-id="ccae5-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ccae5-166">The privacy statement Url.</span></span> <span data-ttu-id="ccae5-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ccae5-168">informationUrl</span></span>|<span data-ttu-id="ccae5-169">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-169">String</span></span>|<span data-ttu-id="ccae5-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ccae5-170">The more information Url.</span></span> <span data-ttu-id="ccae5-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-172">owner</span><span class="sxs-lookup"><span data-stu-id="ccae5-172">owner</span></span>|<span data-ttu-id="ccae5-173">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-173">String</span></span>|<span data-ttu-id="ccae5-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-174">The owner of the app.</span></span> <span data-ttu-id="ccae5-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-176">developer</span><span class="sxs-lookup"><span data-stu-id="ccae5-176">developer</span></span>|<span data-ttu-id="ccae5-177">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-177">String</span></span>|<span data-ttu-id="ccae5-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-178">The developer of the app.</span></span> <span data-ttu-id="ccae5-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-180">notes</span><span class="sxs-lookup"><span data-stu-id="ccae5-180">notes</span></span>|<span data-ttu-id="ccae5-181">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-181">String</span></span>|<span data-ttu-id="ccae5-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-182">Notes for the app.</span></span> <span data-ttu-id="ccae5-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ccae5-184">uploadState</span></span>|<span data-ttu-id="ccae5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ccae5-185">Int32</span></span>|<span data-ttu-id="ccae5-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="ccae5-186">The upload state.</span></span> <span data-ttu-id="ccae5-187">Возможные значения: 0- `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="ccae5-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ccae5-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ccae5-189">publishingState</span></span>|[<span data-ttu-id="ccae5-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ccae5-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ccae5-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-191">The publishing state for the app.</span></span> <span data-ttu-id="ccae5-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ccae5-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ccae5-193">Наследуется от [mobileApp.](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ccae5-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ccae5-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ccae5-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ccae5-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ccae5-195">isAssigned</span></span>|<span data-ttu-id="ccae5-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccae5-196">Boolean</span></span>|<span data-ttu-id="ccae5-197">Значение, указывающее, назначено ли приложению хотя бы одна группа.</span><span class="sxs-lookup"><span data-stu-id="ccae5-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ccae5-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ccae5-199">roleScopeTagIds</span></span>|<span data-ttu-id="ccae5-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ccae5-200">String collection</span></span>|<span data-ttu-id="ccae5-201">Список ид тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ccae5-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ccae5-203">dependentAppCount</span></span>|<span data-ttu-id="ccae5-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ccae5-204">Int32</span></span>|<span data-ttu-id="ccae5-205">Общее количество зависимостей, которые есть у этого приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ccae5-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="ccae5-207">supersedingAppCount</span></span>|<span data-ttu-id="ccae5-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ccae5-208">Int32</span></span>|<span data-ttu-id="ccae5-209">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="ccae5-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="ccae5-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="ccae5-211">supersededAppCount</span></span>|<span data-ttu-id="ccae5-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ccae5-212">Int32</span></span>|<span data-ttu-id="ccae5-213">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="ccae5-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="ccae5-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ccae5-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="ccae5-215">appAvailability</span></span>|[<span data-ttu-id="ccae5-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="ccae5-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="ccae5-217">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-217">The Application's availability.</span></span> <span data-ttu-id="ccae5-218">Наследуется от [managedApp.](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="ccae5-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="ccae5-219">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="ccae5-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="ccae5-220">version</span><span class="sxs-lookup"><span data-stu-id="ccae5-220">version</span></span>|<span data-ttu-id="ccae5-221">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-221">String</span></span>|<span data-ttu-id="ccae5-222">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-222">The Application's version.</span></span> <span data-ttu-id="ccae5-223">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="ccae5-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ccae5-224">committedContentVersion</span></span>|<span data-ttu-id="ccae5-225">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-225">String</span></span>|<span data-ttu-id="ccae5-226">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="ccae5-226">The internal committed content version.</span></span> <span data-ttu-id="ccae5-227">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ccae5-228">fileName</span><span class="sxs-lookup"><span data-stu-id="ccae5-228">fileName</span></span>|<span data-ttu-id="ccae5-229">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-229">String</span></span>|<span data-ttu-id="ccae5-230">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-230">The name of the main Lob application file.</span></span> <span data-ttu-id="ccae5-231">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ccae5-232">size</span><span class="sxs-lookup"><span data-stu-id="ccae5-232">size</span></span>|<span data-ttu-id="ccae5-233">Int64</span><span class="sxs-lookup"><span data-stu-id="ccae5-233">Int64</span></span>|<span data-ttu-id="ccae5-234">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="ccae5-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="ccae5-235">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ccae5-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ccae5-236">bundleId</span><span class="sxs-lookup"><span data-stu-id="ccae5-236">bundleId</span></span>|<span data-ttu-id="ccae5-237">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-237">String</span></span>|<span data-ttu-id="ccae5-238">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-238">The Identity Name.</span></span>|
|<span data-ttu-id="ccae5-239">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ccae5-239">applicableDeviceType</span></span>|[<span data-ttu-id="ccae5-240">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ccae5-240">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="ccae5-241">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ccae5-241">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="ccae5-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ccae5-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ccae5-243">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ccae5-243">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="ccae5-244">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ccae5-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ccae5-245">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ccae5-245">expirationDateTime</span></span>|<span data-ttu-id="ccae5-246">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccae5-246">DateTimeOffset</span></span>|<span data-ttu-id="ccae5-247">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="ccae5-247">The expiration time.</span></span>|
|<span data-ttu-id="ccae5-248">versionNumber</span><span class="sxs-lookup"><span data-stu-id="ccae5-248">versionNumber</span></span>|<span data-ttu-id="ccae5-249">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-249">String</span></span>|<span data-ttu-id="ccae5-250">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="ccae5-250">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ccae5-251">buildNumber</span><span class="sxs-lookup"><span data-stu-id="ccae5-251">buildNumber</span></span>|<span data-ttu-id="ccae5-252">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-252">String</span></span>|<span data-ttu-id="ccae5-253">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="ccae5-253">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ccae5-254">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ccae5-254">identityVersion</span></span>|<span data-ttu-id="ccae5-255">String</span><span class="sxs-lookup"><span data-stu-id="ccae5-255">String</span></span>|<span data-ttu-id="ccae5-256">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ccae5-256">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ccae5-257">Ответ</span><span class="sxs-lookup"><span data-stu-id="ccae5-257">Response</span></span>
<span data-ttu-id="ccae5-258">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ccae5-258">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccae5-259">Пример</span><span class="sxs-lookup"><span data-stu-id="ccae5-259">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccae5-260">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccae5-260">Request</span></span>
<span data-ttu-id="ccae5-261">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccae5-261">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ccae5-262">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccae5-262">Response</span></span>
<span data-ttu-id="ccae5-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccae5-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




