---
title: Обновление managedIOSStoreApp
description: Обновляет свойства объекта managedIOSStoreApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c6729298cabdd6625cec4d80f91397a4eac6882
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815361"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="3e188-103">Обновление managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="3e188-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="3e188-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e188-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e188-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e188-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e188-106">Обновляет свойства объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-106">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e188-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3e188-107">Prerequisites</span></span>
<span data-ttu-id="3e188-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e188-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e188-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e188-110">Permission type</span></span>|<span data-ttu-id="3e188-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e188-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e188-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e188-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e188-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e188-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3e188-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e188-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e188-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e188-115">Not supported.</span></span>|
|<span data-ttu-id="3e188-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3e188-116">Application</span></span>|<span data-ttu-id="3e188-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e188-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e188-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e188-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="3e188-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3e188-119">Request headers</span></span>
|<span data-ttu-id="3e188-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e188-120">Header</span></span>|<span data-ttu-id="3e188-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3e188-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e188-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e188-122">Authorization</span></span>|<span data-ttu-id="3e188-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e188-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e188-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3e188-124">Accept</span></span>|<span data-ttu-id="3e188-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3e188-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e188-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e188-126">Request body</span></span>
<span data-ttu-id="3e188-127">В теле запроса добавьте представление объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e188-127">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="3e188-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-128">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="3e188-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e188-129">Property</span></span>|<span data-ttu-id="3e188-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3e188-130">Type</span></span>|<span data-ttu-id="3e188-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3e188-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e188-132">id</span><span class="sxs-lookup"><span data-stu-id="3e188-132">id</span></span>|<span data-ttu-id="3e188-133">Строка</span><span class="sxs-lookup"><span data-stu-id="3e188-133">String</span></span>|<span data-ttu-id="3e188-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3e188-134">Key of the entity.</span></span> <span data-ttu-id="3e188-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3e188-136">displayName</span></span>|<span data-ttu-id="3e188-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3e188-137">String</span></span>|<span data-ttu-id="3e188-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="3e188-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3e188-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-140">description</span><span class="sxs-lookup"><span data-stu-id="3e188-140">description</span></span>|<span data-ttu-id="3e188-141">String</span><span class="sxs-lookup"><span data-stu-id="3e188-141">String</span></span>|<span data-ttu-id="3e188-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-142">The description of the app.</span></span> <span data-ttu-id="3e188-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-144">publisher</span><span class="sxs-lookup"><span data-stu-id="3e188-144">publisher</span></span>|<span data-ttu-id="3e188-145">String</span><span class="sxs-lookup"><span data-stu-id="3e188-145">String</span></span>|<span data-ttu-id="3e188-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-146">The publisher of the app.</span></span> <span data-ttu-id="3e188-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3e188-148">largeIcon</span></span>|[<span data-ttu-id="3e188-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3e188-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3e188-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="3e188-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3e188-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e188-152">createdDateTime</span></span>|<span data-ttu-id="3e188-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e188-153">DateTimeOffset</span></span>|<span data-ttu-id="3e188-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-154">The date and time the app was created.</span></span> <span data-ttu-id="3e188-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e188-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3e188-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e188-157">DateTimeOffset</span></span>|<span data-ttu-id="3e188-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3e188-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3e188-160">isFeatured</span></span>|<span data-ttu-id="3e188-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e188-161">Boolean</span></span>|<span data-ttu-id="3e188-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3e188-163">privacyInformationUrl</span></span>|<span data-ttu-id="3e188-164">String</span><span class="sxs-lookup"><span data-stu-id="3e188-164">String</span></span>|<span data-ttu-id="3e188-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3e188-165">The privacy statement Url.</span></span> <span data-ttu-id="3e188-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3e188-167">informationUrl</span></span>|<span data-ttu-id="3e188-168">String</span><span class="sxs-lookup"><span data-stu-id="3e188-168">String</span></span>|<span data-ttu-id="3e188-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3e188-169">The more information Url.</span></span> <span data-ttu-id="3e188-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-171">owner</span><span class="sxs-lookup"><span data-stu-id="3e188-171">owner</span></span>|<span data-ttu-id="3e188-172">String</span><span class="sxs-lookup"><span data-stu-id="3e188-172">String</span></span>|<span data-ttu-id="3e188-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-173">The owner of the app.</span></span> <span data-ttu-id="3e188-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-175">developer</span><span class="sxs-lookup"><span data-stu-id="3e188-175">developer</span></span>|<span data-ttu-id="3e188-176">String</span><span class="sxs-lookup"><span data-stu-id="3e188-176">String</span></span>|<span data-ttu-id="3e188-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-177">The developer of the app.</span></span> <span data-ttu-id="3e188-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-179">notes</span><span class="sxs-lookup"><span data-stu-id="3e188-179">notes</span></span>|<span data-ttu-id="3e188-180">String</span><span class="sxs-lookup"><span data-stu-id="3e188-180">String</span></span>|<span data-ttu-id="3e188-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-181">Notes for the app.</span></span> <span data-ttu-id="3e188-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="3e188-183">uploadState</span></span>|<span data-ttu-id="3e188-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3e188-184">Int32</span></span>|<span data-ttu-id="3e188-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="3e188-185">The upload state.</span></span> <span data-ttu-id="3e188-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="3e188-187">publishingState</span></span>|[<span data-ttu-id="3e188-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="3e188-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3e188-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-189">The publishing state for the app.</span></span> <span data-ttu-id="3e188-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="3e188-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3e188-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="3e188-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3e188-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3e188-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3e188-193">isAssigned</span></span>|<span data-ttu-id="3e188-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e188-194">Boolean</span></span>|<span data-ttu-id="3e188-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="3e188-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3e188-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3e188-197">roleScopeTagIds</span></span>|<span data-ttu-id="3e188-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3e188-198">String collection</span></span>|<span data-ttu-id="3e188-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3e188-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="3e188-201">dependentAppCount</span></span>|<span data-ttu-id="3e188-202">Int32</span><span class="sxs-lookup"><span data-stu-id="3e188-202">Int32</span></span>|<span data-ttu-id="3e188-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="3e188-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3e188-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="3e188-205">appAvailability</span></span>|[<span data-ttu-id="3e188-206">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="3e188-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="3e188-207">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-207">The Application's availability.</span></span> <span data-ttu-id="3e188-208">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e188-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="3e188-209">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="3e188-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="3e188-210">version</span><span class="sxs-lookup"><span data-stu-id="3e188-210">version</span></span>|<span data-ttu-id="3e188-211">String</span><span class="sxs-lookup"><span data-stu-id="3e188-211">String</span></span>|<span data-ttu-id="3e188-212">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-212">The Application's version.</span></span> <span data-ttu-id="3e188-213">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="3e188-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="3e188-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="3e188-214">bundleId</span></span>|<span data-ttu-id="3e188-215">String</span><span class="sxs-lookup"><span data-stu-id="3e188-215">String</span></span>|<span data-ttu-id="3e188-216">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="3e188-216">The app's Bundle ID.</span></span>|
|<span data-ttu-id="3e188-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3e188-217">appStoreUrl</span></span>|<span data-ttu-id="3e188-218">String</span><span class="sxs-lookup"><span data-stu-id="3e188-218">String</span></span>|<span data-ttu-id="3e188-219">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="3e188-219">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="3e188-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="3e188-220">applicableDeviceType</span></span>|[<span data-ttu-id="3e188-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3e188-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="3e188-222">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="3e188-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="3e188-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3e188-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3e188-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3e188-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="3e188-225">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="3e188-225">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="3e188-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e188-226">Response</span></span>
<span data-ttu-id="3e188-227">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3e188-227">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e188-228">Пример</span><span class="sxs-lookup"><span data-stu-id="3e188-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e188-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e188-229">Request</span></span>
<span data-ttu-id="3e188-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e188-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1238

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="3e188-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e188-231">Response</span></span>
<span data-ttu-id="3e188-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e188-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1410

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
    "v13_0": true
  }
}
```




