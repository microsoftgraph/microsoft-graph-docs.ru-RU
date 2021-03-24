---
title: Обновление объекта macOSOfficeSuiteApp
description: Обновление свойств объекта macOSOfficeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c95a0c5a45a80677d24861132176b1f1949e0d74
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140401"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="a4ad7-103">Обновление объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="a4ad7-103">Update macOSOfficeSuiteApp</span></span>

<span data-ttu-id="a4ad7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4ad7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4ad7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4ad7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4ad7-107">Обновление свойств объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-107">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4ad7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a4ad7-108">Prerequisites</span></span>
<span data-ttu-id="a4ad7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4ad7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4ad7-111">Permission type</span></span>|<span data-ttu-id="a4ad7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4ad7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4ad7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4ad7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4ad7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4ad7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4ad7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4ad7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4ad7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-116">Not supported.</span></span>|
|<span data-ttu-id="a4ad7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4ad7-117">Application</span></span>|<span data-ttu-id="a4ad7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4ad7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4ad7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4ad7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a4ad7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a4ad7-120">Request headers</span></span>
|<span data-ttu-id="a4ad7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4ad7-121">Header</span></span>|<span data-ttu-id="a4ad7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a4ad7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4ad7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4ad7-123">Authorization</span></span>|<span data-ttu-id="a4ad7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4ad7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a4ad7-125">Accept</span></span>|<span data-ttu-id="a4ad7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4ad7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4ad7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4ad7-127">Request body</span></span>
<span data-ttu-id="a4ad7-128">В тексте запроса добавьте представление объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-128">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="a4ad7-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-129">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="a4ad7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4ad7-130">Property</span></span>|<span data-ttu-id="a4ad7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a4ad7-131">Type</span></span>|<span data-ttu-id="a4ad7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a4ad7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4ad7-133">id</span><span class="sxs-lookup"><span data-stu-id="a4ad7-133">id</span></span>|<span data-ttu-id="a4ad7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a4ad7-134">String</span></span>|<span data-ttu-id="a4ad7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-135">Key of the entity.</span></span> <span data-ttu-id="a4ad7-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a4ad7-137">displayName</span></span>|<span data-ttu-id="a4ad7-138">Строка</span><span class="sxs-lookup"><span data-stu-id="a4ad7-138">String</span></span>|<span data-ttu-id="a4ad7-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a4ad7-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-141">description</span><span class="sxs-lookup"><span data-stu-id="a4ad7-141">description</span></span>|<span data-ttu-id="a4ad7-142">Строка</span><span class="sxs-lookup"><span data-stu-id="a4ad7-142">String</span></span>|<span data-ttu-id="a4ad7-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-143">The description of the app.</span></span> <span data-ttu-id="a4ad7-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a4ad7-145">publisher</span></span>|<span data-ttu-id="a4ad7-146">String</span><span class="sxs-lookup"><span data-stu-id="a4ad7-146">String</span></span>|<span data-ttu-id="a4ad7-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-147">The publisher of the app.</span></span> <span data-ttu-id="a4ad7-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a4ad7-149">largeIcon</span></span>|[<span data-ttu-id="a4ad7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a4ad7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a4ad7-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a4ad7-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4ad7-153">createdDateTime</span></span>|<span data-ttu-id="a4ad7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4ad7-154">DateTimeOffset</span></span>|<span data-ttu-id="a4ad7-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-155">The date and time the app was created.</span></span> <span data-ttu-id="a4ad7-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4ad7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a4ad7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4ad7-158">DateTimeOffset</span></span>|<span data-ttu-id="a4ad7-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a4ad7-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a4ad7-161">isFeatured</span></span>|<span data-ttu-id="a4ad7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4ad7-162">Boolean</span></span>|<span data-ttu-id="a4ad7-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a4ad7-164">privacyInformationUrl</span></span>|<span data-ttu-id="a4ad7-165">String</span><span class="sxs-lookup"><span data-stu-id="a4ad7-165">String</span></span>|<span data-ttu-id="a4ad7-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-166">The privacy statement Url.</span></span> <span data-ttu-id="a4ad7-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a4ad7-168">informationUrl</span></span>|<span data-ttu-id="a4ad7-169">String</span><span class="sxs-lookup"><span data-stu-id="a4ad7-169">String</span></span>|<span data-ttu-id="a4ad7-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-170">The more information Url.</span></span> <span data-ttu-id="a4ad7-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-172">owner</span><span class="sxs-lookup"><span data-stu-id="a4ad7-172">owner</span></span>|<span data-ttu-id="a4ad7-173">String</span><span class="sxs-lookup"><span data-stu-id="a4ad7-173">String</span></span>|<span data-ttu-id="a4ad7-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-174">The owner of the app.</span></span> <span data-ttu-id="a4ad7-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-176">developer</span><span class="sxs-lookup"><span data-stu-id="a4ad7-176">developer</span></span>|<span data-ttu-id="a4ad7-177">String</span><span class="sxs-lookup"><span data-stu-id="a4ad7-177">String</span></span>|<span data-ttu-id="a4ad7-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-178">The developer of the app.</span></span> <span data-ttu-id="a4ad7-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-180">notes</span><span class="sxs-lookup"><span data-stu-id="a4ad7-180">notes</span></span>|<span data-ttu-id="a4ad7-181">String</span><span class="sxs-lookup"><span data-stu-id="a4ad7-181">String</span></span>|<span data-ttu-id="a4ad7-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-182">Notes for the app.</span></span> <span data-ttu-id="a4ad7-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a4ad7-184">uploadState</span></span>|<span data-ttu-id="a4ad7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a4ad7-185">Int32</span></span>|<span data-ttu-id="a4ad7-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-186">The upload state.</span></span> <span data-ttu-id="a4ad7-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="a4ad7-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="a4ad7-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="a4ad7-189">publishingState</span></span>|[<span data-ttu-id="a4ad7-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a4ad7-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a4ad7-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-191">The publishing state for the app.</span></span> <span data-ttu-id="a4ad7-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a4ad7-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="a4ad7-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a4ad7-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a4ad7-195">isAssigned</span></span>|<span data-ttu-id="a4ad7-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4ad7-196">Boolean</span></span>|<span data-ttu-id="a4ad7-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a4ad7-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a4ad7-199">roleScopeTagIds</span></span>|<span data-ttu-id="a4ad7-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a4ad7-200">String collection</span></span>|<span data-ttu-id="a4ad7-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a4ad7-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="a4ad7-203">dependentAppCount</span></span>|<span data-ttu-id="a4ad7-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a4ad7-204">Int32</span></span>|<span data-ttu-id="a4ad7-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a4ad7-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="a4ad7-207">supersedingAppCount</span></span>|<span data-ttu-id="a4ad7-208">Int32</span><span class="sxs-lookup"><span data-stu-id="a4ad7-208">Int32</span></span>|<span data-ttu-id="a4ad7-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="a4ad7-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ad7-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="a4ad7-211">supersededAppCount</span></span>|<span data-ttu-id="a4ad7-212">Int32</span><span class="sxs-lookup"><span data-stu-id="a4ad7-212">Int32</span></span>|<span data-ttu-id="a4ad7-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="a4ad7-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ad7-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a4ad7-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4ad7-215">Response</span></span>
<span data-ttu-id="a4ad7-216">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-216">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4ad7-217">Пример</span><span class="sxs-lookup"><span data-stu-id="a4ad7-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4ad7-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4ad7-218">Request</span></span>
<span data-ttu-id="a4ad7-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 775

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "supersededAppCount": 2
}
```

### <a name="response"></a><span data-ttu-id="a4ad7-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4ad7-220">Response</span></span>
<span data-ttu-id="a4ad7-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4ad7-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 947

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "supersededAppCount": 2
}
```




