---
title: Обновление Андроидманажедсторевебапп
description: Обновление свойств объекта Андроидманажедсторевебапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3dd02b10a7d4bf7560cb00b2576c23b30e50968e
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535466"
---
# <a name="update-androidmanagedstorewebapp"></a><span data-ttu-id="cd370-103">Обновление Андроидманажедсторевебапп</span><span class="sxs-lookup"><span data-stu-id="cd370-103">Update androidManagedStoreWebApp</span></span>

> <span data-ttu-id="cd370-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd370-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd370-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd370-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd370-106">Обновление свойств объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="cd370-106">Update the properties of a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd370-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cd370-107">Prerequisites</span></span>
<span data-ttu-id="cd370-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd370-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd370-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd370-110">Permission type</span></span>|<span data-ttu-id="cd370-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd370-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd370-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd370-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd370-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd370-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cd370-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd370-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd370-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd370-115">Not supported.</span></span>|
|<span data-ttu-id="cd370-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cd370-116">Application</span></span>|<span data-ttu-id="cd370-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd370-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd370-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd370-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="cd370-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd370-119">Request headers</span></span>
|<span data-ttu-id="cd370-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd370-120">Header</span></span>|<span data-ttu-id="cd370-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cd370-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd370-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd370-122">Authorization</span></span>|<span data-ttu-id="cd370-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd370-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd370-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cd370-124">Accept</span></span>|<span data-ttu-id="cd370-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd370-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd370-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd370-126">Request body</span></span>
<span data-ttu-id="cd370-127">В тексте запроса добавьте представление объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd370-127">In the request body, supply a JSON representation for the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

<span data-ttu-id="cd370-128">В следующей таблице приведены свойства, необходимые при создании [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-128">The following table shows the properties that are required when you create the [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).</span></span>

|<span data-ttu-id="cd370-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd370-129">Property</span></span>|<span data-ttu-id="cd370-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cd370-130">Type</span></span>|<span data-ttu-id="cd370-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cd370-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd370-132">id</span><span class="sxs-lookup"><span data-stu-id="cd370-132">id</span></span>|<span data-ttu-id="cd370-133">Строка</span><span class="sxs-lookup"><span data-stu-id="cd370-133">String</span></span>|<span data-ttu-id="cd370-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cd370-134">Key of the entity.</span></span> <span data-ttu-id="cd370-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cd370-136">displayName</span></span>|<span data-ttu-id="cd370-137">Строка</span><span class="sxs-lookup"><span data-stu-id="cd370-137">String</span></span>|<span data-ttu-id="cd370-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="cd370-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cd370-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-140">description</span><span class="sxs-lookup"><span data-stu-id="cd370-140">description</span></span>|<span data-ttu-id="cd370-141">Строка</span><span class="sxs-lookup"><span data-stu-id="cd370-141">String</span></span>|<span data-ttu-id="cd370-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="cd370-142">The description of the app.</span></span> <span data-ttu-id="cd370-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-144">publisher</span><span class="sxs-lookup"><span data-stu-id="cd370-144">publisher</span></span>|<span data-ttu-id="cd370-145">String</span><span class="sxs-lookup"><span data-stu-id="cd370-145">String</span></span>|<span data-ttu-id="cd370-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="cd370-146">The publisher of the app.</span></span> <span data-ttu-id="cd370-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cd370-148">largeIcon</span></span>|[<span data-ttu-id="cd370-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cd370-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cd370-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="cd370-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cd370-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd370-152">createdDateTime</span></span>|<span data-ttu-id="cd370-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd370-153">DateTimeOffset</span></span>|<span data-ttu-id="cd370-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="cd370-154">The date and time the app was created.</span></span> <span data-ttu-id="cd370-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd370-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cd370-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd370-157">DateTimeOffset</span></span>|<span data-ttu-id="cd370-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="cd370-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cd370-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cd370-160">isFeatured</span></span>|<span data-ttu-id="cd370-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd370-161">Boolean</span></span>|<span data-ttu-id="cd370-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cd370-163">privacyInformationUrl</span></span>|<span data-ttu-id="cd370-164">String</span><span class="sxs-lookup"><span data-stu-id="cd370-164">String</span></span>|<span data-ttu-id="cd370-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cd370-165">The privacy statement Url.</span></span> <span data-ttu-id="cd370-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cd370-167">informationUrl</span></span>|<span data-ttu-id="cd370-168">String</span><span class="sxs-lookup"><span data-stu-id="cd370-168">String</span></span>|<span data-ttu-id="cd370-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="cd370-169">The more information Url.</span></span> <span data-ttu-id="cd370-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-171">owner</span><span class="sxs-lookup"><span data-stu-id="cd370-171">owner</span></span>|<span data-ttu-id="cd370-172">String</span><span class="sxs-lookup"><span data-stu-id="cd370-172">String</span></span>|<span data-ttu-id="cd370-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="cd370-173">The owner of the app.</span></span> <span data-ttu-id="cd370-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-175">developer</span><span class="sxs-lookup"><span data-stu-id="cd370-175">developer</span></span>|<span data-ttu-id="cd370-176">String</span><span class="sxs-lookup"><span data-stu-id="cd370-176">String</span></span>|<span data-ttu-id="cd370-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="cd370-177">The developer of the app.</span></span> <span data-ttu-id="cd370-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-179">notes</span><span class="sxs-lookup"><span data-stu-id="cd370-179">notes</span></span>|<span data-ttu-id="cd370-180">String</span><span class="sxs-lookup"><span data-stu-id="cd370-180">String</span></span>|<span data-ttu-id="cd370-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="cd370-181">Notes for the app.</span></span> <span data-ttu-id="cd370-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="cd370-183">uploadState</span></span>|<span data-ttu-id="cd370-184">Int32</span><span class="sxs-lookup"><span data-stu-id="cd370-184">Int32</span></span>|<span data-ttu-id="cd370-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="cd370-185">The upload state.</span></span> <span data-ttu-id="cd370-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="cd370-187">publishingState</span></span>|[<span data-ttu-id="cd370-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="cd370-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cd370-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="cd370-189">The publishing state for the app.</span></span> <span data-ttu-id="cd370-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="cd370-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cd370-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="cd370-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cd370-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cd370-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cd370-193">isAssigned</span></span>|<span data-ttu-id="cd370-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd370-194">Boolean</span></span>|<span data-ttu-id="cd370-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="cd370-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cd370-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cd370-197">roleScopeTagIds</span></span>|<span data-ttu-id="cd370-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cd370-198">String collection</span></span>|<span data-ttu-id="cd370-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="cd370-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cd370-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="cd370-201">dependentAppCount</span></span>|<span data-ttu-id="cd370-202">Int32</span><span class="sxs-lookup"><span data-stu-id="cd370-202">Int32</span></span>|<span data-ttu-id="cd370-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="cd370-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="cd370-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cd370-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cd370-205">packageId</span><span class="sxs-lookup"><span data-stu-id="cd370-205">packageId</span></span>|<span data-ttu-id="cd370-206">String</span><span class="sxs-lookup"><span data-stu-id="cd370-206">String</span></span>|<span data-ttu-id="cd370-207">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="cd370-207">The package identifier.</span></span> <span data-ttu-id="cd370-208">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd370-208">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="cd370-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="cd370-209">appIdentifier</span></span>|<span data-ttu-id="cd370-210">String</span><span class="sxs-lookup"><span data-stu-id="cd370-210">String</span></span>|<span data-ttu-id="cd370-211">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="cd370-211">The Identity Name.</span></span> <span data-ttu-id="cd370-212">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd370-212">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="cd370-213">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cd370-213">usedLicenseCount</span></span>|<span data-ttu-id="cd370-214">Int32</span><span class="sxs-lookup"><span data-stu-id="cd370-214">Int32</span></span>|<span data-ttu-id="cd370-215">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="cd370-215">The number of VPP licenses in use.</span></span> <span data-ttu-id="cd370-216">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd370-216">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="cd370-217">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="cd370-217">totalLicenseCount</span></span>|<span data-ttu-id="cd370-218">Int32</span><span class="sxs-lookup"><span data-stu-id="cd370-218">Int32</span></span>|<span data-ttu-id="cd370-219">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="cd370-219">The total number of VPP licenses.</span></span> <span data-ttu-id="cd370-220">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd370-220">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="cd370-221">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="cd370-221">appStoreUrl</span></span>|<span data-ttu-id="cd370-222">String</span><span class="sxs-lookup"><span data-stu-id="cd370-222">String</span></span>|<span data-ttu-id="cd370-223">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="cd370-223">The Play for Work Store app URL.</span></span> <span data-ttu-id="cd370-224">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd370-224">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="cd370-225">Частный</span><span class="sxs-lookup"><span data-stu-id="cd370-225">isPrivate</span></span>|<span data-ttu-id="cd370-226">Логический</span><span class="sxs-lookup"><span data-stu-id="cd370-226">Boolean</span></span>|<span data-ttu-id="cd370-227">Указывает, доступно ли приложение только для указанных пользователей предприятия.</span><span class="sxs-lookup"><span data-stu-id="cd370-227">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="cd370-228">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd370-228">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="cd370-229">иссистемапп</span><span class="sxs-lookup"><span data-stu-id="cd370-229">isSystemApp</span></span>|<span data-ttu-id="cd370-230">Логический</span><span class="sxs-lookup"><span data-stu-id="cd370-230">Boolean</span></span>|<span data-ttu-id="cd370-231">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="cd370-231">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="cd370-232">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd370-232">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="cd370-233">суппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="cd370-233">supportsOemConfig</span></span>|<span data-ttu-id="cd370-234">Логический</span><span class="sxs-lookup"><span data-stu-id="cd370-234">Boolean</span></span>|<span data-ttu-id="cd370-235">Поддерживает ли это приложение политику Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="cd370-235">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="cd370-236">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="cd370-236">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="cd370-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd370-237">Response</span></span>
<span data-ttu-id="cd370-238">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd370-238">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd370-239">Пример</span><span class="sxs-lookup"><span data-stu-id="cd370-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd370-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd370-240">Request</span></span>
<span data-ttu-id="cd370-241">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd370-241">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cd370-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd370-242">Response</span></span>
<span data-ttu-id="cd370-p127">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd370-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






