---
title: Обновление AndroidForWorkApp
description: Обновление свойств объекта AndroidForWorkApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 062131cb18c217e9fa7f6a0db836f2d05bd1eed3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141101"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="45914-103">Обновление AndroidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="45914-103">Update androidForWorkApp</span></span>

<span data-ttu-id="45914-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45914-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45914-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45914-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45914-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45914-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45914-107">Обновление свойств объекта [AndroidForWorkApp.](../resources/intune-apps-androidforworkapp.md)</span><span class="sxs-lookup"><span data-stu-id="45914-107">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45914-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="45914-108">Prerequisites</span></span>
<span data-ttu-id="45914-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45914-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45914-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45914-111">Permission type</span></span>|<span data-ttu-id="45914-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45914-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45914-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45914-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45914-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45914-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45914-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45914-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45914-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45914-116">Not supported.</span></span>|
|<span data-ttu-id="45914-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="45914-117">Application</span></span>|<span data-ttu-id="45914-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45914-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45914-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45914-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="45914-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45914-120">Request headers</span></span>
|<span data-ttu-id="45914-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45914-121">Header</span></span>|<span data-ttu-id="45914-122">Значение</span><span class="sxs-lookup"><span data-stu-id="45914-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45914-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45914-123">Authorization</span></span>|<span data-ttu-id="45914-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45914-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45914-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45914-125">Accept</span></span>|<span data-ttu-id="45914-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45914-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45914-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45914-127">Request body</span></span>
<span data-ttu-id="45914-128">В теле запроса поставляем представление JSON для [объекта AndroidForWorkApp.](../resources/intune-apps-androidforworkapp.md)</span><span class="sxs-lookup"><span data-stu-id="45914-128">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="45914-129">В следующей таблице показаны свойства, необходимые при создании [androidForWorkApp.](../resources/intune-apps-androidforworkapp.md)</span><span class="sxs-lookup"><span data-stu-id="45914-129">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="45914-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="45914-130">Property</span></span>|<span data-ttu-id="45914-131">Тип</span><span class="sxs-lookup"><span data-stu-id="45914-131">Type</span></span>|<span data-ttu-id="45914-132">Описание</span><span class="sxs-lookup"><span data-stu-id="45914-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45914-133">id</span><span class="sxs-lookup"><span data-stu-id="45914-133">id</span></span>|<span data-ttu-id="45914-134">Строка</span><span class="sxs-lookup"><span data-stu-id="45914-134">String</span></span>|<span data-ttu-id="45914-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="45914-135">Key of the entity.</span></span> <span data-ttu-id="45914-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-137">displayName</span><span class="sxs-lookup"><span data-stu-id="45914-137">displayName</span></span>|<span data-ttu-id="45914-138">Строка</span><span class="sxs-lookup"><span data-stu-id="45914-138">String</span></span>|<span data-ttu-id="45914-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="45914-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="45914-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-141">description</span><span class="sxs-lookup"><span data-stu-id="45914-141">description</span></span>|<span data-ttu-id="45914-142">Строка</span><span class="sxs-lookup"><span data-stu-id="45914-142">String</span></span>|<span data-ttu-id="45914-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="45914-143">The description of the app.</span></span> <span data-ttu-id="45914-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-145">publisher</span><span class="sxs-lookup"><span data-stu-id="45914-145">publisher</span></span>|<span data-ttu-id="45914-146">String</span><span class="sxs-lookup"><span data-stu-id="45914-146">String</span></span>|<span data-ttu-id="45914-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="45914-147">The publisher of the app.</span></span> <span data-ttu-id="45914-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="45914-149">largeIcon</span></span>|[<span data-ttu-id="45914-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="45914-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="45914-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="45914-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="45914-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45914-153">createdDateTime</span></span>|<span data-ttu-id="45914-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45914-154">DateTimeOffset</span></span>|<span data-ttu-id="45914-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="45914-155">The date and time the app was created.</span></span> <span data-ttu-id="45914-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45914-157">lastModifiedDateTime</span></span>|<span data-ttu-id="45914-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45914-158">DateTimeOffset</span></span>|<span data-ttu-id="45914-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="45914-159">The date and time the app was last modified.</span></span> <span data-ttu-id="45914-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="45914-161">isFeatured</span></span>|<span data-ttu-id="45914-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="45914-162">Boolean</span></span>|<span data-ttu-id="45914-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="45914-164">privacyInformationUrl</span></span>|<span data-ttu-id="45914-165">String</span><span class="sxs-lookup"><span data-stu-id="45914-165">String</span></span>|<span data-ttu-id="45914-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="45914-166">The privacy statement Url.</span></span> <span data-ttu-id="45914-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="45914-168">informationUrl</span></span>|<span data-ttu-id="45914-169">String</span><span class="sxs-lookup"><span data-stu-id="45914-169">String</span></span>|<span data-ttu-id="45914-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="45914-170">The more information Url.</span></span> <span data-ttu-id="45914-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-172">owner</span><span class="sxs-lookup"><span data-stu-id="45914-172">owner</span></span>|<span data-ttu-id="45914-173">String</span><span class="sxs-lookup"><span data-stu-id="45914-173">String</span></span>|<span data-ttu-id="45914-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="45914-174">The owner of the app.</span></span> <span data-ttu-id="45914-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-176">developer</span><span class="sxs-lookup"><span data-stu-id="45914-176">developer</span></span>|<span data-ttu-id="45914-177">String</span><span class="sxs-lookup"><span data-stu-id="45914-177">String</span></span>|<span data-ttu-id="45914-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="45914-178">The developer of the app.</span></span> <span data-ttu-id="45914-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-180">notes</span><span class="sxs-lookup"><span data-stu-id="45914-180">notes</span></span>|<span data-ttu-id="45914-181">String</span><span class="sxs-lookup"><span data-stu-id="45914-181">String</span></span>|<span data-ttu-id="45914-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="45914-182">Notes for the app.</span></span> <span data-ttu-id="45914-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="45914-184">uploadState</span></span>|<span data-ttu-id="45914-185">Int32</span><span class="sxs-lookup"><span data-stu-id="45914-185">Int32</span></span>|<span data-ttu-id="45914-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="45914-186">The upload state.</span></span> <span data-ttu-id="45914-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="45914-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="45914-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="45914-189">publishingState</span></span>|[<span data-ttu-id="45914-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="45914-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="45914-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="45914-191">The publishing state for the app.</span></span> <span data-ttu-id="45914-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="45914-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="45914-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="45914-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="45914-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="45914-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="45914-195">isAssigned</span></span>|<span data-ttu-id="45914-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="45914-196">Boolean</span></span>|<span data-ttu-id="45914-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="45914-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="45914-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45914-199">roleScopeTagIds</span></span>|<span data-ttu-id="45914-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="45914-200">String collection</span></span>|<span data-ttu-id="45914-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="45914-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="45914-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="45914-203">dependentAppCount</span></span>|<span data-ttu-id="45914-204">Int32</span><span class="sxs-lookup"><span data-stu-id="45914-204">Int32</span></span>|<span data-ttu-id="45914-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="45914-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="45914-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="45914-207">supersedingAppCount</span></span>|<span data-ttu-id="45914-208">Int32</span><span class="sxs-lookup"><span data-stu-id="45914-208">Int32</span></span>|<span data-ttu-id="45914-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="45914-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="45914-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="45914-211">supersededAppCount</span></span>|<span data-ttu-id="45914-212">Int32</span><span class="sxs-lookup"><span data-stu-id="45914-212">Int32</span></span>|<span data-ttu-id="45914-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="45914-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="45914-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45914-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45914-215">packageId</span><span class="sxs-lookup"><span data-stu-id="45914-215">packageId</span></span>|<span data-ttu-id="45914-216">String</span><span class="sxs-lookup"><span data-stu-id="45914-216">String</span></span>|<span data-ttu-id="45914-217">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="45914-217">The package identifier.</span></span>|
|<span data-ttu-id="45914-218">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="45914-218">appIdentifier</span></span>|<span data-ttu-id="45914-219">String</span><span class="sxs-lookup"><span data-stu-id="45914-219">String</span></span>|<span data-ttu-id="45914-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="45914-220">The Identity Name.</span></span>|
|<span data-ttu-id="45914-221">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="45914-221">usedLicenseCount</span></span>|<span data-ttu-id="45914-222">Int32</span><span class="sxs-lookup"><span data-stu-id="45914-222">Int32</span></span>|<span data-ttu-id="45914-223">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="45914-223">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="45914-224">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="45914-224">totalLicenseCount</span></span>|<span data-ttu-id="45914-225">Int32</span><span class="sxs-lookup"><span data-stu-id="45914-225">Int32</span></span>|<span data-ttu-id="45914-226">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="45914-226">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="45914-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="45914-227">appStoreUrl</span></span>|<span data-ttu-id="45914-228">String</span><span class="sxs-lookup"><span data-stu-id="45914-228">String</span></span>|<span data-ttu-id="45914-229">URL-адрес приложения Play for Work Store.</span><span class="sxs-lookup"><span data-stu-id="45914-229">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="45914-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="45914-230">Response</span></span>
<span data-ttu-id="45914-231">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45914-231">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45914-232">Пример</span><span class="sxs-lookup"><span data-stu-id="45914-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="45914-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="45914-233">Request</span></span>
<span data-ttu-id="45914-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45914-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 960

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="45914-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="45914-235">Response</span></span>
<span data-ttu-id="45914-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45914-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1132

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




