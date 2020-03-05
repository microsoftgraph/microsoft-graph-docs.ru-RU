---
title: Обновление Андроидманажедсторевебапп
description: Обновление свойств объекта Андроидманажедсторевебапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c2bf5c47ad9a30eb6d3b5c012981e3e56c0553f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445836"
---
# <a name="update-androidmanagedstorewebapp"></a><span data-ttu-id="d57b1-103">Обновление Андроидманажедсторевебапп</span><span class="sxs-lookup"><span data-stu-id="d57b1-103">Update androidManagedStoreWebApp</span></span>

<span data-ttu-id="d57b1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d57b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d57b1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d57b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d57b1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d57b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d57b1-107">Обновление свойств объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d57b1-107">Update the properties of a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d57b1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d57b1-108">Prerequisites</span></span>
<span data-ttu-id="d57b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d57b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d57b1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d57b1-111">Permission type</span></span>|<span data-ttu-id="d57b1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d57b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d57b1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d57b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d57b1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d57b1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d57b1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d57b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d57b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d57b1-116">Not supported.</span></span>|
|<span data-ttu-id="d57b1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d57b1-117">Application</span></span>|<span data-ttu-id="d57b1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d57b1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d57b1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d57b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="d57b1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d57b1-120">Request headers</span></span>
|<span data-ttu-id="d57b1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d57b1-121">Header</span></span>|<span data-ttu-id="d57b1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d57b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d57b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d57b1-123">Authorization</span></span>|<span data-ttu-id="d57b1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d57b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d57b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d57b1-125">Accept</span></span>|<span data-ttu-id="d57b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d57b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d57b1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d57b1-127">Request body</span></span>
<span data-ttu-id="d57b1-128">В тексте запроса добавьте представление объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d57b1-128">In the request body, supply a JSON representation for the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

<span data-ttu-id="d57b1-129">В следующей таблице приведены свойства, необходимые при создании [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-129">The following table shows the properties that are required when you create the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span></span>

|<span data-ttu-id="d57b1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d57b1-130">Property</span></span>|<span data-ttu-id="d57b1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d57b1-131">Type</span></span>|<span data-ttu-id="d57b1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d57b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d57b1-133">id</span><span class="sxs-lookup"><span data-stu-id="d57b1-133">id</span></span>|<span data-ttu-id="d57b1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d57b1-134">String</span></span>|<span data-ttu-id="d57b1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d57b1-135">Key of the entity.</span></span> <span data-ttu-id="d57b1-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d57b1-137">displayName</span></span>|<span data-ttu-id="d57b1-138">Строка</span><span class="sxs-lookup"><span data-stu-id="d57b1-138">String</span></span>|<span data-ttu-id="d57b1-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d57b1-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d57b1-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-141">description</span><span class="sxs-lookup"><span data-stu-id="d57b1-141">description</span></span>|<span data-ttu-id="d57b1-142">Строка</span><span class="sxs-lookup"><span data-stu-id="d57b1-142">String</span></span>|<span data-ttu-id="d57b1-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d57b1-143">The description of the app.</span></span> <span data-ttu-id="d57b1-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d57b1-145">publisher</span></span>|<span data-ttu-id="d57b1-146">String</span><span class="sxs-lookup"><span data-stu-id="d57b1-146">String</span></span>|<span data-ttu-id="d57b1-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d57b1-147">The publisher of the app.</span></span> <span data-ttu-id="d57b1-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d57b1-149">largeIcon</span></span>|[<span data-ttu-id="d57b1-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d57b1-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d57b1-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d57b1-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d57b1-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d57b1-153">createdDateTime</span></span>|<span data-ttu-id="d57b1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d57b1-154">DateTimeOffset</span></span>|<span data-ttu-id="d57b1-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d57b1-155">The date and time the app was created.</span></span> <span data-ttu-id="d57b1-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d57b1-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d57b1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d57b1-158">DateTimeOffset</span></span>|<span data-ttu-id="d57b1-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d57b1-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d57b1-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d57b1-161">isFeatured</span></span>|<span data-ttu-id="d57b1-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d57b1-162">Boolean</span></span>|<span data-ttu-id="d57b1-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d57b1-164">privacyInformationUrl</span></span>|<span data-ttu-id="d57b1-165">String</span><span class="sxs-lookup"><span data-stu-id="d57b1-165">String</span></span>|<span data-ttu-id="d57b1-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d57b1-166">The privacy statement Url.</span></span> <span data-ttu-id="d57b1-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d57b1-168">informationUrl</span></span>|<span data-ttu-id="d57b1-169">String</span><span class="sxs-lookup"><span data-stu-id="d57b1-169">String</span></span>|<span data-ttu-id="d57b1-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d57b1-170">The more information Url.</span></span> <span data-ttu-id="d57b1-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-172">owner</span><span class="sxs-lookup"><span data-stu-id="d57b1-172">owner</span></span>|<span data-ttu-id="d57b1-173">String</span><span class="sxs-lookup"><span data-stu-id="d57b1-173">String</span></span>|<span data-ttu-id="d57b1-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d57b1-174">The owner of the app.</span></span> <span data-ttu-id="d57b1-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-176">developer</span><span class="sxs-lookup"><span data-stu-id="d57b1-176">developer</span></span>|<span data-ttu-id="d57b1-177">String</span><span class="sxs-lookup"><span data-stu-id="d57b1-177">String</span></span>|<span data-ttu-id="d57b1-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d57b1-178">The developer of the app.</span></span> <span data-ttu-id="d57b1-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-180">notes</span><span class="sxs-lookup"><span data-stu-id="d57b1-180">notes</span></span>|<span data-ttu-id="d57b1-181">String</span><span class="sxs-lookup"><span data-stu-id="d57b1-181">String</span></span>|<span data-ttu-id="d57b1-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="d57b1-182">Notes for the app.</span></span> <span data-ttu-id="d57b1-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d57b1-184">uploadState</span></span>|<span data-ttu-id="d57b1-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d57b1-185">Int32</span></span>|<span data-ttu-id="d57b1-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="d57b1-186">The upload state.</span></span> <span data-ttu-id="d57b1-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d57b1-188">publishingState</span></span>|[<span data-ttu-id="d57b1-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="d57b1-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d57b1-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="d57b1-190">The publishing state for the app.</span></span> <span data-ttu-id="d57b1-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d57b1-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d57b1-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="d57b1-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d57b1-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d57b1-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d57b1-194">isAssigned</span></span>|<span data-ttu-id="d57b1-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="d57b1-195">Boolean</span></span>|<span data-ttu-id="d57b1-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="d57b1-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d57b1-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d57b1-198">roleScopeTagIds</span></span>|<span data-ttu-id="d57b1-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d57b1-199">String collection</span></span>|<span data-ttu-id="d57b1-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d57b1-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d57b1-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="d57b1-202">dependentAppCount</span></span>|<span data-ttu-id="d57b1-203">Int32</span><span class="sxs-lookup"><span data-stu-id="d57b1-203">Int32</span></span>|<span data-ttu-id="d57b1-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="d57b1-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d57b1-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d57b1-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d57b1-206">packageId</span><span class="sxs-lookup"><span data-stu-id="d57b1-206">packageId</span></span>|<span data-ttu-id="d57b1-207">String</span><span class="sxs-lookup"><span data-stu-id="d57b1-207">String</span></span>|<span data-ttu-id="d57b1-208">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="d57b1-208">The package identifier.</span></span> <span data-ttu-id="d57b1-209">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d57b1-209">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d57b1-210">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d57b1-210">appIdentifier</span></span>|<span data-ttu-id="d57b1-211">String</span><span class="sxs-lookup"><span data-stu-id="d57b1-211">String</span></span>|<span data-ttu-id="d57b1-212">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d57b1-212">The Identity Name.</span></span> <span data-ttu-id="d57b1-213">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d57b1-213">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d57b1-214">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d57b1-214">usedLicenseCount</span></span>|<span data-ttu-id="d57b1-215">Int32</span><span class="sxs-lookup"><span data-stu-id="d57b1-215">Int32</span></span>|<span data-ttu-id="d57b1-216">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="d57b1-216">The number of VPP licenses in use.</span></span> <span data-ttu-id="d57b1-217">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d57b1-217">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d57b1-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d57b1-218">totalLicenseCount</span></span>|<span data-ttu-id="d57b1-219">Int32</span><span class="sxs-lookup"><span data-stu-id="d57b1-219">Int32</span></span>|<span data-ttu-id="d57b1-220">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="d57b1-220">The total number of VPP licenses.</span></span> <span data-ttu-id="d57b1-221">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d57b1-221">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d57b1-222">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d57b1-222">appStoreUrl</span></span>|<span data-ttu-id="d57b1-223">String</span><span class="sxs-lookup"><span data-stu-id="d57b1-223">String</span></span>|<span data-ttu-id="d57b1-224">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="d57b1-224">The Play for Work Store app URL.</span></span> <span data-ttu-id="d57b1-225">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d57b1-225">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d57b1-226">Частный</span><span class="sxs-lookup"><span data-stu-id="d57b1-226">isPrivate</span></span>|<span data-ttu-id="d57b1-227">Логический</span><span class="sxs-lookup"><span data-stu-id="d57b1-227">Boolean</span></span>|<span data-ttu-id="d57b1-228">Указывает, доступно ли приложение только для указанных пользователей предприятия.</span><span class="sxs-lookup"><span data-stu-id="d57b1-228">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="d57b1-229">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d57b1-229">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d57b1-230">иссистемапп</span><span class="sxs-lookup"><span data-stu-id="d57b1-230">isSystemApp</span></span>|<span data-ttu-id="d57b1-231">Логический</span><span class="sxs-lookup"><span data-stu-id="d57b1-231">Boolean</span></span>|<span data-ttu-id="d57b1-232">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="d57b1-232">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="d57b1-233">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d57b1-233">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d57b1-234">суппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="d57b1-234">supportsOemConfig</span></span>|<span data-ttu-id="d57b1-235">Логический</span><span class="sxs-lookup"><span data-stu-id="d57b1-235">Boolean</span></span>|<span data-ttu-id="d57b1-236">Поддерживает ли это приложение политику Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="d57b1-236">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="d57b1-237">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d57b1-237">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d57b1-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="d57b1-238">Response</span></span>
<span data-ttu-id="d57b1-239">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d57b1-239">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d57b1-240">Пример</span><span class="sxs-lookup"><span data-stu-id="d57b1-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="d57b1-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="d57b1-241">Request</span></span>
<span data-ttu-id="d57b1-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d57b1-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 987

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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="d57b1-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="d57b1-243">Response</span></span>
<span data-ttu-id="d57b1-p127">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d57b1-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1159

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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```





