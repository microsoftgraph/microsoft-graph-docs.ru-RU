---
title: Создание AndroidManagedStoreApp
description: Создайте новый объект AndroidManagedStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 61381599a4de67e5b4b691d22364cd82737d9adc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144440"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="17ccd-103">Создание AndroidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="17ccd-103">Create androidManagedStoreApp</span></span>

<span data-ttu-id="17ccd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17ccd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17ccd-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17ccd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17ccd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17ccd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17ccd-107">Создайте новый [объект AndroidManagedStoreApp.](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ccd-107">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17ccd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="17ccd-108">Prerequisites</span></span>
<span data-ttu-id="17ccd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17ccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17ccd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17ccd-111">Permission type</span></span>|<span data-ttu-id="17ccd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17ccd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17ccd-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17ccd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17ccd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17ccd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="17ccd-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17ccd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17ccd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17ccd-116">Not supported.</span></span>|
|<span data-ttu-id="17ccd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="17ccd-117">Application</span></span>|<span data-ttu-id="17ccd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17ccd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17ccd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17ccd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="17ccd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="17ccd-120">Request headers</span></span>
|<span data-ttu-id="17ccd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17ccd-121">Header</span></span>|<span data-ttu-id="17ccd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="17ccd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17ccd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="17ccd-123">Authorization</span></span>|<span data-ttu-id="17ccd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17ccd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17ccd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="17ccd-125">Accept</span></span>|<span data-ttu-id="17ccd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17ccd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17ccd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17ccd-127">Request body</span></span>
<span data-ttu-id="17ccd-128">В теле запроса поставляем представление JSON для объекта AndroidManagedStoreApp.</span><span class="sxs-lookup"><span data-stu-id="17ccd-128">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="17ccd-129">В следующей таблице показаны свойства, необходимые при создании androidManagedStoreApp.</span><span class="sxs-lookup"><span data-stu-id="17ccd-129">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="17ccd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="17ccd-130">Property</span></span>|<span data-ttu-id="17ccd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="17ccd-131">Type</span></span>|<span data-ttu-id="17ccd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="17ccd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17ccd-133">id</span><span class="sxs-lookup"><span data-stu-id="17ccd-133">id</span></span>|<span data-ttu-id="17ccd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="17ccd-134">String</span></span>|<span data-ttu-id="17ccd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="17ccd-135">Key of the entity.</span></span> <span data-ttu-id="17ccd-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="17ccd-137">displayName</span></span>|<span data-ttu-id="17ccd-138">Строка</span><span class="sxs-lookup"><span data-stu-id="17ccd-138">String</span></span>|<span data-ttu-id="17ccd-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="17ccd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="17ccd-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-141">description</span><span class="sxs-lookup"><span data-stu-id="17ccd-141">description</span></span>|<span data-ttu-id="17ccd-142">Строка</span><span class="sxs-lookup"><span data-stu-id="17ccd-142">String</span></span>|<span data-ttu-id="17ccd-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="17ccd-143">The description of the app.</span></span> <span data-ttu-id="17ccd-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-145">publisher</span><span class="sxs-lookup"><span data-stu-id="17ccd-145">publisher</span></span>|<span data-ttu-id="17ccd-146">String</span><span class="sxs-lookup"><span data-stu-id="17ccd-146">String</span></span>|<span data-ttu-id="17ccd-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="17ccd-147">The publisher of the app.</span></span> <span data-ttu-id="17ccd-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="17ccd-149">largeIcon</span></span>|[<span data-ttu-id="17ccd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="17ccd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="17ccd-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="17ccd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="17ccd-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17ccd-153">createdDateTime</span></span>|<span data-ttu-id="17ccd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17ccd-154">DateTimeOffset</span></span>|<span data-ttu-id="17ccd-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="17ccd-155">The date and time the app was created.</span></span> <span data-ttu-id="17ccd-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17ccd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="17ccd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17ccd-158">DateTimeOffset</span></span>|<span data-ttu-id="17ccd-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="17ccd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="17ccd-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="17ccd-161">isFeatured</span></span>|<span data-ttu-id="17ccd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ccd-162">Boolean</span></span>|<span data-ttu-id="17ccd-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="17ccd-164">privacyInformationUrl</span></span>|<span data-ttu-id="17ccd-165">String</span><span class="sxs-lookup"><span data-stu-id="17ccd-165">String</span></span>|<span data-ttu-id="17ccd-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="17ccd-166">The privacy statement Url.</span></span> <span data-ttu-id="17ccd-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="17ccd-168">informationUrl</span></span>|<span data-ttu-id="17ccd-169">String</span><span class="sxs-lookup"><span data-stu-id="17ccd-169">String</span></span>|<span data-ttu-id="17ccd-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="17ccd-170">The more information Url.</span></span> <span data-ttu-id="17ccd-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-172">owner</span><span class="sxs-lookup"><span data-stu-id="17ccd-172">owner</span></span>|<span data-ttu-id="17ccd-173">String</span><span class="sxs-lookup"><span data-stu-id="17ccd-173">String</span></span>|<span data-ttu-id="17ccd-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="17ccd-174">The owner of the app.</span></span> <span data-ttu-id="17ccd-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-176">developer</span><span class="sxs-lookup"><span data-stu-id="17ccd-176">developer</span></span>|<span data-ttu-id="17ccd-177">String</span><span class="sxs-lookup"><span data-stu-id="17ccd-177">String</span></span>|<span data-ttu-id="17ccd-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="17ccd-178">The developer of the app.</span></span> <span data-ttu-id="17ccd-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-180">notes</span><span class="sxs-lookup"><span data-stu-id="17ccd-180">notes</span></span>|<span data-ttu-id="17ccd-181">String</span><span class="sxs-lookup"><span data-stu-id="17ccd-181">String</span></span>|<span data-ttu-id="17ccd-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="17ccd-182">Notes for the app.</span></span> <span data-ttu-id="17ccd-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="17ccd-184">uploadState</span></span>|<span data-ttu-id="17ccd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="17ccd-185">Int32</span></span>|<span data-ttu-id="17ccd-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="17ccd-186">The upload state.</span></span> <span data-ttu-id="17ccd-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="17ccd-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="17ccd-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="17ccd-189">publishingState</span></span>|[<span data-ttu-id="17ccd-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="17ccd-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="17ccd-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="17ccd-191">The publishing state for the app.</span></span> <span data-ttu-id="17ccd-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="17ccd-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="17ccd-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="17ccd-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="17ccd-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="17ccd-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="17ccd-195">isAssigned</span></span>|<span data-ttu-id="17ccd-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ccd-196">Boolean</span></span>|<span data-ttu-id="17ccd-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="17ccd-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="17ccd-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17ccd-199">roleScopeTagIds</span></span>|<span data-ttu-id="17ccd-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="17ccd-200">String collection</span></span>|<span data-ttu-id="17ccd-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="17ccd-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="17ccd-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="17ccd-203">dependentAppCount</span></span>|<span data-ttu-id="17ccd-204">Int32</span><span class="sxs-lookup"><span data-stu-id="17ccd-204">Int32</span></span>|<span data-ttu-id="17ccd-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="17ccd-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="17ccd-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="17ccd-207">supersedingAppCount</span></span>|<span data-ttu-id="17ccd-208">Int32</span><span class="sxs-lookup"><span data-stu-id="17ccd-208">Int32</span></span>|<span data-ttu-id="17ccd-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="17ccd-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="17ccd-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="17ccd-211">supersededAppCount</span></span>|<span data-ttu-id="17ccd-212">Int32</span><span class="sxs-lookup"><span data-stu-id="17ccd-212">Int32</span></span>|<span data-ttu-id="17ccd-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="17ccd-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="17ccd-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ccd-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="17ccd-215">packageId</span><span class="sxs-lookup"><span data-stu-id="17ccd-215">packageId</span></span>|<span data-ttu-id="17ccd-216">String</span><span class="sxs-lookup"><span data-stu-id="17ccd-216">String</span></span>|<span data-ttu-id="17ccd-217">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="17ccd-217">The package identifier.</span></span>|
|<span data-ttu-id="17ccd-218">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="17ccd-218">appIdentifier</span></span>|<span data-ttu-id="17ccd-219">String</span><span class="sxs-lookup"><span data-stu-id="17ccd-219">String</span></span>|<span data-ttu-id="17ccd-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="17ccd-220">The Identity Name.</span></span>|
|<span data-ttu-id="17ccd-221">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="17ccd-221">usedLicenseCount</span></span>|<span data-ttu-id="17ccd-222">Int32</span><span class="sxs-lookup"><span data-stu-id="17ccd-222">Int32</span></span>|<span data-ttu-id="17ccd-223">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="17ccd-223">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="17ccd-224">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="17ccd-224">totalLicenseCount</span></span>|<span data-ttu-id="17ccd-225">Int32</span><span class="sxs-lookup"><span data-stu-id="17ccd-225">Int32</span></span>|<span data-ttu-id="17ccd-226">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="17ccd-226">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="17ccd-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="17ccd-227">appStoreUrl</span></span>|<span data-ttu-id="17ccd-228">String</span><span class="sxs-lookup"><span data-stu-id="17ccd-228">String</span></span>|<span data-ttu-id="17ccd-229">URL-адрес приложения Play for Work Store.</span><span class="sxs-lookup"><span data-stu-id="17ccd-229">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="17ccd-230">isPrivate</span><span class="sxs-lookup"><span data-stu-id="17ccd-230">isPrivate</span></span>|<span data-ttu-id="17ccd-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ccd-231">Boolean</span></span>|<span data-ttu-id="17ccd-232">Указывает, доступно ли приложение только пользователям данного предприятия.</span><span class="sxs-lookup"><span data-stu-id="17ccd-232">Indicates whether the app is only available to a given enterprise's users.</span></span>|
|<span data-ttu-id="17ccd-233">isSystemApp</span><span class="sxs-lookup"><span data-stu-id="17ccd-233">isSystemApp</span></span>|<span data-ttu-id="17ccd-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ccd-234">Boolean</span></span>|<span data-ttu-id="17ccd-235">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="17ccd-235">Indicates whether the app is a preinstalled system app.</span></span>|
|<span data-ttu-id="17ccd-236">appTracks</span><span class="sxs-lookup"><span data-stu-id="17ccd-236">appTracks</span></span>|<span data-ttu-id="17ccd-237">[коллекция AndroidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="17ccd-237">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="17ccd-238">Отслеживает, которые видны этому предприятию.</span><span class="sxs-lookup"><span data-stu-id="17ccd-238">The tracks that are visible to this enterprise.</span></span>|
|<span data-ttu-id="17ccd-239">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="17ccd-239">supportsOemConfig</span></span>|<span data-ttu-id="17ccd-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ccd-240">Boolean</span></span>|<span data-ttu-id="17ccd-241">Поддерживает ли это приложение политику OEMConfig.</span><span class="sxs-lookup"><span data-stu-id="17ccd-241">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="17ccd-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="17ccd-242">Response</span></span>
<span data-ttu-id="17ccd-243">В случае успеха этот метод возвращает код отклика и `201 Created` [объект AndroidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17ccd-243">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17ccd-244">Пример</span><span class="sxs-lookup"><span data-stu-id="17ccd-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="17ccd-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="17ccd-245">Request</span></span>
<span data-ttu-id="17ccd-246">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17ccd-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1225

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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

### <a name="response"></a><span data-ttu-id="17ccd-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="17ccd-247">Response</span></span>
<span data-ttu-id="17ccd-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17ccd-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1397

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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




