---
title: Обновление officeSuiteApp
description: Обновление свойств объекта officeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 16105781f02931fd3eaf62b3ca4703fc20d9290d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976909"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="07e5b-103">Обновление officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="07e5b-103">Update officeSuiteApp</span></span>

<span data-ttu-id="07e5b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07e5b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07e5b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07e5b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07e5b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07e5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07e5b-107">Обновление свойств объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="07e5b-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07e5b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="07e5b-108">Prerequisites</span></span>
<span data-ttu-id="07e5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07e5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07e5b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07e5b-111">Permission type</span></span>|<span data-ttu-id="07e5b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07e5b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07e5b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07e5b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07e5b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07e5b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="07e5b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07e5b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07e5b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07e5b-116">Not supported.</span></span>|
|<span data-ttu-id="07e5b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07e5b-117">Application</span></span>|<span data-ttu-id="07e5b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07e5b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07e5b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07e5b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="07e5b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="07e5b-120">Request headers</span></span>
|<span data-ttu-id="07e5b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07e5b-121">Header</span></span>|<span data-ttu-id="07e5b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="07e5b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07e5b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07e5b-123">Authorization</span></span>|<span data-ttu-id="07e5b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07e5b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07e5b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="07e5b-125">Accept</span></span>|<span data-ttu-id="07e5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07e5b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07e5b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="07e5b-127">Request body</span></span>
<span data-ttu-id="07e5b-128">В тексте запроса добавьте представление объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07e5b-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="07e5b-129">В следующей таблице приведены свойства, необходимые при создании [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="07e5b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="07e5b-130">Property</span></span>|<span data-ttu-id="07e5b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="07e5b-131">Type</span></span>|<span data-ttu-id="07e5b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="07e5b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07e5b-133">id</span><span class="sxs-lookup"><span data-stu-id="07e5b-133">id</span></span>|<span data-ttu-id="07e5b-134">String</span><span class="sxs-lookup"><span data-stu-id="07e5b-134">String</span></span>|<span data-ttu-id="07e5b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="07e5b-135">Key of the entity.</span></span> <span data-ttu-id="07e5b-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="07e5b-137">displayName</span></span>|<span data-ttu-id="07e5b-138">String</span><span class="sxs-lookup"><span data-stu-id="07e5b-138">String</span></span>|<span data-ttu-id="07e5b-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="07e5b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="07e5b-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-141">description</span><span class="sxs-lookup"><span data-stu-id="07e5b-141">description</span></span>|<span data-ttu-id="07e5b-142">String</span><span class="sxs-lookup"><span data-stu-id="07e5b-142">String</span></span>|<span data-ttu-id="07e5b-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="07e5b-143">The description of the app.</span></span> <span data-ttu-id="07e5b-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-145">publisher</span><span class="sxs-lookup"><span data-stu-id="07e5b-145">publisher</span></span>|<span data-ttu-id="07e5b-146">String</span><span class="sxs-lookup"><span data-stu-id="07e5b-146">String</span></span>|<span data-ttu-id="07e5b-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="07e5b-147">The publisher of the app.</span></span> <span data-ttu-id="07e5b-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="07e5b-149">largeIcon</span></span>|[<span data-ttu-id="07e5b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="07e5b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="07e5b-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="07e5b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="07e5b-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07e5b-153">createdDateTime</span></span>|<span data-ttu-id="07e5b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07e5b-154">DateTimeOffset</span></span>|<span data-ttu-id="07e5b-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="07e5b-155">The date and time the app was created.</span></span> <span data-ttu-id="07e5b-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07e5b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="07e5b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07e5b-158">DateTimeOffset</span></span>|<span data-ttu-id="07e5b-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="07e5b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="07e5b-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="07e5b-161">isFeatured</span></span>|<span data-ttu-id="07e5b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="07e5b-162">Boolean</span></span>|<span data-ttu-id="07e5b-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="07e5b-164">privacyInformationUrl</span></span>|<span data-ttu-id="07e5b-165">String</span><span class="sxs-lookup"><span data-stu-id="07e5b-165">String</span></span>|<span data-ttu-id="07e5b-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="07e5b-166">The privacy statement Url.</span></span> <span data-ttu-id="07e5b-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="07e5b-168">informationUrl</span></span>|<span data-ttu-id="07e5b-169">String</span><span class="sxs-lookup"><span data-stu-id="07e5b-169">String</span></span>|<span data-ttu-id="07e5b-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="07e5b-170">The more information Url.</span></span> <span data-ttu-id="07e5b-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-172">owner</span><span class="sxs-lookup"><span data-stu-id="07e5b-172">owner</span></span>|<span data-ttu-id="07e5b-173">String</span><span class="sxs-lookup"><span data-stu-id="07e5b-173">String</span></span>|<span data-ttu-id="07e5b-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="07e5b-174">The owner of the app.</span></span> <span data-ttu-id="07e5b-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-176">developer</span><span class="sxs-lookup"><span data-stu-id="07e5b-176">developer</span></span>|<span data-ttu-id="07e5b-177">String</span><span class="sxs-lookup"><span data-stu-id="07e5b-177">String</span></span>|<span data-ttu-id="07e5b-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="07e5b-178">The developer of the app.</span></span> <span data-ttu-id="07e5b-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-180">notes</span><span class="sxs-lookup"><span data-stu-id="07e5b-180">notes</span></span>|<span data-ttu-id="07e5b-181">String</span><span class="sxs-lookup"><span data-stu-id="07e5b-181">String</span></span>|<span data-ttu-id="07e5b-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="07e5b-182">Notes for the app.</span></span> <span data-ttu-id="07e5b-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="07e5b-184">uploadState</span></span>|<span data-ttu-id="07e5b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="07e5b-185">Int32</span></span>|<span data-ttu-id="07e5b-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="07e5b-186">The upload state.</span></span> <span data-ttu-id="07e5b-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="07e5b-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="07e5b-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="07e5b-189">publishingState</span></span>|[<span data-ttu-id="07e5b-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="07e5b-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="07e5b-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="07e5b-191">The publishing state for the app.</span></span> <span data-ttu-id="07e5b-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="07e5b-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="07e5b-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="07e5b-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="07e5b-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="07e5b-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="07e5b-195">isAssigned</span></span>|<span data-ttu-id="07e5b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="07e5b-196">Boolean</span></span>|<span data-ttu-id="07e5b-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="07e5b-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="07e5b-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="07e5b-199">roleScopeTagIds</span></span>|<span data-ttu-id="07e5b-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="07e5b-200">String collection</span></span>|<span data-ttu-id="07e5b-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="07e5b-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="07e5b-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="07e5b-203">dependentAppCount</span></span>|<span data-ttu-id="07e5b-204">Int32</span><span class="sxs-lookup"><span data-stu-id="07e5b-204">Int32</span></span>|<span data-ttu-id="07e5b-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="07e5b-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="07e5b-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="07e5b-207">supersedingAppCount</span></span>|<span data-ttu-id="07e5b-208">Int32</span><span class="sxs-lookup"><span data-stu-id="07e5b-208">Int32</span></span>|<span data-ttu-id="07e5b-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="07e5b-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="07e5b-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="07e5b-211">supersededAppCount</span></span>|<span data-ttu-id="07e5b-212">Int32</span><span class="sxs-lookup"><span data-stu-id="07e5b-212">Int32</span></span>|<span data-ttu-id="07e5b-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="07e5b-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="07e5b-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="07e5b-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07e5b-215">аутоакцептеула</span><span class="sxs-lookup"><span data-stu-id="07e5b-215">autoAcceptEula</span></span>|<span data-ttu-id="07e5b-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="07e5b-216">Boolean</span></span>|<span data-ttu-id="07e5b-217">Значение, которое будет автоматически принимать условия лицензионного соглашения на устройстве ендусер.</span><span class="sxs-lookup"><span data-stu-id="07e5b-217">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="07e5b-218">productIds</span><span class="sxs-lookup"><span data-stu-id="07e5b-218">productIds</span></span>|<span data-ttu-id="07e5b-219">Коллекция [оффицепродуктид](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="07e5b-219">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="07e5b-220">Идентификаторы продуктов, представляющие SKU набора Office365.</span><span class="sxs-lookup"><span data-stu-id="07e5b-220">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="07e5b-221">Возможные значения: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="07e5b-221">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="07e5b-222">excludedApps</span><span class="sxs-lookup"><span data-stu-id="07e5b-222">excludedApps</span></span>|<span data-ttu-id="07e5b-223">[excludedApps](../resources/intune-apps-excludedapps.md);</span><span class="sxs-lookup"><span data-stu-id="07e5b-223">[excludedApps](../resources/intune-apps-excludedapps.md)</span></span>|<span data-ttu-id="07e5b-224">Свойство для представления приложений, исключаемых из выбранного идентификатора продукта Office365.</span><span class="sxs-lookup"><span data-stu-id="07e5b-224">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="07e5b-225">Свойства usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="07e5b-225">useSharedComputerActivation</span></span>|<span data-ttu-id="07e5b-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="07e5b-226">Boolean</span></span>|<span data-ttu-id="07e5b-227">Свойство для представления того, используется ли активация на общем компьютере не для приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="07e5b-227">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="07e5b-228">updateChannel</span><span class="sxs-lookup"><span data-stu-id="07e5b-228">updateChannel</span></span>|[<span data-ttu-id="07e5b-229">оффицеупдатечаннел</span><span class="sxs-lookup"><span data-stu-id="07e5b-229">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="07e5b-230">Свойство для представления канала обновления Office365.</span><span class="sxs-lookup"><span data-stu-id="07e5b-230">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="07e5b-231">Возможные значения: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="07e5b-231">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.</span></span>|
|<span data-ttu-id="07e5b-232">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="07e5b-232">officePlatformArchitecture</span></span>|[<span data-ttu-id="07e5b-233">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="07e5b-233">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="07e5b-234">Свойство для представления версии набора приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="07e5b-234">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="07e5b-235">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="07e5b-235">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="07e5b-236">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="07e5b-236">localesToInstall</span></span>|<span data-ttu-id="07e5b-237">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="07e5b-237">String collection</span></span>|<span data-ttu-id="07e5b-238">Свойство для представления языковых стандартов, устанавливаемых при установке приложений из Office365.</span><span class="sxs-lookup"><span data-stu-id="07e5b-238">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="07e5b-239">В нем используется стандартная спецификация RFC 6033.</span><span class="sxs-lookup"><span data-stu-id="07e5b-239">It uses standard RFC 6033.</span></span> <span data-ttu-id="07e5b-240">Словом https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="07e5b-240">Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="07e5b-241">инсталлпрогрессдисплайлевел</span><span class="sxs-lookup"><span data-stu-id="07e5b-241">installProgressDisplayLevel</span></span>|[<span data-ttu-id="07e5b-242">оффицесуитеинсталлпрогрессдисплайлевел</span><span class="sxs-lookup"><span data-stu-id="07e5b-242">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="07e5b-243">Для указания уровня отображения пользовательского интерфейса установки хода установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="07e5b-243">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="07e5b-244">Возможные значения: `none`, `full`.</span><span class="sxs-lookup"><span data-stu-id="07e5b-244">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="07e5b-245">шаулдунинсталлолдерверсионсофоффице</span><span class="sxs-lookup"><span data-stu-id="07e5b-245">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="07e5b-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="07e5b-246">Boolean</span></span>|<span data-ttu-id="07e5b-247">Свойство, определяющее, следует ли удалить существующий MSI Office, если на устройстве развернут набор приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="07e5b-247">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="07e5b-248">Атрибута targetversion</span><span class="sxs-lookup"><span data-stu-id="07e5b-248">targetVersion</span></span>|<span data-ttu-id="07e5b-249">String</span><span class="sxs-lookup"><span data-stu-id="07e5b-249">String</span></span>|<span data-ttu-id="07e5b-250">Свойство, представляющее определенную целевую версию для набора приложений Office365, который должен быть развернут на устройствах.</span><span class="sxs-lookup"><span data-stu-id="07e5b-250">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="07e5b-251">упдатеверсион</span><span class="sxs-lookup"><span data-stu-id="07e5b-251">updateVersion</span></span>|<span data-ttu-id="07e5b-252">String</span><span class="sxs-lookup"><span data-stu-id="07e5b-252">String</span></span>|<span data-ttu-id="07e5b-253">Свойство для представления версии обновления, в которой определенная Целевая версия доступна для набора приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="07e5b-253">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="07e5b-254">оффицеконфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="07e5b-254">officeConfigurationXml</span></span>|<span data-ttu-id="07e5b-255">Binary</span><span class="sxs-lookup"><span data-stu-id="07e5b-255">Binary</span></span>|<span data-ttu-id="07e5b-256">Свойство, представляющее XML-файл конфигурации, который можно указать для приложений Office профессиональный плюс.</span><span class="sxs-lookup"><span data-stu-id="07e5b-256">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="07e5b-257">Имеет приоритет над всеми другими свойствами.</span><span class="sxs-lookup"><span data-stu-id="07e5b-257">Takes precedence over all other properties.</span></span> <span data-ttu-id="07e5b-258">Если этот параметр указан, для создания приложения будет использоваться XML-файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="07e5b-258">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="07e5b-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="07e5b-259">Response</span></span>
<span data-ttu-id="07e5b-260">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07e5b-260">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07e5b-261">Пример</span><span class="sxs-lookup"><span data-stu-id="07e5b-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="07e5b-262">Запрос</span><span class="sxs-lookup"><span data-stu-id="07e5b-262">Request</span></span>
<span data-ttu-id="07e5b-263">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07e5b-263">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1675

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "bing": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="07e5b-264">Отклик</span><span class="sxs-lookup"><span data-stu-id="07e5b-264">Response</span></span>
<span data-ttu-id="07e5b-p127">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07e5b-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1847

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "bing": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```






