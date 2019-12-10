---
title: Обновление Андроидманажедсторевебапп
description: Обновление свойств объекта Андроидманажедсторевебапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6cbc3dee0f59f1c4b534fb5fd9747473801d7a66
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39926280"
---
# <a name="update-androidmanagedstorewebapp"></a><span data-ttu-id="bb2a9-103">Обновление Андроидманажедсторевебапп</span><span class="sxs-lookup"><span data-stu-id="bb2a9-103">Update androidManagedStoreWebApp</span></span>

> <span data-ttu-id="bb2a9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb2a9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb2a9-106">Обновление свойств объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="bb2a9-106">Update the properties of a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb2a9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bb2a9-107">Prerequisites</span></span>
<span data-ttu-id="bb2a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb2a9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb2a9-110">Permission type</span></span>|<span data-ttu-id="bb2a9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb2a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb2a9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb2a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb2a9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb2a9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bb2a9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb2a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb2a9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-115">Not supported.</span></span>|
|<span data-ttu-id="bb2a9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb2a9-116">Application</span></span>|<span data-ttu-id="bb2a9-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb2a9-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb2a9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb2a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="bb2a9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bb2a9-119">Request headers</span></span>
|<span data-ttu-id="bb2a9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb2a9-120">Header</span></span>|<span data-ttu-id="bb2a9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bb2a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb2a9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb2a9-122">Authorization</span></span>|<span data-ttu-id="bb2a9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb2a9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bb2a9-124">Accept</span></span>|<span data-ttu-id="bb2a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb2a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb2a9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bb2a9-126">Request body</span></span>
<span data-ttu-id="bb2a9-127">В тексте запроса добавьте представление объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-127">In the request body, supply a JSON representation for the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

<span data-ttu-id="bb2a9-128">В следующей таблице приведены свойства, необходимые при создании [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-128">The following table shows the properties that are required when you create the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span></span>

|<span data-ttu-id="bb2a9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb2a9-129">Property</span></span>|<span data-ttu-id="bb2a9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bb2a9-130">Type</span></span>|<span data-ttu-id="bb2a9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bb2a9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb2a9-132">id</span><span class="sxs-lookup"><span data-stu-id="bb2a9-132">id</span></span>|<span data-ttu-id="bb2a9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="bb2a9-133">String</span></span>|<span data-ttu-id="bb2a9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-134">Key of the entity.</span></span> <span data-ttu-id="bb2a9-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bb2a9-136">displayName</span></span>|<span data-ttu-id="bb2a9-137">Строка</span><span class="sxs-lookup"><span data-stu-id="bb2a9-137">String</span></span>|<span data-ttu-id="bb2a9-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bb2a9-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-140">description</span><span class="sxs-lookup"><span data-stu-id="bb2a9-140">description</span></span>|<span data-ttu-id="bb2a9-141">Строка</span><span class="sxs-lookup"><span data-stu-id="bb2a9-141">String</span></span>|<span data-ttu-id="bb2a9-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-142">The description of the app.</span></span> <span data-ttu-id="bb2a9-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-144">publisher</span><span class="sxs-lookup"><span data-stu-id="bb2a9-144">publisher</span></span>|<span data-ttu-id="bb2a9-145">Строка</span><span class="sxs-lookup"><span data-stu-id="bb2a9-145">String</span></span>|<span data-ttu-id="bb2a9-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-146">The publisher of the app.</span></span> <span data-ttu-id="bb2a9-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bb2a9-148">largeIcon</span></span>|[<span data-ttu-id="bb2a9-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bb2a9-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bb2a9-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bb2a9-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb2a9-152">createdDateTime</span></span>|<span data-ttu-id="bb2a9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb2a9-153">DateTimeOffset</span></span>|<span data-ttu-id="bb2a9-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-154">The date and time the app was created.</span></span> <span data-ttu-id="bb2a9-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb2a9-156">lastModifiedDateTime</span></span>|<span data-ttu-id="bb2a9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb2a9-157">DateTimeOffset</span></span>|<span data-ttu-id="bb2a9-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-158">The date and time the app was last modified.</span></span> <span data-ttu-id="bb2a9-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bb2a9-160">isFeatured</span></span>|<span data-ttu-id="bb2a9-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb2a9-161">Boolean</span></span>|<span data-ttu-id="bb2a9-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bb2a9-163">privacyInformationUrl</span></span>|<span data-ttu-id="bb2a9-164">Строка</span><span class="sxs-lookup"><span data-stu-id="bb2a9-164">String</span></span>|<span data-ttu-id="bb2a9-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-165">The privacy statement Url.</span></span> <span data-ttu-id="bb2a9-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bb2a9-167">informationUrl</span></span>|<span data-ttu-id="bb2a9-168">Строка</span><span class="sxs-lookup"><span data-stu-id="bb2a9-168">String</span></span>|<span data-ttu-id="bb2a9-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-169">The more information Url.</span></span> <span data-ttu-id="bb2a9-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-171">owner</span><span class="sxs-lookup"><span data-stu-id="bb2a9-171">owner</span></span>|<span data-ttu-id="bb2a9-172">String</span><span class="sxs-lookup"><span data-stu-id="bb2a9-172">String</span></span>|<span data-ttu-id="bb2a9-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-173">The owner of the app.</span></span> <span data-ttu-id="bb2a9-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-175">developer</span><span class="sxs-lookup"><span data-stu-id="bb2a9-175">developer</span></span>|<span data-ttu-id="bb2a9-176">Строка</span><span class="sxs-lookup"><span data-stu-id="bb2a9-176">String</span></span>|<span data-ttu-id="bb2a9-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-177">The developer of the app.</span></span> <span data-ttu-id="bb2a9-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-179">notes</span><span class="sxs-lookup"><span data-stu-id="bb2a9-179">notes</span></span>|<span data-ttu-id="bb2a9-180">Строка</span><span class="sxs-lookup"><span data-stu-id="bb2a9-180">String</span></span>|<span data-ttu-id="bb2a9-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-181">Notes for the app.</span></span> <span data-ttu-id="bb2a9-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="bb2a9-183">uploadState</span></span>|<span data-ttu-id="bb2a9-184">Int32</span><span class="sxs-lookup"><span data-stu-id="bb2a9-184">Int32</span></span>|<span data-ttu-id="bb2a9-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-185">The upload state.</span></span> <span data-ttu-id="bb2a9-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="bb2a9-187">publishingState</span></span>|[<span data-ttu-id="bb2a9-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="bb2a9-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bb2a9-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-189">The publishing state for the app.</span></span> <span data-ttu-id="bb2a9-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bb2a9-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="bb2a9-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bb2a9-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bb2a9-193">isAssigned</span></span>|<span data-ttu-id="bb2a9-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb2a9-194">Boolean</span></span>|<span data-ttu-id="bb2a9-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="bb2a9-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb2a9-197">roleScopeTagIds</span></span>|<span data-ttu-id="bb2a9-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bb2a9-198">String collection</span></span>|<span data-ttu-id="bb2a9-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="bb2a9-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="bb2a9-201">dependentAppCount</span></span>|<span data-ttu-id="bb2a9-202">Int32</span><span class="sxs-lookup"><span data-stu-id="bb2a9-202">Int32</span></span>|<span data-ttu-id="bb2a9-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="bb2a9-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb2a9-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb2a9-205">packageId</span><span class="sxs-lookup"><span data-stu-id="bb2a9-205">packageId</span></span>|<span data-ttu-id="bb2a9-206">Строка</span><span class="sxs-lookup"><span data-stu-id="bb2a9-206">String</span></span>|<span data-ttu-id="bb2a9-207">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-207">The package identifier.</span></span> <span data-ttu-id="bb2a9-208">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb2a9-208">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="bb2a9-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="bb2a9-209">appIdentifier</span></span>|<span data-ttu-id="bb2a9-210">String</span><span class="sxs-lookup"><span data-stu-id="bb2a9-210">String</span></span>|<span data-ttu-id="bb2a9-211">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-211">The Identity Name.</span></span> <span data-ttu-id="bb2a9-212">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb2a9-212">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="bb2a9-213">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="bb2a9-213">usedLicenseCount</span></span>|<span data-ttu-id="bb2a9-214">Int32</span><span class="sxs-lookup"><span data-stu-id="bb2a9-214">Int32</span></span>|<span data-ttu-id="bb2a9-215">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-215">The number of VPP licenses in use.</span></span> <span data-ttu-id="bb2a9-216">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb2a9-216">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="bb2a9-217">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="bb2a9-217">totalLicenseCount</span></span>|<span data-ttu-id="bb2a9-218">Int32</span><span class="sxs-lookup"><span data-stu-id="bb2a9-218">Int32</span></span>|<span data-ttu-id="bb2a9-219">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-219">The total number of VPP licenses.</span></span> <span data-ttu-id="bb2a9-220">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb2a9-220">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="bb2a9-221">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="bb2a9-221">appStoreUrl</span></span>|<span data-ttu-id="bb2a9-222">String</span><span class="sxs-lookup"><span data-stu-id="bb2a9-222">String</span></span>|<span data-ttu-id="bb2a9-223">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-223">The Play for Work Store app URL.</span></span> <span data-ttu-id="bb2a9-224">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb2a9-224">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="bb2a9-225">Частный</span><span class="sxs-lookup"><span data-stu-id="bb2a9-225">isPrivate</span></span>|<span data-ttu-id="bb2a9-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb2a9-226">Boolean</span></span>|<span data-ttu-id="bb2a9-227">Указывает, доступно ли приложение только для указанных пользователей предприятия.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-227">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="bb2a9-228">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb2a9-228">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="bb2a9-229">иссистемапп</span><span class="sxs-lookup"><span data-stu-id="bb2a9-229">isSystemApp</span></span>|<span data-ttu-id="bb2a9-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb2a9-230">Boolean</span></span>|<span data-ttu-id="bb2a9-231">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-231">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="bb2a9-232">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb2a9-232">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="bb2a9-233">суппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="bb2a9-233">supportsOemConfig</span></span>|<span data-ttu-id="bb2a9-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb2a9-234">Boolean</span></span>|<span data-ttu-id="bb2a9-235">Поддерживает ли это приложение политику Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-235">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="bb2a9-236">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb2a9-236">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="bb2a9-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb2a9-237">Response</span></span>
<span data-ttu-id="bb2a9-238">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-238">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb2a9-239">Пример</span><span class="sxs-lookup"><span data-stu-id="bb2a9-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb2a9-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb2a9-240">Request</span></span>
<span data-ttu-id="bb2a9-241">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-241">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb2a9-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb2a9-242">Response</span></span>
<span data-ttu-id="bb2a9-p127">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb2a9-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





