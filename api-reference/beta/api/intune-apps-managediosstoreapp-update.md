---
title: Обновление managedIOSStoreApp
description: Обновляет свойства объекта managedIOSStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b04b685fe84f0fce11e56d93e580b4fafba97776
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39936383"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="9ba59-103">Обновление managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="9ba59-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="9ba59-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ba59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ba59-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ba59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ba59-106">Обновляет свойства объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-106">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ba59-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9ba59-107">Prerequisites</span></span>
<span data-ttu-id="9ba59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ba59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ba59-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ba59-110">Permission type</span></span>|<span data-ttu-id="9ba59-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ba59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ba59-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ba59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ba59-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ba59-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ba59-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ba59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ba59-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ba59-115">Not supported.</span></span>|
|<span data-ttu-id="9ba59-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ba59-116">Application</span></span>|<span data-ttu-id="9ba59-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ba59-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ba59-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ba59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9ba59-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9ba59-119">Request headers</span></span>
|<span data-ttu-id="9ba59-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ba59-120">Header</span></span>|<span data-ttu-id="9ba59-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9ba59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ba59-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ba59-122">Authorization</span></span>|<span data-ttu-id="9ba59-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ba59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ba59-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9ba59-124">Accept</span></span>|<span data-ttu-id="9ba59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ba59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ba59-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9ba59-126">Request body</span></span>
<span data-ttu-id="9ba59-127">В теле запроса добавьте представление объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ba59-127">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="9ba59-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-128">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="9ba59-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ba59-129">Property</span></span>|<span data-ttu-id="9ba59-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9ba59-130">Type</span></span>|<span data-ttu-id="9ba59-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9ba59-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ba59-132">id</span><span class="sxs-lookup"><span data-stu-id="9ba59-132">id</span></span>|<span data-ttu-id="9ba59-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9ba59-133">String</span></span>|<span data-ttu-id="9ba59-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9ba59-134">Key of the entity.</span></span> <span data-ttu-id="9ba59-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9ba59-136">displayName</span></span>|<span data-ttu-id="9ba59-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9ba59-137">String</span></span>|<span data-ttu-id="9ba59-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9ba59-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9ba59-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-140">description</span><span class="sxs-lookup"><span data-stu-id="9ba59-140">description</span></span>|<span data-ttu-id="9ba59-141">Строка</span><span class="sxs-lookup"><span data-stu-id="9ba59-141">String</span></span>|<span data-ttu-id="9ba59-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-142">The description of the app.</span></span> <span data-ttu-id="9ba59-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9ba59-144">publisher</span></span>|<span data-ttu-id="9ba59-145">Строка</span><span class="sxs-lookup"><span data-stu-id="9ba59-145">String</span></span>|<span data-ttu-id="9ba59-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-146">The publisher of the app.</span></span> <span data-ttu-id="9ba59-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9ba59-148">largeIcon</span></span>|[<span data-ttu-id="9ba59-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ba59-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9ba59-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9ba59-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9ba59-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ba59-152">createdDateTime</span></span>|<span data-ttu-id="9ba59-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ba59-153">DateTimeOffset</span></span>|<span data-ttu-id="9ba59-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-154">The date and time the app was created.</span></span> <span data-ttu-id="9ba59-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ba59-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9ba59-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ba59-157">DateTimeOffset</span></span>|<span data-ttu-id="9ba59-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9ba59-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9ba59-160">isFeatured</span></span>|<span data-ttu-id="9ba59-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ba59-161">Boolean</span></span>|<span data-ttu-id="9ba59-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9ba59-163">privacyInformationUrl</span></span>|<span data-ttu-id="9ba59-164">Строка</span><span class="sxs-lookup"><span data-stu-id="9ba59-164">String</span></span>|<span data-ttu-id="9ba59-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9ba59-165">The privacy statement Url.</span></span> <span data-ttu-id="9ba59-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9ba59-167">informationUrl</span></span>|<span data-ttu-id="9ba59-168">Строка</span><span class="sxs-lookup"><span data-stu-id="9ba59-168">String</span></span>|<span data-ttu-id="9ba59-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9ba59-169">The more information Url.</span></span> <span data-ttu-id="9ba59-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-171">owner</span><span class="sxs-lookup"><span data-stu-id="9ba59-171">owner</span></span>|<span data-ttu-id="9ba59-172">String</span><span class="sxs-lookup"><span data-stu-id="9ba59-172">String</span></span>|<span data-ttu-id="9ba59-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-173">The owner of the app.</span></span> <span data-ttu-id="9ba59-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-175">developer</span><span class="sxs-lookup"><span data-stu-id="9ba59-175">developer</span></span>|<span data-ttu-id="9ba59-176">Строка</span><span class="sxs-lookup"><span data-stu-id="9ba59-176">String</span></span>|<span data-ttu-id="9ba59-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-177">The developer of the app.</span></span> <span data-ttu-id="9ba59-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-179">notes</span><span class="sxs-lookup"><span data-stu-id="9ba59-179">notes</span></span>|<span data-ttu-id="9ba59-180">Строка</span><span class="sxs-lookup"><span data-stu-id="9ba59-180">String</span></span>|<span data-ttu-id="9ba59-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-181">Notes for the app.</span></span> <span data-ttu-id="9ba59-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9ba59-183">uploadState</span></span>|<span data-ttu-id="9ba59-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9ba59-184">Int32</span></span>|<span data-ttu-id="9ba59-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="9ba59-185">The upload state.</span></span> <span data-ttu-id="9ba59-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9ba59-187">publishingState</span></span>|[<span data-ttu-id="9ba59-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9ba59-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9ba59-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-189">The publishing state for the app.</span></span> <span data-ttu-id="9ba59-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9ba59-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9ba59-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="9ba59-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9ba59-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9ba59-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9ba59-193">isAssigned</span></span>|<span data-ttu-id="9ba59-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ba59-194">Boolean</span></span>|<span data-ttu-id="9ba59-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="9ba59-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9ba59-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ba59-197">roleScopeTagIds</span></span>|<span data-ttu-id="9ba59-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9ba59-198">String collection</span></span>|<span data-ttu-id="9ba59-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9ba59-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="9ba59-201">dependentAppCount</span></span>|<span data-ttu-id="9ba59-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9ba59-202">Int32</span></span>|<span data-ttu-id="9ba59-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9ba59-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba59-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="9ba59-205">appAvailability</span></span>|[<span data-ttu-id="9ba59-206">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="9ba59-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="9ba59-207">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-207">The Application's availability.</span></span> <span data-ttu-id="9ba59-208">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba59-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="9ba59-209">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="9ba59-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="9ba59-210">version</span><span class="sxs-lookup"><span data-stu-id="9ba59-210">version</span></span>|<span data-ttu-id="9ba59-211">String</span><span class="sxs-lookup"><span data-stu-id="9ba59-211">String</span></span>|<span data-ttu-id="9ba59-212">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-212">The Application's version.</span></span> <span data-ttu-id="9ba59-213">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ba59-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="9ba59-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="9ba59-214">bundleId</span></span>|<span data-ttu-id="9ba59-215">Строка</span><span class="sxs-lookup"><span data-stu-id="9ba59-215">String</span></span>|<span data-ttu-id="9ba59-216">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba59-216">The app's Bundle ID.</span></span>|
|<span data-ttu-id="9ba59-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9ba59-217">appStoreUrl</span></span>|<span data-ttu-id="9ba59-218">String</span><span class="sxs-lookup"><span data-stu-id="9ba59-218">String</span></span>|<span data-ttu-id="9ba59-219">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="9ba59-219">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="9ba59-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9ba59-220">applicableDeviceType</span></span>|[<span data-ttu-id="9ba59-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9ba59-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="9ba59-222">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="9ba59-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="9ba59-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9ba59-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9ba59-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9ba59-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="9ba59-225">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="9ba59-225">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="9ba59-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ba59-226">Response</span></span>
<span data-ttu-id="9ba59-227">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9ba59-227">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ba59-228">Пример</span><span class="sxs-lookup"><span data-stu-id="9ba59-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ba59-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ba59-229">Request</span></span>
<span data-ttu-id="9ba59-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ba59-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ba59-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ba59-231">Response</span></span>
<span data-ttu-id="9ba59-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ba59-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





