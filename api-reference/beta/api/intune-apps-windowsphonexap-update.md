---
title: Обновление windowsPhoneXAP
description: Обновление свойств объекта WindowsPhoneXAP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 35ed34d6ef9fc1224951a1e6961099dfb2c65191
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133775"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="57d65-103">Обновление windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="57d65-103">Update windowsPhoneXAP</span></span>

<span data-ttu-id="57d65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57d65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57d65-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57d65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57d65-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57d65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57d65-107">Обновление свойств объекта [WindowsPhoneXAP.](../resources/intune-apps-windowsphonexap.md)</span><span class="sxs-lookup"><span data-stu-id="57d65-107">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57d65-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="57d65-108">Prerequisites</span></span>
<span data-ttu-id="57d65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57d65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57d65-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57d65-111">Permission type</span></span>|<span data-ttu-id="57d65-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57d65-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57d65-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57d65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57d65-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57d65-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="57d65-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57d65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57d65-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57d65-116">Not supported.</span></span>|
|<span data-ttu-id="57d65-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="57d65-117">Application</span></span>|<span data-ttu-id="57d65-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57d65-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57d65-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57d65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="57d65-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="57d65-120">Request headers</span></span>
|<span data-ttu-id="57d65-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57d65-121">Header</span></span>|<span data-ttu-id="57d65-122">Значение</span><span class="sxs-lookup"><span data-stu-id="57d65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57d65-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="57d65-123">Authorization</span></span>|<span data-ttu-id="57d65-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57d65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57d65-125">Accept</span><span class="sxs-lookup"><span data-stu-id="57d65-125">Accept</span></span>|<span data-ttu-id="57d65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57d65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57d65-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57d65-127">Request body</span></span>
<span data-ttu-id="57d65-128">В теле запроса поставляем представление JSON для [объекта WindowsPhoneXAP.](../resources/intune-apps-windowsphonexap.md)</span><span class="sxs-lookup"><span data-stu-id="57d65-128">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="57d65-129">В следующей таблице показаны свойства, необходимые при создании [windowsPhoneXAP.](../resources/intune-apps-windowsphonexap.md)</span><span class="sxs-lookup"><span data-stu-id="57d65-129">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="57d65-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="57d65-130">Property</span></span>|<span data-ttu-id="57d65-131">Тип</span><span class="sxs-lookup"><span data-stu-id="57d65-131">Type</span></span>|<span data-ttu-id="57d65-132">Описание</span><span class="sxs-lookup"><span data-stu-id="57d65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57d65-133">id</span><span class="sxs-lookup"><span data-stu-id="57d65-133">id</span></span>|<span data-ttu-id="57d65-134">Строка</span><span class="sxs-lookup"><span data-stu-id="57d65-134">String</span></span>|<span data-ttu-id="57d65-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="57d65-135">Key of the entity.</span></span> <span data-ttu-id="57d65-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-137">displayName</span><span class="sxs-lookup"><span data-stu-id="57d65-137">displayName</span></span>|<span data-ttu-id="57d65-138">Строка</span><span class="sxs-lookup"><span data-stu-id="57d65-138">String</span></span>|<span data-ttu-id="57d65-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="57d65-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="57d65-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-141">description</span><span class="sxs-lookup"><span data-stu-id="57d65-141">description</span></span>|<span data-ttu-id="57d65-142">Строка</span><span class="sxs-lookup"><span data-stu-id="57d65-142">String</span></span>|<span data-ttu-id="57d65-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="57d65-143">The description of the app.</span></span> <span data-ttu-id="57d65-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-145">publisher</span><span class="sxs-lookup"><span data-stu-id="57d65-145">publisher</span></span>|<span data-ttu-id="57d65-146">String</span><span class="sxs-lookup"><span data-stu-id="57d65-146">String</span></span>|<span data-ttu-id="57d65-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="57d65-147">The publisher of the app.</span></span> <span data-ttu-id="57d65-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="57d65-149">largeIcon</span></span>|[<span data-ttu-id="57d65-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="57d65-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="57d65-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="57d65-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="57d65-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57d65-153">createdDateTime</span></span>|<span data-ttu-id="57d65-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57d65-154">DateTimeOffset</span></span>|<span data-ttu-id="57d65-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="57d65-155">The date and time the app was created.</span></span> <span data-ttu-id="57d65-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57d65-157">lastModifiedDateTime</span></span>|<span data-ttu-id="57d65-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57d65-158">DateTimeOffset</span></span>|<span data-ttu-id="57d65-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="57d65-159">The date and time the app was last modified.</span></span> <span data-ttu-id="57d65-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="57d65-161">isFeatured</span></span>|<span data-ttu-id="57d65-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="57d65-162">Boolean</span></span>|<span data-ttu-id="57d65-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="57d65-164">privacyInformationUrl</span></span>|<span data-ttu-id="57d65-165">String</span><span class="sxs-lookup"><span data-stu-id="57d65-165">String</span></span>|<span data-ttu-id="57d65-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="57d65-166">The privacy statement Url.</span></span> <span data-ttu-id="57d65-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="57d65-168">informationUrl</span></span>|<span data-ttu-id="57d65-169">String</span><span class="sxs-lookup"><span data-stu-id="57d65-169">String</span></span>|<span data-ttu-id="57d65-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="57d65-170">The more information Url.</span></span> <span data-ttu-id="57d65-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-172">owner</span><span class="sxs-lookup"><span data-stu-id="57d65-172">owner</span></span>|<span data-ttu-id="57d65-173">String</span><span class="sxs-lookup"><span data-stu-id="57d65-173">String</span></span>|<span data-ttu-id="57d65-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="57d65-174">The owner of the app.</span></span> <span data-ttu-id="57d65-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-176">developer</span><span class="sxs-lookup"><span data-stu-id="57d65-176">developer</span></span>|<span data-ttu-id="57d65-177">String</span><span class="sxs-lookup"><span data-stu-id="57d65-177">String</span></span>|<span data-ttu-id="57d65-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="57d65-178">The developer of the app.</span></span> <span data-ttu-id="57d65-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-180">notes</span><span class="sxs-lookup"><span data-stu-id="57d65-180">notes</span></span>|<span data-ttu-id="57d65-181">String</span><span class="sxs-lookup"><span data-stu-id="57d65-181">String</span></span>|<span data-ttu-id="57d65-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="57d65-182">Notes for the app.</span></span> <span data-ttu-id="57d65-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="57d65-184">uploadState</span></span>|<span data-ttu-id="57d65-185">Int32</span><span class="sxs-lookup"><span data-stu-id="57d65-185">Int32</span></span>|<span data-ttu-id="57d65-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="57d65-186">The upload state.</span></span> <span data-ttu-id="57d65-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="57d65-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="57d65-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="57d65-189">publishingState</span></span>|[<span data-ttu-id="57d65-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="57d65-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="57d65-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="57d65-191">The publishing state for the app.</span></span> <span data-ttu-id="57d65-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="57d65-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="57d65-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="57d65-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="57d65-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="57d65-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="57d65-195">isAssigned</span></span>|<span data-ttu-id="57d65-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="57d65-196">Boolean</span></span>|<span data-ttu-id="57d65-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="57d65-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="57d65-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="57d65-199">roleScopeTagIds</span></span>|<span data-ttu-id="57d65-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="57d65-200">String collection</span></span>|<span data-ttu-id="57d65-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="57d65-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="57d65-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="57d65-203">dependentAppCount</span></span>|<span data-ttu-id="57d65-204">Int32</span><span class="sxs-lookup"><span data-stu-id="57d65-204">Int32</span></span>|<span data-ttu-id="57d65-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="57d65-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="57d65-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="57d65-207">supersedingAppCount</span></span>|<span data-ttu-id="57d65-208">Int32</span><span class="sxs-lookup"><span data-stu-id="57d65-208">Int32</span></span>|<span data-ttu-id="57d65-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="57d65-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="57d65-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="57d65-211">supersededAppCount</span></span>|<span data-ttu-id="57d65-212">Int32</span><span class="sxs-lookup"><span data-stu-id="57d65-212">Int32</span></span>|<span data-ttu-id="57d65-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="57d65-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="57d65-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="57d65-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="57d65-215">committedContentVersion</span></span>|<span data-ttu-id="57d65-216">String</span><span class="sxs-lookup"><span data-stu-id="57d65-216">String</span></span>|<span data-ttu-id="57d65-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="57d65-217">The internal committed content version.</span></span> <span data-ttu-id="57d65-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="57d65-219">fileName</span><span class="sxs-lookup"><span data-stu-id="57d65-219">fileName</span></span>|<span data-ttu-id="57d65-220">String</span><span class="sxs-lookup"><span data-stu-id="57d65-220">String</span></span>|<span data-ttu-id="57d65-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="57d65-221">The name of the main Lob application file.</span></span> <span data-ttu-id="57d65-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="57d65-223">size</span><span class="sxs-lookup"><span data-stu-id="57d65-223">size</span></span>|<span data-ttu-id="57d65-224">Int64</span><span class="sxs-lookup"><span data-stu-id="57d65-224">Int64</span></span>|<span data-ttu-id="57d65-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="57d65-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="57d65-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="57d65-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="57d65-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="57d65-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="57d65-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="57d65-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="57d65-229">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="57d65-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="57d65-230">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="57d65-230">productIdentifier</span></span>|<span data-ttu-id="57d65-231">Строка</span><span class="sxs-lookup"><span data-stu-id="57d65-231">String</span></span>|<span data-ttu-id="57d65-232">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="57d65-232">The Product Identifier.</span></span>|
|<span data-ttu-id="57d65-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="57d65-233">identityVersion</span></span>|<span data-ttu-id="57d65-234">String</span><span class="sxs-lookup"><span data-stu-id="57d65-234">String</span></span>|<span data-ttu-id="57d65-235">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="57d65-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="57d65-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="57d65-236">Response</span></span>
<span data-ttu-id="57d65-237">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57d65-237">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57d65-238">Пример</span><span class="sxs-lookup"><span data-stu-id="57d65-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="57d65-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="57d65-239">Request</span></span>
<span data-ttu-id="57d65-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57d65-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1340

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="57d65-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d65-241">Response</span></span>
<span data-ttu-id="57d65-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57d65-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1512

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```




