---
title: Create managedAndroidLobApp
description: Создание объекта managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 970879cbdcf84f47ee3ce12c428d11df55ae74f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990356"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="a9401-103">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="a9401-103">Create managedAndroidLobApp</span></span>

<span data-ttu-id="a9401-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9401-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9401-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9401-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9401-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9401-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9401-107">Создание объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9401-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a9401-108">Prerequisites</span></span>
<span data-ttu-id="a9401-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9401-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9401-111">Permission type</span></span>|<span data-ttu-id="a9401-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9401-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9401-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9401-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9401-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9401-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a9401-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9401-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9401-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9401-116">Not supported.</span></span>|
|<span data-ttu-id="a9401-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9401-117">Application</span></span>|<span data-ttu-id="a9401-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9401-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9401-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9401-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a9401-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a9401-120">Request headers</span></span>
|<span data-ttu-id="a9401-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9401-121">Header</span></span>|<span data-ttu-id="a9401-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a9401-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9401-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9401-123">Authorization</span></span>|<span data-ttu-id="a9401-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9401-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9401-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9401-125">Accept</span></span>|<span data-ttu-id="a9401-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9401-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9401-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a9401-127">Request body</span></span>
<span data-ttu-id="a9401-128">В тексте запроса добавьте представление объекта managedAndroidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9401-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="a9401-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="a9401-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="a9401-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9401-130">Property</span></span>|<span data-ttu-id="a9401-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a9401-131">Type</span></span>|<span data-ttu-id="a9401-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a9401-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9401-133">id</span><span class="sxs-lookup"><span data-stu-id="a9401-133">id</span></span>|<span data-ttu-id="a9401-134">String</span><span class="sxs-lookup"><span data-stu-id="a9401-134">String</span></span>|<span data-ttu-id="a9401-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a9401-135">Key of the entity.</span></span> <span data-ttu-id="a9401-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a9401-137">displayName</span></span>|<span data-ttu-id="a9401-138">String</span><span class="sxs-lookup"><span data-stu-id="a9401-138">String</span></span>|<span data-ttu-id="a9401-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a9401-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a9401-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-141">description</span><span class="sxs-lookup"><span data-stu-id="a9401-141">description</span></span>|<span data-ttu-id="a9401-142">String</span><span class="sxs-lookup"><span data-stu-id="a9401-142">String</span></span>|<span data-ttu-id="a9401-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-143">The description of the app.</span></span> <span data-ttu-id="a9401-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a9401-145">publisher</span></span>|<span data-ttu-id="a9401-146">String</span><span class="sxs-lookup"><span data-stu-id="a9401-146">String</span></span>|<span data-ttu-id="a9401-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-147">The publisher of the app.</span></span> <span data-ttu-id="a9401-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a9401-149">largeIcon</span></span>|[<span data-ttu-id="a9401-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a9401-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a9401-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a9401-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a9401-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9401-153">createdDateTime</span></span>|<span data-ttu-id="a9401-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9401-154">DateTimeOffset</span></span>|<span data-ttu-id="a9401-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-155">The date and time the app was created.</span></span> <span data-ttu-id="a9401-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9401-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a9401-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9401-158">DateTimeOffset</span></span>|<span data-ttu-id="a9401-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a9401-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a9401-161">isFeatured</span></span>|<span data-ttu-id="a9401-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9401-162">Boolean</span></span>|<span data-ttu-id="a9401-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a9401-164">privacyInformationUrl</span></span>|<span data-ttu-id="a9401-165">String</span><span class="sxs-lookup"><span data-stu-id="a9401-165">String</span></span>|<span data-ttu-id="a9401-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a9401-166">The privacy statement Url.</span></span> <span data-ttu-id="a9401-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a9401-168">informationUrl</span></span>|<span data-ttu-id="a9401-169">String</span><span class="sxs-lookup"><span data-stu-id="a9401-169">String</span></span>|<span data-ttu-id="a9401-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a9401-170">The more information Url.</span></span> <span data-ttu-id="a9401-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-172">owner</span><span class="sxs-lookup"><span data-stu-id="a9401-172">owner</span></span>|<span data-ttu-id="a9401-173">String</span><span class="sxs-lookup"><span data-stu-id="a9401-173">String</span></span>|<span data-ttu-id="a9401-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-174">The owner of the app.</span></span> <span data-ttu-id="a9401-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-176">developer</span><span class="sxs-lookup"><span data-stu-id="a9401-176">developer</span></span>|<span data-ttu-id="a9401-177">String</span><span class="sxs-lookup"><span data-stu-id="a9401-177">String</span></span>|<span data-ttu-id="a9401-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-178">The developer of the app.</span></span> <span data-ttu-id="a9401-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-180">notes</span><span class="sxs-lookup"><span data-stu-id="a9401-180">notes</span></span>|<span data-ttu-id="a9401-181">String</span><span class="sxs-lookup"><span data-stu-id="a9401-181">String</span></span>|<span data-ttu-id="a9401-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-182">Notes for the app.</span></span> <span data-ttu-id="a9401-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a9401-184">uploadState</span></span>|<span data-ttu-id="a9401-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a9401-185">Int32</span></span>|<span data-ttu-id="a9401-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="a9401-186">The upload state.</span></span> <span data-ttu-id="a9401-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="a9401-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="a9401-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="a9401-189">publishingState</span></span>|[<span data-ttu-id="a9401-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="a9401-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a9401-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-191">The publishing state for the app.</span></span> <span data-ttu-id="a9401-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a9401-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a9401-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="a9401-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a9401-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a9401-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a9401-195">isAssigned</span></span>|<span data-ttu-id="a9401-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9401-196">Boolean</span></span>|<span data-ttu-id="a9401-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="a9401-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a9401-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9401-199">roleScopeTagIds</span></span>|<span data-ttu-id="a9401-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a9401-200">String collection</span></span>|<span data-ttu-id="a9401-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a9401-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a9401-203">dependentAppCount</span></span>|<span data-ttu-id="a9401-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a9401-204">Int32</span></span>|<span data-ttu-id="a9401-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a9401-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a9401-207">supersedingAppCount</span></span>|<span data-ttu-id="a9401-208">Int32</span><span class="sxs-lookup"><span data-stu-id="a9401-208">Int32</span></span>|<span data-ttu-id="a9401-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="a9401-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="a9401-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a9401-211">supersededAppCount</span></span>|<span data-ttu-id="a9401-212">Int32</span><span class="sxs-lookup"><span data-stu-id="a9401-212">Int32</span></span>|<span data-ttu-id="a9401-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="a9401-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="a9401-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9401-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="a9401-215">appAvailability</span></span>|[<span data-ttu-id="a9401-216">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="a9401-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="a9401-217">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-217">The Application's availability.</span></span> <span data-ttu-id="a9401-218">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="a9401-219">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="a9401-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="a9401-220">version</span><span class="sxs-lookup"><span data-stu-id="a9401-220">version</span></span>|<span data-ttu-id="a9401-221">String</span><span class="sxs-lookup"><span data-stu-id="a9401-221">String</span></span>|<span data-ttu-id="a9401-222">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-222">The Application's version.</span></span> <span data-ttu-id="a9401-223">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="a9401-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a9401-224">committedContentVersion</span></span>|<span data-ttu-id="a9401-225">String</span><span class="sxs-lookup"><span data-stu-id="a9401-225">String</span></span>|<span data-ttu-id="a9401-226">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="a9401-226">The internal committed content version.</span></span> <span data-ttu-id="a9401-227">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a9401-228">fileName</span><span class="sxs-lookup"><span data-stu-id="a9401-228">fileName</span></span>|<span data-ttu-id="a9401-229">String</span><span class="sxs-lookup"><span data-stu-id="a9401-229">String</span></span>|<span data-ttu-id="a9401-230">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="a9401-230">The name of the main Lob application file.</span></span> <span data-ttu-id="a9401-231">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a9401-232">size</span><span class="sxs-lookup"><span data-stu-id="a9401-232">size</span></span>|<span data-ttu-id="a9401-233">Int64</span><span class="sxs-lookup"><span data-stu-id="a9401-233">Int64</span></span>|<span data-ttu-id="a9401-234">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="a9401-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="a9401-235">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9401-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a9401-236">packageId</span><span class="sxs-lookup"><span data-stu-id="a9401-236">packageId</span></span>|<span data-ttu-id="a9401-237">String</span><span class="sxs-lookup"><span data-stu-id="a9401-237">String</span></span>|<span data-ttu-id="a9401-238">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="a9401-238">The package identifier.</span></span>|
|<span data-ttu-id="a9401-239">identityName</span><span class="sxs-lookup"><span data-stu-id="a9401-239">identityName</span></span>|<span data-ttu-id="a9401-240">String</span><span class="sxs-lookup"><span data-stu-id="a9401-240">String</span></span>|<span data-ttu-id="a9401-241">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a9401-241">The Identity Name.</span></span>|
|<span data-ttu-id="a9401-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a9401-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a9401-243">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a9401-243">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="a9401-244">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="a9401-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a9401-245">versionName</span><span class="sxs-lookup"><span data-stu-id="a9401-245">versionName</span></span>|<span data-ttu-id="a9401-246">String</span><span class="sxs-lookup"><span data-stu-id="a9401-246">String</span></span>|<span data-ttu-id="a9401-247">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="a9401-247">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a9401-248">versionCode</span><span class="sxs-lookup"><span data-stu-id="a9401-248">versionCode</span></span>|<span data-ttu-id="a9401-249">String</span><span class="sxs-lookup"><span data-stu-id="a9401-249">String</span></span>|<span data-ttu-id="a9401-250">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="a9401-250">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a9401-251">identityVersion</span><span class="sxs-lookup"><span data-stu-id="a9401-251">identityVersion</span></span>|<span data-ttu-id="a9401-252">String</span><span class="sxs-lookup"><span data-stu-id="a9401-252">String</span></span>|<span data-ttu-id="a9401-253">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a9401-253">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="a9401-254">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9401-254">Response</span></span>
<span data-ttu-id="a9401-255">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a9401-255">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9401-256">Пример</span><span class="sxs-lookup"><span data-stu-id="a9401-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9401-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9401-257">Request</span></span>
<span data-ttu-id="a9401-258">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9401-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1548

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
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="a9401-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9401-259">Response</span></span>
<span data-ttu-id="a9401-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9401-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1720

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
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```






