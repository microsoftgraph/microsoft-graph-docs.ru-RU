---
title: Create managedAndroidStoreApp
description: Создание нового объекта managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f82737edbf60eab5a0aa6d742752def379733b4d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014996"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="c24c4-103">Create managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="c24c4-103">Create managedAndroidStoreApp</span></span>

<span data-ttu-id="c24c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c24c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c24c4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c24c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c24c4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c24c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c24c4-107">Создание нового объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-107">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c24c4-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c24c4-108">Prerequisites</span></span>
<span data-ttu-id="c24c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c24c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c24c4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c24c4-111">Permission type</span></span>|<span data-ttu-id="c24c4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c24c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c24c4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c24c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c24c4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c24c4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c24c4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c24c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c24c4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c24c4-116">Not supported.</span></span>|
|<span data-ttu-id="c24c4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c24c4-117">Application</span></span>|<span data-ttu-id="c24c4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c24c4-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c24c4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c24c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c24c4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c24c4-120">Request headers</span></span>
|<span data-ttu-id="c24c4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c24c4-121">Header</span></span>|<span data-ttu-id="c24c4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c24c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c24c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c24c4-123">Authorization</span></span>|<span data-ttu-id="c24c4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c24c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c24c4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c24c4-125">Accept</span></span>|<span data-ttu-id="c24c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c24c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c24c4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c24c4-127">Request body</span></span>
<span data-ttu-id="c24c4-128">В теле запроса добавьте представление объекта managedAndroidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c24c4-128">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="c24c4-129">Ниже показаны свойства, которые необходимо указывать при создании объекта managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="c24c4-129">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="c24c4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c24c4-130">Property</span></span>|<span data-ttu-id="c24c4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c24c4-131">Type</span></span>|<span data-ttu-id="c24c4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c24c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c24c4-133">id</span><span class="sxs-lookup"><span data-stu-id="c24c4-133">id</span></span>|<span data-ttu-id="c24c4-134">String</span><span class="sxs-lookup"><span data-stu-id="c24c4-134">String</span></span>|<span data-ttu-id="c24c4-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c24c4-135">Key of the entity.</span></span> <span data-ttu-id="c24c4-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c24c4-137">displayName</span></span>|<span data-ttu-id="c24c4-138">String</span><span class="sxs-lookup"><span data-stu-id="c24c4-138">String</span></span>|<span data-ttu-id="c24c4-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c24c4-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c24c4-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-141">description</span><span class="sxs-lookup"><span data-stu-id="c24c4-141">description</span></span>|<span data-ttu-id="c24c4-142">String</span><span class="sxs-lookup"><span data-stu-id="c24c4-142">String</span></span>|<span data-ttu-id="c24c4-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-143">The description of the app.</span></span> <span data-ttu-id="c24c4-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c24c4-145">publisher</span></span>|<span data-ttu-id="c24c4-146">String</span><span class="sxs-lookup"><span data-stu-id="c24c4-146">String</span></span>|<span data-ttu-id="c24c4-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-147">The publisher of the app.</span></span> <span data-ttu-id="c24c4-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c24c4-149">largeIcon</span></span>|[<span data-ttu-id="c24c4-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c24c4-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c24c4-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="c24c4-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c24c4-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c24c4-153">createdDateTime</span></span>|<span data-ttu-id="c24c4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c24c4-154">DateTimeOffset</span></span>|<span data-ttu-id="c24c4-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-155">The date and time the app was created.</span></span> <span data-ttu-id="c24c4-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c24c4-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c24c4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c24c4-158">DateTimeOffset</span></span>|<span data-ttu-id="c24c4-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c24c4-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c24c4-161">isFeatured</span></span>|<span data-ttu-id="c24c4-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c24c4-162">Boolean</span></span>|<span data-ttu-id="c24c4-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c24c4-164">privacyInformationUrl</span></span>|<span data-ttu-id="c24c4-165">String</span><span class="sxs-lookup"><span data-stu-id="c24c4-165">String</span></span>|<span data-ttu-id="c24c4-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c24c4-166">The privacy statement Url.</span></span> <span data-ttu-id="c24c4-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c24c4-168">informationUrl</span></span>|<span data-ttu-id="c24c4-169">String</span><span class="sxs-lookup"><span data-stu-id="c24c4-169">String</span></span>|<span data-ttu-id="c24c4-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="c24c4-170">The more information Url.</span></span> <span data-ttu-id="c24c4-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-172">owner</span><span class="sxs-lookup"><span data-stu-id="c24c4-172">owner</span></span>|<span data-ttu-id="c24c4-173">String</span><span class="sxs-lookup"><span data-stu-id="c24c4-173">String</span></span>|<span data-ttu-id="c24c4-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-174">The owner of the app.</span></span> <span data-ttu-id="c24c4-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-176">developer</span><span class="sxs-lookup"><span data-stu-id="c24c4-176">developer</span></span>|<span data-ttu-id="c24c4-177">String</span><span class="sxs-lookup"><span data-stu-id="c24c4-177">String</span></span>|<span data-ttu-id="c24c4-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-178">The developer of the app.</span></span> <span data-ttu-id="c24c4-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-180">notes</span><span class="sxs-lookup"><span data-stu-id="c24c4-180">notes</span></span>|<span data-ttu-id="c24c4-181">String</span><span class="sxs-lookup"><span data-stu-id="c24c4-181">String</span></span>|<span data-ttu-id="c24c4-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-182">Notes for the app.</span></span> <span data-ttu-id="c24c4-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c24c4-184">uploadState</span></span>|<span data-ttu-id="c24c4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c24c4-185">Int32</span></span>|<span data-ttu-id="c24c4-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="c24c4-186">The upload state.</span></span> <span data-ttu-id="c24c4-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="c24c4-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="c24c4-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="c24c4-189">publishingState</span></span>|[<span data-ttu-id="c24c4-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="c24c4-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c24c4-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-191">The publishing state for the app.</span></span> <span data-ttu-id="c24c4-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="c24c4-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c24c4-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="c24c4-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c24c4-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c24c4-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c24c4-195">isAssigned</span></span>|<span data-ttu-id="c24c4-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="c24c4-196">Boolean</span></span>|<span data-ttu-id="c24c4-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="c24c4-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c24c4-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c24c4-199">roleScopeTagIds</span></span>|<span data-ttu-id="c24c4-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c24c4-200">String collection</span></span>|<span data-ttu-id="c24c4-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c24c4-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="c24c4-203">dependentAppCount</span></span>|<span data-ttu-id="c24c4-204">Int32</span><span class="sxs-lookup"><span data-stu-id="c24c4-204">Int32</span></span>|<span data-ttu-id="c24c4-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="c24c4-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="c24c4-207">supersedingAppCount</span></span>|<span data-ttu-id="c24c4-208">Int32</span><span class="sxs-lookup"><span data-stu-id="c24c4-208">Int32</span></span>|<span data-ttu-id="c24c4-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="c24c4-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="c24c4-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="c24c4-211">supersededAppCount</span></span>|<span data-ttu-id="c24c4-212">Int32</span><span class="sxs-lookup"><span data-stu-id="c24c4-212">Int32</span></span>|<span data-ttu-id="c24c4-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="c24c4-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="c24c4-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c24c4-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="c24c4-215">appAvailability</span></span>|[<span data-ttu-id="c24c4-216">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="c24c4-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="c24c4-217">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-217">The Application's availability.</span></span> <span data-ttu-id="c24c4-218">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="c24c4-219">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="c24c4-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="c24c4-220">version</span><span class="sxs-lookup"><span data-stu-id="c24c4-220">version</span></span>|<span data-ttu-id="c24c4-221">String</span><span class="sxs-lookup"><span data-stu-id="c24c4-221">String</span></span>|<span data-ttu-id="c24c4-222">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-222">The Application's version.</span></span> <span data-ttu-id="c24c4-223">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c24c4-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="c24c4-224">packageId</span><span class="sxs-lookup"><span data-stu-id="c24c4-224">packageId</span></span>|<span data-ttu-id="c24c4-225">String</span><span class="sxs-lookup"><span data-stu-id="c24c4-225">String</span></span>|<span data-ttu-id="c24c4-226">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="c24c4-226">The app's package ID.</span></span>|
|<span data-ttu-id="c24c4-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c24c4-227">appStoreUrl</span></span>|<span data-ttu-id="c24c4-228">String</span><span class="sxs-lookup"><span data-stu-id="c24c4-228">String</span></span>|<span data-ttu-id="c24c4-229">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="c24c4-229">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="c24c4-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c24c4-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c24c4-231">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c24c4-231">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="c24c4-232">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="c24c4-232">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="c24c4-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="c24c4-233">Response</span></span>
<span data-ttu-id="c24c4-234">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c24c4-234">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c24c4-235">Пример</span><span class="sxs-lookup"><span data-stu-id="c24c4-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="c24c4-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="c24c4-236">Request</span></span>
<span data-ttu-id="c24c4-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c24c4-237">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c24c4-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="c24c4-238">Response</span></span>
<span data-ttu-id="c24c4-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c24c4-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






