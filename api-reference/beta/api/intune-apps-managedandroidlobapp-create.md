---
title: Create managedAndroidLobApp
description: Создание объекта managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9eb57a81da2aaae1f7c9dae16cd1673eb045fe11
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157353"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="59302-103">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="59302-103">Create managedAndroidLobApp</span></span>

<span data-ttu-id="59302-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59302-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59302-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59302-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59302-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59302-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59302-107">Создание объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59302-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="59302-108">Prerequisites</span></span>
<span data-ttu-id="59302-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59302-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59302-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59302-111">Permission type</span></span>|<span data-ttu-id="59302-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="59302-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59302-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59302-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59302-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59302-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="59302-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59302-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59302-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59302-116">Not supported.</span></span>|
|<span data-ttu-id="59302-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59302-117">Application</span></span>|<span data-ttu-id="59302-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59302-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59302-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59302-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="59302-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="59302-120">Request headers</span></span>
|<span data-ttu-id="59302-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59302-121">Header</span></span>|<span data-ttu-id="59302-122">Значение</span><span class="sxs-lookup"><span data-stu-id="59302-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59302-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59302-123">Authorization</span></span>|<span data-ttu-id="59302-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59302-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59302-125">Accept</span><span class="sxs-lookup"><span data-stu-id="59302-125">Accept</span></span>|<span data-ttu-id="59302-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59302-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59302-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59302-127">Request body</span></span>
<span data-ttu-id="59302-128">В тексте запроса добавьте представление объекта managedAndroidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59302-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="59302-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="59302-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="59302-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="59302-130">Property</span></span>|<span data-ttu-id="59302-131">Тип</span><span class="sxs-lookup"><span data-stu-id="59302-131">Type</span></span>|<span data-ttu-id="59302-132">Описание</span><span class="sxs-lookup"><span data-stu-id="59302-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59302-133">id</span><span class="sxs-lookup"><span data-stu-id="59302-133">id</span></span>|<span data-ttu-id="59302-134">String</span><span class="sxs-lookup"><span data-stu-id="59302-134">String</span></span>|<span data-ttu-id="59302-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="59302-135">Key of the entity.</span></span> <span data-ttu-id="59302-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-137">displayName</span><span class="sxs-lookup"><span data-stu-id="59302-137">displayName</span></span>|<span data-ttu-id="59302-138">String</span><span class="sxs-lookup"><span data-stu-id="59302-138">String</span></span>|<span data-ttu-id="59302-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="59302-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="59302-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-141">description</span><span class="sxs-lookup"><span data-stu-id="59302-141">description</span></span>|<span data-ttu-id="59302-142">String</span><span class="sxs-lookup"><span data-stu-id="59302-142">String</span></span>|<span data-ttu-id="59302-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-143">The description of the app.</span></span> <span data-ttu-id="59302-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-145">publisher</span><span class="sxs-lookup"><span data-stu-id="59302-145">publisher</span></span>|<span data-ttu-id="59302-146">String</span><span class="sxs-lookup"><span data-stu-id="59302-146">String</span></span>|<span data-ttu-id="59302-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-147">The publisher of the app.</span></span> <span data-ttu-id="59302-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="59302-149">largeIcon</span></span>|[<span data-ttu-id="59302-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="59302-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="59302-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="59302-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="59302-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59302-153">createdDateTime</span></span>|<span data-ttu-id="59302-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59302-154">DateTimeOffset</span></span>|<span data-ttu-id="59302-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-155">The date and time the app was created.</span></span> <span data-ttu-id="59302-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59302-157">lastModifiedDateTime</span></span>|<span data-ttu-id="59302-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59302-158">DateTimeOffset</span></span>|<span data-ttu-id="59302-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-159">The date and time the app was last modified.</span></span> <span data-ttu-id="59302-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="59302-161">isFeatured</span></span>|<span data-ttu-id="59302-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="59302-162">Boolean</span></span>|<span data-ttu-id="59302-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="59302-164">privacyInformationUrl</span></span>|<span data-ttu-id="59302-165">String</span><span class="sxs-lookup"><span data-stu-id="59302-165">String</span></span>|<span data-ttu-id="59302-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="59302-166">The privacy statement Url.</span></span> <span data-ttu-id="59302-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="59302-168">informationUrl</span></span>|<span data-ttu-id="59302-169">String</span><span class="sxs-lookup"><span data-stu-id="59302-169">String</span></span>|<span data-ttu-id="59302-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="59302-170">The more information Url.</span></span> <span data-ttu-id="59302-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-172">owner</span><span class="sxs-lookup"><span data-stu-id="59302-172">owner</span></span>|<span data-ttu-id="59302-173">String</span><span class="sxs-lookup"><span data-stu-id="59302-173">String</span></span>|<span data-ttu-id="59302-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-174">The owner of the app.</span></span> <span data-ttu-id="59302-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-176">developer</span><span class="sxs-lookup"><span data-stu-id="59302-176">developer</span></span>|<span data-ttu-id="59302-177">String</span><span class="sxs-lookup"><span data-stu-id="59302-177">String</span></span>|<span data-ttu-id="59302-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-178">The developer of the app.</span></span> <span data-ttu-id="59302-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-180">notes</span><span class="sxs-lookup"><span data-stu-id="59302-180">notes</span></span>|<span data-ttu-id="59302-181">String</span><span class="sxs-lookup"><span data-stu-id="59302-181">String</span></span>|<span data-ttu-id="59302-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-182">Notes for the app.</span></span> <span data-ttu-id="59302-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="59302-184">uploadState</span></span>|<span data-ttu-id="59302-185">Int32</span><span class="sxs-lookup"><span data-stu-id="59302-185">Int32</span></span>|<span data-ttu-id="59302-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="59302-186">The upload state.</span></span> <span data-ttu-id="59302-187">Возможные значения: 0- `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="59302-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="59302-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="59302-189">publishingState</span></span>|[<span data-ttu-id="59302-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="59302-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="59302-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-191">The publishing state for the app.</span></span> <span data-ttu-id="59302-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="59302-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="59302-193">Наследуется от [mobileApp.](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59302-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="59302-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="59302-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="59302-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="59302-195">isAssigned</span></span>|<span data-ttu-id="59302-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="59302-196">Boolean</span></span>|<span data-ttu-id="59302-197">Значение, указывающее, назначено ли приложению хотя бы одна группа.</span><span class="sxs-lookup"><span data-stu-id="59302-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="59302-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="59302-199">roleScopeTagIds</span></span>|<span data-ttu-id="59302-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="59302-200">String collection</span></span>|<span data-ttu-id="59302-201">Список ид тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="59302-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="59302-203">dependentAppCount</span></span>|<span data-ttu-id="59302-204">Int32</span><span class="sxs-lookup"><span data-stu-id="59302-204">Int32</span></span>|<span data-ttu-id="59302-205">Общее количество зависимостей, которые есть у этого приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="59302-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="59302-207">supersedingAppCount</span></span>|<span data-ttu-id="59302-208">Int32</span><span class="sxs-lookup"><span data-stu-id="59302-208">Int32</span></span>|<span data-ttu-id="59302-209">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="59302-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="59302-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="59302-211">supersededAppCount</span></span>|<span data-ttu-id="59302-212">Int32</span><span class="sxs-lookup"><span data-stu-id="59302-212">Int32</span></span>|<span data-ttu-id="59302-213">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="59302-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="59302-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59302-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="59302-215">appAvailability</span></span>|[<span data-ttu-id="59302-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="59302-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="59302-217">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-217">The Application's availability.</span></span> <span data-ttu-id="59302-218">Наследуется от [managedApp.](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="59302-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="59302-219">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="59302-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="59302-220">version</span><span class="sxs-lookup"><span data-stu-id="59302-220">version</span></span>|<span data-ttu-id="59302-221">String</span><span class="sxs-lookup"><span data-stu-id="59302-221">String</span></span>|<span data-ttu-id="59302-222">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-222">The Application's version.</span></span> <span data-ttu-id="59302-223">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="59302-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="59302-224">committedContentVersion</span></span>|<span data-ttu-id="59302-225">String</span><span class="sxs-lookup"><span data-stu-id="59302-225">String</span></span>|<span data-ttu-id="59302-226">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="59302-226">The internal committed content version.</span></span> <span data-ttu-id="59302-227">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="59302-228">fileName</span><span class="sxs-lookup"><span data-stu-id="59302-228">fileName</span></span>|<span data-ttu-id="59302-229">String</span><span class="sxs-lookup"><span data-stu-id="59302-229">String</span></span>|<span data-ttu-id="59302-230">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="59302-230">The name of the main Lob application file.</span></span> <span data-ttu-id="59302-231">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="59302-232">size</span><span class="sxs-lookup"><span data-stu-id="59302-232">size</span></span>|<span data-ttu-id="59302-233">Int64</span><span class="sxs-lookup"><span data-stu-id="59302-233">Int64</span></span>|<span data-ttu-id="59302-234">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="59302-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="59302-235">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="59302-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="59302-236">packageId</span><span class="sxs-lookup"><span data-stu-id="59302-236">packageId</span></span>|<span data-ttu-id="59302-237">String</span><span class="sxs-lookup"><span data-stu-id="59302-237">String</span></span>|<span data-ttu-id="59302-238">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="59302-238">The package identifier.</span></span>|
|<span data-ttu-id="59302-239">identityName</span><span class="sxs-lookup"><span data-stu-id="59302-239">identityName</span></span>|<span data-ttu-id="59302-240">String</span><span class="sxs-lookup"><span data-stu-id="59302-240">String</span></span>|<span data-ttu-id="59302-241">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="59302-241">The Identity Name.</span></span>|
|<span data-ttu-id="59302-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="59302-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="59302-243">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="59302-243">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="59302-244">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="59302-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="59302-245">versionName</span><span class="sxs-lookup"><span data-stu-id="59302-245">versionName</span></span>|<span data-ttu-id="59302-246">String</span><span class="sxs-lookup"><span data-stu-id="59302-246">String</span></span>|<span data-ttu-id="59302-247">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="59302-247">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="59302-248">versionCode</span><span class="sxs-lookup"><span data-stu-id="59302-248">versionCode</span></span>|<span data-ttu-id="59302-249">String</span><span class="sxs-lookup"><span data-stu-id="59302-249">String</span></span>|<span data-ttu-id="59302-250">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="59302-250">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="59302-251">identityVersion</span><span class="sxs-lookup"><span data-stu-id="59302-251">identityVersion</span></span>|<span data-ttu-id="59302-252">String</span><span class="sxs-lookup"><span data-stu-id="59302-252">String</span></span>|<span data-ttu-id="59302-253">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="59302-253">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="59302-254">Ответ</span><span class="sxs-lookup"><span data-stu-id="59302-254">Response</span></span>
<span data-ttu-id="59302-255">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="59302-255">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59302-256">Пример</span><span class="sxs-lookup"><span data-stu-id="59302-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="59302-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="59302-257">Request</span></span>
<span data-ttu-id="59302-258">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59302-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1588

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="59302-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="59302-259">Response</span></span>
<span data-ttu-id="59302-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59302-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1760

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




