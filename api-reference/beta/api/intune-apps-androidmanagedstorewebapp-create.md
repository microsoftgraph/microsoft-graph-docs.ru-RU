---
title: Создание AndroidManagedStoreWebApp
description: Создание нового объекта AndroidManagedStoreWebApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02c2ef44ea107529e40dd4a3f0d0ed0767f25979
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144384"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="4da22-103">Создание AndroidManagedStoreWebApp</span><span class="sxs-lookup"><span data-stu-id="4da22-103">Create androidManagedStoreWebApp</span></span>

<span data-ttu-id="4da22-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4da22-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4da22-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4da22-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4da22-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4da22-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4da22-107">Создание нового [объекта AndroidManagedStoreWebApp.](../resources/intune-apps-androidmanagedstorewebapp.md)</span><span class="sxs-lookup"><span data-stu-id="4da22-107">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4da22-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4da22-108">Prerequisites</span></span>
<span data-ttu-id="4da22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4da22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4da22-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4da22-111">Permission type</span></span>|<span data-ttu-id="4da22-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4da22-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4da22-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4da22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4da22-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4da22-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4da22-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4da22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4da22-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4da22-116">Not supported.</span></span>|
|<span data-ttu-id="4da22-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4da22-117">Application</span></span>|<span data-ttu-id="4da22-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4da22-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4da22-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4da22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4da22-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4da22-120">Request headers</span></span>
|<span data-ttu-id="4da22-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4da22-121">Header</span></span>|<span data-ttu-id="4da22-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4da22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4da22-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4da22-123">Authorization</span></span>|<span data-ttu-id="4da22-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4da22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4da22-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4da22-125">Accept</span></span>|<span data-ttu-id="4da22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4da22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4da22-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4da22-127">Request body</span></span>
<span data-ttu-id="4da22-128">В теле запроса поставляем представление JSON для объекта AndroidManagedStoreWebApp.</span><span class="sxs-lookup"><span data-stu-id="4da22-128">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="4da22-129">В следующей таблице показаны свойства, необходимые при создании androidManagedStoreWebApp.</span><span class="sxs-lookup"><span data-stu-id="4da22-129">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="4da22-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4da22-130">Property</span></span>|<span data-ttu-id="4da22-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4da22-131">Type</span></span>|<span data-ttu-id="4da22-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4da22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4da22-133">id</span><span class="sxs-lookup"><span data-stu-id="4da22-133">id</span></span>|<span data-ttu-id="4da22-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4da22-134">String</span></span>|<span data-ttu-id="4da22-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4da22-135">Key of the entity.</span></span> <span data-ttu-id="4da22-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4da22-137">displayName</span></span>|<span data-ttu-id="4da22-138">Строка</span><span class="sxs-lookup"><span data-stu-id="4da22-138">String</span></span>|<span data-ttu-id="4da22-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="4da22-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4da22-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-141">description</span><span class="sxs-lookup"><span data-stu-id="4da22-141">description</span></span>|<span data-ttu-id="4da22-142">Строка</span><span class="sxs-lookup"><span data-stu-id="4da22-142">String</span></span>|<span data-ttu-id="4da22-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="4da22-143">The description of the app.</span></span> <span data-ttu-id="4da22-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-145">publisher</span><span class="sxs-lookup"><span data-stu-id="4da22-145">publisher</span></span>|<span data-ttu-id="4da22-146">String</span><span class="sxs-lookup"><span data-stu-id="4da22-146">String</span></span>|<span data-ttu-id="4da22-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="4da22-147">The publisher of the app.</span></span> <span data-ttu-id="4da22-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4da22-149">largeIcon</span></span>|[<span data-ttu-id="4da22-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4da22-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4da22-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="4da22-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4da22-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4da22-153">createdDateTime</span></span>|<span data-ttu-id="4da22-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4da22-154">DateTimeOffset</span></span>|<span data-ttu-id="4da22-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="4da22-155">The date and time the app was created.</span></span> <span data-ttu-id="4da22-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4da22-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4da22-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4da22-158">DateTimeOffset</span></span>|<span data-ttu-id="4da22-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="4da22-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4da22-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4da22-161">isFeatured</span></span>|<span data-ttu-id="4da22-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4da22-162">Boolean</span></span>|<span data-ttu-id="4da22-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4da22-164">privacyInformationUrl</span></span>|<span data-ttu-id="4da22-165">String</span><span class="sxs-lookup"><span data-stu-id="4da22-165">String</span></span>|<span data-ttu-id="4da22-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4da22-166">The privacy statement Url.</span></span> <span data-ttu-id="4da22-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4da22-168">informationUrl</span></span>|<span data-ttu-id="4da22-169">String</span><span class="sxs-lookup"><span data-stu-id="4da22-169">String</span></span>|<span data-ttu-id="4da22-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="4da22-170">The more information Url.</span></span> <span data-ttu-id="4da22-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-172">owner</span><span class="sxs-lookup"><span data-stu-id="4da22-172">owner</span></span>|<span data-ttu-id="4da22-173">String</span><span class="sxs-lookup"><span data-stu-id="4da22-173">String</span></span>|<span data-ttu-id="4da22-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="4da22-174">The owner of the app.</span></span> <span data-ttu-id="4da22-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-176">developer</span><span class="sxs-lookup"><span data-stu-id="4da22-176">developer</span></span>|<span data-ttu-id="4da22-177">String</span><span class="sxs-lookup"><span data-stu-id="4da22-177">String</span></span>|<span data-ttu-id="4da22-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="4da22-178">The developer of the app.</span></span> <span data-ttu-id="4da22-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-180">notes</span><span class="sxs-lookup"><span data-stu-id="4da22-180">notes</span></span>|<span data-ttu-id="4da22-181">String</span><span class="sxs-lookup"><span data-stu-id="4da22-181">String</span></span>|<span data-ttu-id="4da22-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="4da22-182">Notes for the app.</span></span> <span data-ttu-id="4da22-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4da22-184">uploadState</span></span>|<span data-ttu-id="4da22-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4da22-185">Int32</span></span>|<span data-ttu-id="4da22-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="4da22-186">The upload state.</span></span> <span data-ttu-id="4da22-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="4da22-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="4da22-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="4da22-189">publishingState</span></span>|[<span data-ttu-id="4da22-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4da22-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4da22-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="4da22-191">The publishing state for the app.</span></span> <span data-ttu-id="4da22-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="4da22-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4da22-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4da22-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4da22-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4da22-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4da22-195">isAssigned</span></span>|<span data-ttu-id="4da22-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="4da22-196">Boolean</span></span>|<span data-ttu-id="4da22-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="4da22-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4da22-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4da22-199">roleScopeTagIds</span></span>|<span data-ttu-id="4da22-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4da22-200">String collection</span></span>|<span data-ttu-id="4da22-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="4da22-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4da22-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4da22-203">dependentAppCount</span></span>|<span data-ttu-id="4da22-204">Int32</span><span class="sxs-lookup"><span data-stu-id="4da22-204">Int32</span></span>|<span data-ttu-id="4da22-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="4da22-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4da22-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="4da22-207">supersedingAppCount</span></span>|<span data-ttu-id="4da22-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4da22-208">Int32</span></span>|<span data-ttu-id="4da22-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="4da22-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="4da22-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="4da22-211">supersededAppCount</span></span>|<span data-ttu-id="4da22-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4da22-212">Int32</span></span>|<span data-ttu-id="4da22-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="4da22-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="4da22-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4da22-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4da22-215">packageId</span><span class="sxs-lookup"><span data-stu-id="4da22-215">packageId</span></span>|<span data-ttu-id="4da22-216">String</span><span class="sxs-lookup"><span data-stu-id="4da22-216">String</span></span>|<span data-ttu-id="4da22-217">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="4da22-217">The package identifier.</span></span> <span data-ttu-id="4da22-218">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4da22-218">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4da22-219">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="4da22-219">appIdentifier</span></span>|<span data-ttu-id="4da22-220">String</span><span class="sxs-lookup"><span data-stu-id="4da22-220">String</span></span>|<span data-ttu-id="4da22-221">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4da22-221">The Identity Name.</span></span> <span data-ttu-id="4da22-222">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4da22-222">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4da22-223">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4da22-223">usedLicenseCount</span></span>|<span data-ttu-id="4da22-224">Int32</span><span class="sxs-lookup"><span data-stu-id="4da22-224">Int32</span></span>|<span data-ttu-id="4da22-225">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="4da22-225">The number of VPP licenses in use.</span></span> <span data-ttu-id="4da22-226">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4da22-226">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4da22-227">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4da22-227">totalLicenseCount</span></span>|<span data-ttu-id="4da22-228">Int32</span><span class="sxs-lookup"><span data-stu-id="4da22-228">Int32</span></span>|<span data-ttu-id="4da22-229">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="4da22-229">The total number of VPP licenses.</span></span> <span data-ttu-id="4da22-230">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4da22-230">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4da22-231">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4da22-231">appStoreUrl</span></span>|<span data-ttu-id="4da22-232">String</span><span class="sxs-lookup"><span data-stu-id="4da22-232">String</span></span>|<span data-ttu-id="4da22-233">URL-адрес приложения Play for Work Store.</span><span class="sxs-lookup"><span data-stu-id="4da22-233">The Play for Work Store app URL.</span></span> <span data-ttu-id="4da22-234">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4da22-234">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4da22-235">isPrivate</span><span class="sxs-lookup"><span data-stu-id="4da22-235">isPrivate</span></span>|<span data-ttu-id="4da22-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="4da22-236">Boolean</span></span>|<span data-ttu-id="4da22-237">Указывает, доступно ли приложение только пользователям данного предприятия.</span><span class="sxs-lookup"><span data-stu-id="4da22-237">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="4da22-238">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4da22-238">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4da22-239">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="4da22-239">isSystemApp</span></span>|<span data-ttu-id="4da22-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="4da22-240">Boolean</span></span>|<span data-ttu-id="4da22-241">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="4da22-241">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="4da22-242">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4da22-242">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4da22-243">appTracks</span><span class="sxs-lookup"><span data-stu-id="4da22-243">appTracks</span></span>|<span data-ttu-id="4da22-244">[коллекция AndroidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="4da22-244">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="4da22-245">Отслеживает, которые видны этому предприятию.</span><span class="sxs-lookup"><span data-stu-id="4da22-245">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="4da22-246">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4da22-246">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="4da22-247">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="4da22-247">supportsOemConfig</span></span>|<span data-ttu-id="4da22-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="4da22-248">Boolean</span></span>|<span data-ttu-id="4da22-249">Поддерживает ли это приложение политику OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="4da22-249">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="4da22-250">Унаследованный от [AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="4da22-250">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4da22-251">Отклик</span><span class="sxs-lookup"><span data-stu-id="4da22-251">Response</span></span>
<span data-ttu-id="4da22-252">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект AndroidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4da22-252">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4da22-253">Пример</span><span class="sxs-lookup"><span data-stu-id="4da22-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="4da22-254">Запрос</span><span class="sxs-lookup"><span data-stu-id="4da22-254">Request</span></span>
<span data-ttu-id="4da22-255">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4da22-255">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1228

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="4da22-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="4da22-256">Response</span></span>
<span data-ttu-id="4da22-p130">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4da22-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1400

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```




