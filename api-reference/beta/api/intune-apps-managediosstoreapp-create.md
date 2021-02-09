---
title: Create managedIOSStoreApp
description: Создание объекта managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a8c3a888900da2e6d170085a630bc7de1e448753
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155442"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="8dc04-103">Create managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="8dc04-103">Create managedIOSStoreApp</span></span>

<span data-ttu-id="8dc04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dc04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8dc04-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dc04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dc04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8dc04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dc04-107">Создание объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-107">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8dc04-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8dc04-108">Prerequisites</span></span>
<span data-ttu-id="8dc04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dc04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dc04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dc04-111">Permission type</span></span>|<span data-ttu-id="8dc04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dc04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dc04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dc04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8dc04-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dc04-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8dc04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dc04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dc04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dc04-116">Not supported.</span></span>|
|<span data-ttu-id="8dc04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8dc04-117">Application</span></span>|<span data-ttu-id="8dc04-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dc04-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dc04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dc04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8dc04-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8dc04-120">Request headers</span></span>
|<span data-ttu-id="8dc04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8dc04-121">Header</span></span>|<span data-ttu-id="8dc04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8dc04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8dc04-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dc04-123">Authorization</span></span>|<span data-ttu-id="8dc04-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dc04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8dc04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8dc04-125">Accept</span></span>|<span data-ttu-id="8dc04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8dc04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dc04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dc04-127">Request body</span></span>
<span data-ttu-id="8dc04-128">В теле запроса добавьте представление объекта managedIOSStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8dc04-128">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="8dc04-129">Ниже показаны свойства, которые необходимо указывать при создании объекта managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="8dc04-129">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="8dc04-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dc04-130">Property</span></span>|<span data-ttu-id="8dc04-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8dc04-131">Type</span></span>|<span data-ttu-id="8dc04-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8dc04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dc04-133">id</span><span class="sxs-lookup"><span data-stu-id="8dc04-133">id</span></span>|<span data-ttu-id="8dc04-134">String</span><span class="sxs-lookup"><span data-stu-id="8dc04-134">String</span></span>|<span data-ttu-id="8dc04-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8dc04-135">Key of the entity.</span></span> <span data-ttu-id="8dc04-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8dc04-137">displayName</span></span>|<span data-ttu-id="8dc04-138">String</span><span class="sxs-lookup"><span data-stu-id="8dc04-138">String</span></span>|<span data-ttu-id="8dc04-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="8dc04-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8dc04-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-141">description</span><span class="sxs-lookup"><span data-stu-id="8dc04-141">description</span></span>|<span data-ttu-id="8dc04-142">String</span><span class="sxs-lookup"><span data-stu-id="8dc04-142">String</span></span>|<span data-ttu-id="8dc04-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-143">The description of the app.</span></span> <span data-ttu-id="8dc04-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8dc04-145">publisher</span></span>|<span data-ttu-id="8dc04-146">String</span><span class="sxs-lookup"><span data-stu-id="8dc04-146">String</span></span>|<span data-ttu-id="8dc04-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-147">The publisher of the app.</span></span> <span data-ttu-id="8dc04-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8dc04-149">largeIcon</span></span>|[<span data-ttu-id="8dc04-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8dc04-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8dc04-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="8dc04-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8dc04-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8dc04-153">createdDateTime</span></span>|<span data-ttu-id="8dc04-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dc04-154">DateTimeOffset</span></span>|<span data-ttu-id="8dc04-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-155">The date and time the app was created.</span></span> <span data-ttu-id="8dc04-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8dc04-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8dc04-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dc04-158">DateTimeOffset</span></span>|<span data-ttu-id="8dc04-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8dc04-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8dc04-161">isFeatured</span></span>|<span data-ttu-id="8dc04-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dc04-162">Boolean</span></span>|<span data-ttu-id="8dc04-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8dc04-164">privacyInformationUrl</span></span>|<span data-ttu-id="8dc04-165">String</span><span class="sxs-lookup"><span data-stu-id="8dc04-165">String</span></span>|<span data-ttu-id="8dc04-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8dc04-166">The privacy statement Url.</span></span> <span data-ttu-id="8dc04-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8dc04-168">informationUrl</span></span>|<span data-ttu-id="8dc04-169">String</span><span class="sxs-lookup"><span data-stu-id="8dc04-169">String</span></span>|<span data-ttu-id="8dc04-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="8dc04-170">The more information Url.</span></span> <span data-ttu-id="8dc04-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-172">owner</span><span class="sxs-lookup"><span data-stu-id="8dc04-172">owner</span></span>|<span data-ttu-id="8dc04-173">String</span><span class="sxs-lookup"><span data-stu-id="8dc04-173">String</span></span>|<span data-ttu-id="8dc04-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-174">The owner of the app.</span></span> <span data-ttu-id="8dc04-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-176">developer</span><span class="sxs-lookup"><span data-stu-id="8dc04-176">developer</span></span>|<span data-ttu-id="8dc04-177">String</span><span class="sxs-lookup"><span data-stu-id="8dc04-177">String</span></span>|<span data-ttu-id="8dc04-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-178">The developer of the app.</span></span> <span data-ttu-id="8dc04-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-180">notes</span><span class="sxs-lookup"><span data-stu-id="8dc04-180">notes</span></span>|<span data-ttu-id="8dc04-181">String</span><span class="sxs-lookup"><span data-stu-id="8dc04-181">String</span></span>|<span data-ttu-id="8dc04-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-182">Notes for the app.</span></span> <span data-ttu-id="8dc04-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8dc04-184">uploadState</span></span>|<span data-ttu-id="8dc04-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc04-185">Int32</span></span>|<span data-ttu-id="8dc04-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="8dc04-186">The upload state.</span></span> <span data-ttu-id="8dc04-187">Возможные значения: 0- `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="8dc04-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="8dc04-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="8dc04-189">publishingState</span></span>|[<span data-ttu-id="8dc04-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8dc04-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8dc04-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-191">The publishing state for the app.</span></span> <span data-ttu-id="8dc04-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="8dc04-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8dc04-193">Наследуется от [mobileApp.](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8dc04-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8dc04-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8dc04-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8dc04-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8dc04-195">isAssigned</span></span>|<span data-ttu-id="8dc04-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dc04-196">Boolean</span></span>|<span data-ttu-id="8dc04-197">Значение, указывающее, назначено ли приложению хотя бы одна группа.</span><span class="sxs-lookup"><span data-stu-id="8dc04-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8dc04-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8dc04-199">roleScopeTagIds</span></span>|<span data-ttu-id="8dc04-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8dc04-200">String collection</span></span>|<span data-ttu-id="8dc04-201">Список ид тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8dc04-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="8dc04-203">dependentAppCount</span></span>|<span data-ttu-id="8dc04-204">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc04-204">Int32</span></span>|<span data-ttu-id="8dc04-205">Общее количество зависимостей, которые есть у этого приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8dc04-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="8dc04-207">supersedingAppCount</span></span>|<span data-ttu-id="8dc04-208">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc04-208">Int32</span></span>|<span data-ttu-id="8dc04-209">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="8dc04-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="8dc04-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="8dc04-211">supersededAppCount</span></span>|<span data-ttu-id="8dc04-212">Int32</span><span class="sxs-lookup"><span data-stu-id="8dc04-212">Int32</span></span>|<span data-ttu-id="8dc04-213">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="8dc04-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="8dc04-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dc04-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dc04-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="8dc04-215">appAvailability</span></span>|[<span data-ttu-id="8dc04-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="8dc04-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="8dc04-217">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-217">The Application's availability.</span></span> <span data-ttu-id="8dc04-218">Наследуется от [managedApp.](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8dc04-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="8dc04-219">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="8dc04-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="8dc04-220">version</span><span class="sxs-lookup"><span data-stu-id="8dc04-220">version</span></span>|<span data-ttu-id="8dc04-221">String</span><span class="sxs-lookup"><span data-stu-id="8dc04-221">String</span></span>|<span data-ttu-id="8dc04-222">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-222">The Application's version.</span></span> <span data-ttu-id="8dc04-223">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8dc04-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="8dc04-224">bundleId</span><span class="sxs-lookup"><span data-stu-id="8dc04-224">bundleId</span></span>|<span data-ttu-id="8dc04-225">String</span><span class="sxs-lookup"><span data-stu-id="8dc04-225">String</span></span>|<span data-ttu-id="8dc04-226">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="8dc04-226">The app's Bundle ID.</span></span>|
|<span data-ttu-id="8dc04-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8dc04-227">appStoreUrl</span></span>|<span data-ttu-id="8dc04-228">String</span><span class="sxs-lookup"><span data-stu-id="8dc04-228">String</span></span>|<span data-ttu-id="8dc04-229">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="8dc04-229">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="8dc04-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="8dc04-230">applicableDeviceType</span></span>|[<span data-ttu-id="8dc04-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="8dc04-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="8dc04-232">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="8dc04-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="8dc04-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8dc04-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8dc04-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8dc04-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="8dc04-235">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="8dc04-235">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="8dc04-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="8dc04-236">Response</span></span>
<span data-ttu-id="8dc04-237">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8dc04-237">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dc04-238">Пример</span><span class="sxs-lookup"><span data-stu-id="8dc04-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="8dc04-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dc04-239">Request</span></span>
<span data-ttu-id="8dc04-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dc04-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1315

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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
    "v13_0": true,
    "v14_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="8dc04-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dc04-241">Response</span></span>
<span data-ttu-id="8dc04-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8dc04-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1487

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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
    "v13_0": true,
    "v14_0": true
  }
}
```




