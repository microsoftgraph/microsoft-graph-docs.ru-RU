---
title: Create managedAndroidStoreApp
description: Создание нового объекта managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 832ca1bf8d7ef7c70f344bfb5a6bcfcbff250c27
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699592"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="6cf4c-103">Create managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="6cf4c-103">Create managedAndroidStoreApp</span></span>

<span data-ttu-id="6cf4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cf4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cf4c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cf4c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cf4c-107">Создание нового объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-107">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cf4c-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6cf4c-108">Prerequisites</span></span>
<span data-ttu-id="6cf4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cf4c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cf4c-111">Permission type</span></span>|<span data-ttu-id="6cf4c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cf4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cf4c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cf4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cf4c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cf4c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6cf4c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cf4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cf4c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-116">Not supported.</span></span>|
|<span data-ttu-id="6cf4c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cf4c-117">Application</span></span>|<span data-ttu-id="6cf4c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cf4c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cf4c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cf4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6cf4c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6cf4c-120">Request headers</span></span>
|<span data-ttu-id="6cf4c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6cf4c-121">Header</span></span>|<span data-ttu-id="6cf4c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6cf4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cf4c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6cf4c-123">Authorization</span></span>|<span data-ttu-id="6cf4c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cf4c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6cf4c-125">Accept</span></span>|<span data-ttu-id="6cf4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cf4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cf4c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6cf4c-127">Request body</span></span>
<span data-ttu-id="6cf4c-128">В теле запроса добавьте представление объекта managedAndroidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-128">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="6cf4c-129">Ниже показаны свойства, которые необходимо указывать при создании объекта managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-129">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="6cf4c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cf4c-130">Property</span></span>|<span data-ttu-id="6cf4c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6cf4c-131">Type</span></span>|<span data-ttu-id="6cf4c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6cf4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cf4c-133">id</span><span class="sxs-lookup"><span data-stu-id="6cf4c-133">id</span></span>|<span data-ttu-id="6cf4c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6cf4c-134">String</span></span>|<span data-ttu-id="6cf4c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-135">Key of the entity.</span></span> <span data-ttu-id="6cf4c-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6cf4c-137">displayName</span></span>|<span data-ttu-id="6cf4c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="6cf4c-138">String</span></span>|<span data-ttu-id="6cf4c-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6cf4c-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-141">description</span><span class="sxs-lookup"><span data-stu-id="6cf4c-141">description</span></span>|<span data-ttu-id="6cf4c-142">Строка</span><span class="sxs-lookup"><span data-stu-id="6cf4c-142">String</span></span>|<span data-ttu-id="6cf4c-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-143">The description of the app.</span></span> <span data-ttu-id="6cf4c-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-145">publisher</span><span class="sxs-lookup"><span data-stu-id="6cf4c-145">publisher</span></span>|<span data-ttu-id="6cf4c-146">String</span><span class="sxs-lookup"><span data-stu-id="6cf4c-146">String</span></span>|<span data-ttu-id="6cf4c-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-147">The publisher of the app.</span></span> <span data-ttu-id="6cf4c-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6cf4c-149">largeIcon</span></span>|[<span data-ttu-id="6cf4c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6cf4c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6cf4c-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6cf4c-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cf4c-153">createdDateTime</span></span>|<span data-ttu-id="6cf4c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cf4c-154">DateTimeOffset</span></span>|<span data-ttu-id="6cf4c-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-155">The date and time the app was created.</span></span> <span data-ttu-id="6cf4c-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cf4c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="6cf4c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cf4c-158">DateTimeOffset</span></span>|<span data-ttu-id="6cf4c-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="6cf4c-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6cf4c-161">isFeatured</span></span>|<span data-ttu-id="6cf4c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cf4c-162">Boolean</span></span>|<span data-ttu-id="6cf4c-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6cf4c-164">privacyInformationUrl</span></span>|<span data-ttu-id="6cf4c-165">String</span><span class="sxs-lookup"><span data-stu-id="6cf4c-165">String</span></span>|<span data-ttu-id="6cf4c-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-166">The privacy statement Url.</span></span> <span data-ttu-id="6cf4c-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6cf4c-168">informationUrl</span></span>|<span data-ttu-id="6cf4c-169">String</span><span class="sxs-lookup"><span data-stu-id="6cf4c-169">String</span></span>|<span data-ttu-id="6cf4c-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-170">The more information Url.</span></span> <span data-ttu-id="6cf4c-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-172">owner</span><span class="sxs-lookup"><span data-stu-id="6cf4c-172">owner</span></span>|<span data-ttu-id="6cf4c-173">String</span><span class="sxs-lookup"><span data-stu-id="6cf4c-173">String</span></span>|<span data-ttu-id="6cf4c-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-174">The owner of the app.</span></span> <span data-ttu-id="6cf4c-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-176">developer</span><span class="sxs-lookup"><span data-stu-id="6cf4c-176">developer</span></span>|<span data-ttu-id="6cf4c-177">String</span><span class="sxs-lookup"><span data-stu-id="6cf4c-177">String</span></span>|<span data-ttu-id="6cf4c-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-178">The developer of the app.</span></span> <span data-ttu-id="6cf4c-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-180">notes</span><span class="sxs-lookup"><span data-stu-id="6cf4c-180">notes</span></span>|<span data-ttu-id="6cf4c-181">String</span><span class="sxs-lookup"><span data-stu-id="6cf4c-181">String</span></span>|<span data-ttu-id="6cf4c-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-182">Notes for the app.</span></span> <span data-ttu-id="6cf4c-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="6cf4c-184">uploadState</span></span>|<span data-ttu-id="6cf4c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf4c-185">Int32</span></span>|<span data-ttu-id="6cf4c-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-186">The upload state.</span></span> <span data-ttu-id="6cf4c-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="6cf4c-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="6cf4c-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="6cf4c-189">publishingState</span></span>|[<span data-ttu-id="6cf4c-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="6cf4c-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6cf4c-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-191">The publishing state for the app.</span></span> <span data-ttu-id="6cf4c-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6cf4c-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="6cf4c-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6cf4c-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6cf4c-195">isAssigned</span></span>|<span data-ttu-id="6cf4c-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cf4c-196">Boolean</span></span>|<span data-ttu-id="6cf4c-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6cf4c-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6cf4c-199">roleScopeTagIds</span></span>|<span data-ttu-id="6cf4c-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6cf4c-200">String collection</span></span>|<span data-ttu-id="6cf4c-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6cf4c-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="6cf4c-203">dependentAppCount</span></span>|<span data-ttu-id="6cf4c-204">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf4c-204">Int32</span></span>|<span data-ttu-id="6cf4c-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6cf4c-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="6cf4c-207">supersedingAppCount</span></span>|<span data-ttu-id="6cf4c-208">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf4c-208">Int32</span></span>|<span data-ttu-id="6cf4c-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="6cf4c-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="6cf4c-211">supersededAppCount</span></span>|<span data-ttu-id="6cf4c-212">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf4c-212">Int32</span></span>|<span data-ttu-id="6cf4c-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="6cf4c-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf4c-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="6cf4c-215">appAvailability</span></span>|[<span data-ttu-id="6cf4c-216">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="6cf4c-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="6cf4c-217">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-217">The Application's availability.</span></span> <span data-ttu-id="6cf4c-218">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="6cf4c-219">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="6cf4c-220">version</span><span class="sxs-lookup"><span data-stu-id="6cf4c-220">version</span></span>|<span data-ttu-id="6cf4c-221">String</span><span class="sxs-lookup"><span data-stu-id="6cf4c-221">String</span></span>|<span data-ttu-id="6cf4c-222">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-222">The Application's version.</span></span> <span data-ttu-id="6cf4c-223">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf4c-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="6cf4c-224">packageId</span><span class="sxs-lookup"><span data-stu-id="6cf4c-224">packageId</span></span>|<span data-ttu-id="6cf4c-225">String</span><span class="sxs-lookup"><span data-stu-id="6cf4c-225">String</span></span>|<span data-ttu-id="6cf4c-226">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-226">The app's package ID.</span></span>|
|<span data-ttu-id="6cf4c-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6cf4c-227">appStoreUrl</span></span>|<span data-ttu-id="6cf4c-228">String</span><span class="sxs-lookup"><span data-stu-id="6cf4c-228">String</span></span>|<span data-ttu-id="6cf4c-229">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-229">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="6cf4c-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6cf4c-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6cf4c-231">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6cf4c-231">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="6cf4c-232">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-232">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="6cf4c-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="6cf4c-233">Response</span></span>
<span data-ttu-id="6cf4c-234">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-234">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cf4c-235">Пример</span><span class="sxs-lookup"><span data-stu-id="6cf4c-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cf4c-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cf4c-236">Request</span></span>
<span data-ttu-id="6cf4c-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-237">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1321

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="6cf4c-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cf4c-238">Response</span></span>
<span data-ttu-id="6cf4c-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cf4c-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1493

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```





