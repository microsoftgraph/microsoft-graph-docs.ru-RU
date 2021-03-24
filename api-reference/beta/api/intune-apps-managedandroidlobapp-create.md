---
title: Create managedAndroidLobApp
description: Создание объекта managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f019d246eb57942046b25e6386fad769683c8629
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143754"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="ba40f-103">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="ba40f-103">Create managedAndroidLobApp</span></span>

<span data-ttu-id="ba40f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba40f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba40f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba40f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba40f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba40f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba40f-107">Создание объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba40f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ba40f-108">Prerequisites</span></span>
<span data-ttu-id="ba40f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba40f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba40f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba40f-111">Permission type</span></span>|<span data-ttu-id="ba40f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba40f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba40f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba40f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba40f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba40f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ba40f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba40f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba40f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba40f-116">Not supported.</span></span>|
|<span data-ttu-id="ba40f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ba40f-117">Application</span></span>|<span data-ttu-id="ba40f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba40f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba40f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba40f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ba40f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ba40f-120">Request headers</span></span>
|<span data-ttu-id="ba40f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba40f-121">Header</span></span>|<span data-ttu-id="ba40f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ba40f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba40f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba40f-123">Authorization</span></span>|<span data-ttu-id="ba40f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba40f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba40f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ba40f-125">Accept</span></span>|<span data-ttu-id="ba40f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba40f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba40f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba40f-127">Request body</span></span>
<span data-ttu-id="ba40f-128">В тексте запроса добавьте представление объекта managedAndroidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba40f-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="ba40f-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="ba40f-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="ba40f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba40f-130">Property</span></span>|<span data-ttu-id="ba40f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ba40f-131">Type</span></span>|<span data-ttu-id="ba40f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ba40f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba40f-133">id</span><span class="sxs-lookup"><span data-stu-id="ba40f-133">id</span></span>|<span data-ttu-id="ba40f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ba40f-134">String</span></span>|<span data-ttu-id="ba40f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ba40f-135">Key of the entity.</span></span> <span data-ttu-id="ba40f-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ba40f-137">displayName</span></span>|<span data-ttu-id="ba40f-138">Строка</span><span class="sxs-lookup"><span data-stu-id="ba40f-138">String</span></span>|<span data-ttu-id="ba40f-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ba40f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ba40f-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-141">description</span><span class="sxs-lookup"><span data-stu-id="ba40f-141">description</span></span>|<span data-ttu-id="ba40f-142">Строка</span><span class="sxs-lookup"><span data-stu-id="ba40f-142">String</span></span>|<span data-ttu-id="ba40f-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-143">The description of the app.</span></span> <span data-ttu-id="ba40f-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ba40f-145">publisher</span></span>|<span data-ttu-id="ba40f-146">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-146">String</span></span>|<span data-ttu-id="ba40f-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-147">The publisher of the app.</span></span> <span data-ttu-id="ba40f-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ba40f-149">largeIcon</span></span>|[<span data-ttu-id="ba40f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ba40f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ba40f-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ba40f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ba40f-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba40f-153">createdDateTime</span></span>|<span data-ttu-id="ba40f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba40f-154">DateTimeOffset</span></span>|<span data-ttu-id="ba40f-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-155">The date and time the app was created.</span></span> <span data-ttu-id="ba40f-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba40f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ba40f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba40f-158">DateTimeOffset</span></span>|<span data-ttu-id="ba40f-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ba40f-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ba40f-161">isFeatured</span></span>|<span data-ttu-id="ba40f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba40f-162">Boolean</span></span>|<span data-ttu-id="ba40f-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ba40f-164">privacyInformationUrl</span></span>|<span data-ttu-id="ba40f-165">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-165">String</span></span>|<span data-ttu-id="ba40f-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ba40f-166">The privacy statement Url.</span></span> <span data-ttu-id="ba40f-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ba40f-168">informationUrl</span></span>|<span data-ttu-id="ba40f-169">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-169">String</span></span>|<span data-ttu-id="ba40f-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ba40f-170">The more information Url.</span></span> <span data-ttu-id="ba40f-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-172">owner</span><span class="sxs-lookup"><span data-stu-id="ba40f-172">owner</span></span>|<span data-ttu-id="ba40f-173">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-173">String</span></span>|<span data-ttu-id="ba40f-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-174">The owner of the app.</span></span> <span data-ttu-id="ba40f-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-176">developer</span><span class="sxs-lookup"><span data-stu-id="ba40f-176">developer</span></span>|<span data-ttu-id="ba40f-177">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-177">String</span></span>|<span data-ttu-id="ba40f-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-178">The developer of the app.</span></span> <span data-ttu-id="ba40f-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-180">notes</span><span class="sxs-lookup"><span data-stu-id="ba40f-180">notes</span></span>|<span data-ttu-id="ba40f-181">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-181">String</span></span>|<span data-ttu-id="ba40f-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-182">Notes for the app.</span></span> <span data-ttu-id="ba40f-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ba40f-184">uploadState</span></span>|<span data-ttu-id="ba40f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ba40f-185">Int32</span></span>|<span data-ttu-id="ba40f-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="ba40f-186">The upload state.</span></span> <span data-ttu-id="ba40f-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="ba40f-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ba40f-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ba40f-189">publishingState</span></span>|[<span data-ttu-id="ba40f-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ba40f-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ba40f-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-191">The publishing state for the app.</span></span> <span data-ttu-id="ba40f-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ba40f-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ba40f-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ba40f-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ba40f-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ba40f-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ba40f-195">isAssigned</span></span>|<span data-ttu-id="ba40f-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba40f-196">Boolean</span></span>|<span data-ttu-id="ba40f-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="ba40f-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ba40f-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ba40f-199">roleScopeTagIds</span></span>|<span data-ttu-id="ba40f-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ba40f-200">String collection</span></span>|<span data-ttu-id="ba40f-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ba40f-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ba40f-203">dependentAppCount</span></span>|<span data-ttu-id="ba40f-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ba40f-204">Int32</span></span>|<span data-ttu-id="ba40f-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="ba40f-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ba40f-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="ba40f-207">supersedingAppCount</span></span>|<span data-ttu-id="ba40f-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ba40f-208">Int32</span></span>|<span data-ttu-id="ba40f-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="ba40f-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="ba40f-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="ba40f-211">supersededAppCount</span></span>|<span data-ttu-id="ba40f-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ba40f-212">Int32</span></span>|<span data-ttu-id="ba40f-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="ba40f-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="ba40f-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ba40f-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="ba40f-215">appAvailability</span></span>|[<span data-ttu-id="ba40f-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="ba40f-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="ba40f-217">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-217">The Application's availability.</span></span> <span data-ttu-id="ba40f-218">Унаследованный от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="ba40f-219">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="ba40f-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="ba40f-220">version</span><span class="sxs-lookup"><span data-stu-id="ba40f-220">version</span></span>|<span data-ttu-id="ba40f-221">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-221">String</span></span>|<span data-ttu-id="ba40f-222">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-222">The Application's version.</span></span> <span data-ttu-id="ba40f-223">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="ba40f-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ba40f-224">committedContentVersion</span></span>|<span data-ttu-id="ba40f-225">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-225">String</span></span>|<span data-ttu-id="ba40f-226">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="ba40f-226">The internal committed content version.</span></span> <span data-ttu-id="ba40f-227">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ba40f-228">fileName</span><span class="sxs-lookup"><span data-stu-id="ba40f-228">fileName</span></span>|<span data-ttu-id="ba40f-229">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-229">String</span></span>|<span data-ttu-id="ba40f-230">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-230">The name of the main Lob application file.</span></span> <span data-ttu-id="ba40f-231">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ba40f-232">size</span><span class="sxs-lookup"><span data-stu-id="ba40f-232">size</span></span>|<span data-ttu-id="ba40f-233">Int64</span><span class="sxs-lookup"><span data-stu-id="ba40f-233">Int64</span></span>|<span data-ttu-id="ba40f-234">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="ba40f-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="ba40f-235">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ba40f-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ba40f-236">packageId</span><span class="sxs-lookup"><span data-stu-id="ba40f-236">packageId</span></span>|<span data-ttu-id="ba40f-237">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-237">String</span></span>|<span data-ttu-id="ba40f-238">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="ba40f-238">The package identifier.</span></span>|
|<span data-ttu-id="ba40f-239">identityName</span><span class="sxs-lookup"><span data-stu-id="ba40f-239">identityName</span></span>|<span data-ttu-id="ba40f-240">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-240">String</span></span>|<span data-ttu-id="ba40f-241">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-241">The Identity Name.</span></span>|
|<span data-ttu-id="ba40f-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ba40f-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ba40f-243">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ba40f-243">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="ba40f-244">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ba40f-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ba40f-245">versionName</span><span class="sxs-lookup"><span data-stu-id="ba40f-245">versionName</span></span>|<span data-ttu-id="ba40f-246">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-246">String</span></span>|<span data-ttu-id="ba40f-247">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="ba40f-247">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ba40f-248">versionCode</span><span class="sxs-lookup"><span data-stu-id="ba40f-248">versionCode</span></span>|<span data-ttu-id="ba40f-249">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-249">String</span></span>|<span data-ttu-id="ba40f-250">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="ba40f-250">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ba40f-251">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ba40f-251">identityVersion</span></span>|<span data-ttu-id="ba40f-252">String</span><span class="sxs-lookup"><span data-stu-id="ba40f-252">String</span></span>|<span data-ttu-id="ba40f-253">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ba40f-253">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ba40f-254">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba40f-254">Response</span></span>
<span data-ttu-id="ba40f-255">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ba40f-255">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba40f-256">Пример</span><span class="sxs-lookup"><span data-stu-id="ba40f-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba40f-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba40f-257">Request</span></span>
<span data-ttu-id="ba40f-258">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba40f-258">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ba40f-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba40f-259">Response</span></span>
<span data-ttu-id="ba40f-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba40f-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




