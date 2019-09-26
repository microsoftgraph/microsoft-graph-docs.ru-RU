---
title: Create managedIOSStoreApp
description: Создание объекта managedIOSStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d268ac5526fa2ef96beacd1aa3d80c87e99005f9
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37172928"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="ad244-103">Create managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="ad244-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="ad244-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad244-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad244-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad244-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad244-106">Создание объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-106">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad244-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ad244-107">Prerequisites</span></span>
<span data-ttu-id="ad244-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad244-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad244-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad244-110">Permission type</span></span>|<span data-ttu-id="ad244-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad244-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad244-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad244-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad244-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad244-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad244-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad244-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad244-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad244-115">Not supported.</span></span>|
|<span data-ttu-id="ad244-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad244-116">Application</span></span>|<span data-ttu-id="ad244-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad244-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad244-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad244-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ad244-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad244-119">Request headers</span></span>
|<span data-ttu-id="ad244-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad244-120">Header</span></span>|<span data-ttu-id="ad244-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ad244-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad244-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad244-122">Authorization</span></span>|<span data-ttu-id="ad244-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad244-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad244-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ad244-124">Accept</span></span>|<span data-ttu-id="ad244-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad244-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad244-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad244-126">Request body</span></span>
<span data-ttu-id="ad244-127">В теле запроса добавьте представление объекта managedIOSStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad244-127">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="ad244-128">Ниже показаны свойства, которые необходимо указывать при создании объекта managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="ad244-128">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="ad244-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad244-129">Property</span></span>|<span data-ttu-id="ad244-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ad244-130">Type</span></span>|<span data-ttu-id="ad244-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ad244-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad244-132">id</span><span class="sxs-lookup"><span data-stu-id="ad244-132">id</span></span>|<span data-ttu-id="ad244-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ad244-133">String</span></span>|<span data-ttu-id="ad244-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ad244-134">Key of the entity.</span></span> <span data-ttu-id="ad244-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ad244-136">displayName</span></span>|<span data-ttu-id="ad244-137">Строка</span><span class="sxs-lookup"><span data-stu-id="ad244-137">String</span></span>|<span data-ttu-id="ad244-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ad244-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ad244-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-140">description</span><span class="sxs-lookup"><span data-stu-id="ad244-140">description</span></span>|<span data-ttu-id="ad244-141">String.</span><span class="sxs-lookup"><span data-stu-id="ad244-141">String</span></span>|<span data-ttu-id="ad244-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-142">The description of the app.</span></span> <span data-ttu-id="ad244-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-144">publisher</span><span class="sxs-lookup"><span data-stu-id="ad244-144">publisher</span></span>|<span data-ttu-id="ad244-145">String.</span><span class="sxs-lookup"><span data-stu-id="ad244-145">String</span></span>|<span data-ttu-id="ad244-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-146">The publisher of the app.</span></span> <span data-ttu-id="ad244-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ad244-148">largeIcon</span></span>|[<span data-ttu-id="ad244-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ad244-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ad244-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ad244-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ad244-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad244-152">createdDateTime</span></span>|<span data-ttu-id="ad244-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad244-153">DateTimeOffset</span></span>|<span data-ttu-id="ad244-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-154">The date and time the app was created.</span></span> <span data-ttu-id="ad244-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad244-156">lastModifiedDateTime</span></span>|<span data-ttu-id="ad244-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad244-157">DateTimeOffset</span></span>|<span data-ttu-id="ad244-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-158">The date and time the app was last modified.</span></span> <span data-ttu-id="ad244-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ad244-160">isFeatured</span></span>|<span data-ttu-id="ad244-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad244-161">Boolean</span></span>|<span data-ttu-id="ad244-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ad244-163">privacyInformationUrl</span></span>|<span data-ttu-id="ad244-164">String.</span><span class="sxs-lookup"><span data-stu-id="ad244-164">String</span></span>|<span data-ttu-id="ad244-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ad244-165">The privacy statement Url.</span></span> <span data-ttu-id="ad244-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ad244-167">informationUrl</span></span>|<span data-ttu-id="ad244-168">String.</span><span class="sxs-lookup"><span data-stu-id="ad244-168">String</span></span>|<span data-ttu-id="ad244-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ad244-169">The more information Url.</span></span> <span data-ttu-id="ad244-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-171">owner</span><span class="sxs-lookup"><span data-stu-id="ad244-171">owner</span></span>|<span data-ttu-id="ad244-172">String</span><span class="sxs-lookup"><span data-stu-id="ad244-172">String</span></span>|<span data-ttu-id="ad244-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-173">The owner of the app.</span></span> <span data-ttu-id="ad244-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-175">developer</span><span class="sxs-lookup"><span data-stu-id="ad244-175">developer</span></span>|<span data-ttu-id="ad244-176">String.</span><span class="sxs-lookup"><span data-stu-id="ad244-176">String</span></span>|<span data-ttu-id="ad244-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-177">The developer of the app.</span></span> <span data-ttu-id="ad244-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-179">notes</span><span class="sxs-lookup"><span data-stu-id="ad244-179">notes</span></span>|<span data-ttu-id="ad244-180">String.</span><span class="sxs-lookup"><span data-stu-id="ad244-180">String</span></span>|<span data-ttu-id="ad244-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-181">Notes for the app.</span></span> <span data-ttu-id="ad244-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="ad244-183">uploadState</span></span>|<span data-ttu-id="ad244-184">Int32</span><span class="sxs-lookup"><span data-stu-id="ad244-184">Int32</span></span>|<span data-ttu-id="ad244-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="ad244-185">The upload state.</span></span> <span data-ttu-id="ad244-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="ad244-187">publishingState</span></span>|[<span data-ttu-id="ad244-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="ad244-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ad244-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-189">The publishing state for the app.</span></span> <span data-ttu-id="ad244-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ad244-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ad244-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ad244-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ad244-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ad244-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ad244-193">isAssigned</span></span>|<span data-ttu-id="ad244-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad244-194">Boolean</span></span>|<span data-ttu-id="ad244-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="ad244-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ad244-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ad244-197">roleScopeTagIds</span></span>|<span data-ttu-id="ad244-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ad244-198">String collection</span></span>|<span data-ttu-id="ad244-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ad244-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="ad244-201">dependentAppCount</span></span>|<span data-ttu-id="ad244-202">Int32</span><span class="sxs-lookup"><span data-stu-id="ad244-202">Int32</span></span>|<span data-ttu-id="ad244-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ad244-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad244-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="ad244-205">appAvailability</span></span>|[<span data-ttu-id="ad244-206">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="ad244-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="ad244-207">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-207">The Application's availability.</span></span> <span data-ttu-id="ad244-208">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad244-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="ad244-209">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="ad244-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="ad244-210">version</span><span class="sxs-lookup"><span data-stu-id="ad244-210">version</span></span>|<span data-ttu-id="ad244-211">String</span><span class="sxs-lookup"><span data-stu-id="ad244-211">String</span></span>|<span data-ttu-id="ad244-212">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-212">The Application's version.</span></span> <span data-ttu-id="ad244-213">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad244-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="ad244-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="ad244-214">bundleId</span></span>|<span data-ttu-id="ad244-215">String.</span><span class="sxs-lookup"><span data-stu-id="ad244-215">String</span></span>|<span data-ttu-id="ad244-216">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="ad244-216">The app's Bundle ID.</span></span>|
|<span data-ttu-id="ad244-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ad244-217">appStoreUrl</span></span>|<span data-ttu-id="ad244-218">String</span><span class="sxs-lookup"><span data-stu-id="ad244-218">String</span></span>|<span data-ttu-id="ad244-219">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="ad244-219">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="ad244-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ad244-220">applicableDeviceType</span></span>|[<span data-ttu-id="ad244-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ad244-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="ad244-222">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ad244-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="ad244-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ad244-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ad244-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ad244-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="ad244-225">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ad244-225">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="ad244-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad244-226">Response</span></span>
<span data-ttu-id="ad244-227">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ad244-227">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad244-228">Пример</span><span class="sxs-lookup"><span data-stu-id="ad244-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad244-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad244-229">Request</span></span>
<span data-ttu-id="ad244-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad244-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="ad244-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad244-231">Response</span></span>
<span data-ttu-id="ad244-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad244-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




