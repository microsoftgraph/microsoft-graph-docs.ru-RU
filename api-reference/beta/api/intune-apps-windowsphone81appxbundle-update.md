---
title: Обновление windowsPhone81AppXBundle
description: Обновление свойств объекта WindowsPhone81AppXBundle.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 234b216b4996cbeafc0191ec2c2d19654df8da16
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865777"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="f3942-103">Обновление windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="f3942-103">Update windowsPhone81AppXBundle</span></span>

<span data-ttu-id="f3942-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3942-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3942-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3942-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3942-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3942-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3942-107">Обновление свойств объекта [WindowsPhone81AppXBundle.](../resources/intune-apps-windowsphone81appxbundle.md)</span><span class="sxs-lookup"><span data-stu-id="f3942-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3942-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3942-108">Prerequisites</span></span>
<span data-ttu-id="f3942-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3942-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3942-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3942-111">Permission type</span></span>|<span data-ttu-id="f3942-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3942-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3942-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3942-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3942-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3942-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3942-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3942-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3942-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3942-116">Not supported.</span></span>|
|<span data-ttu-id="f3942-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f3942-117">Application</span></span>|<span data-ttu-id="f3942-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3942-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3942-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3942-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f3942-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3942-120">Request headers</span></span>
|<span data-ttu-id="f3942-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3942-121">Header</span></span>|<span data-ttu-id="f3942-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3942-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3942-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f3942-123">Authorization</span></span>|<span data-ttu-id="f3942-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3942-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3942-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3942-125">Accept</span></span>|<span data-ttu-id="f3942-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3942-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3942-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3942-127">Request body</span></span>
<span data-ttu-id="f3942-128">В теле запроса поставляем представление JSON для [объекта WindowsPhone81AppXBundle.](../resources/intune-apps-windowsphone81appxbundle.md)</span><span class="sxs-lookup"><span data-stu-id="f3942-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="f3942-129">В следующей таблице показаны свойства, необходимые при создании [windowsPhone81AppXBundle.](../resources/intune-apps-windowsphone81appxbundle.md)</span><span class="sxs-lookup"><span data-stu-id="f3942-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="f3942-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3942-130">Property</span></span>|<span data-ttu-id="f3942-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f3942-131">Type</span></span>|<span data-ttu-id="f3942-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f3942-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3942-133">id</span><span class="sxs-lookup"><span data-stu-id="f3942-133">id</span></span>|<span data-ttu-id="f3942-134">String</span><span class="sxs-lookup"><span data-stu-id="f3942-134">String</span></span>|<span data-ttu-id="f3942-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f3942-135">Key of the entity.</span></span> <span data-ttu-id="f3942-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f3942-137">displayName</span></span>|<span data-ttu-id="f3942-138">String</span><span class="sxs-lookup"><span data-stu-id="f3942-138">String</span></span>|<span data-ttu-id="f3942-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="f3942-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f3942-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-141">description</span><span class="sxs-lookup"><span data-stu-id="f3942-141">description</span></span>|<span data-ttu-id="f3942-142">String</span><span class="sxs-lookup"><span data-stu-id="f3942-142">String</span></span>|<span data-ttu-id="f3942-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f3942-143">The description of the app.</span></span> <span data-ttu-id="f3942-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f3942-145">publisher</span></span>|<span data-ttu-id="f3942-146">String</span><span class="sxs-lookup"><span data-stu-id="f3942-146">String</span></span>|<span data-ttu-id="f3942-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f3942-147">The publisher of the app.</span></span> <span data-ttu-id="f3942-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f3942-149">largeIcon</span></span>|[<span data-ttu-id="f3942-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f3942-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f3942-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f3942-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f3942-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3942-153">createdDateTime</span></span>|<span data-ttu-id="f3942-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3942-154">DateTimeOffset</span></span>|<span data-ttu-id="f3942-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f3942-155">The date and time the app was created.</span></span> <span data-ttu-id="f3942-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3942-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f3942-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3942-158">DateTimeOffset</span></span>|<span data-ttu-id="f3942-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f3942-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f3942-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f3942-161">isFeatured</span></span>|<span data-ttu-id="f3942-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3942-162">Boolean</span></span>|<span data-ttu-id="f3942-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f3942-164">privacyInformationUrl</span></span>|<span data-ttu-id="f3942-165">String</span><span class="sxs-lookup"><span data-stu-id="f3942-165">String</span></span>|<span data-ttu-id="f3942-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f3942-166">The privacy statement Url.</span></span> <span data-ttu-id="f3942-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f3942-168">informationUrl</span></span>|<span data-ttu-id="f3942-169">String</span><span class="sxs-lookup"><span data-stu-id="f3942-169">String</span></span>|<span data-ttu-id="f3942-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f3942-170">The more information Url.</span></span> <span data-ttu-id="f3942-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-172">owner</span><span class="sxs-lookup"><span data-stu-id="f3942-172">owner</span></span>|<span data-ttu-id="f3942-173">String</span><span class="sxs-lookup"><span data-stu-id="f3942-173">String</span></span>|<span data-ttu-id="f3942-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f3942-174">The owner of the app.</span></span> <span data-ttu-id="f3942-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-176">developer</span><span class="sxs-lookup"><span data-stu-id="f3942-176">developer</span></span>|<span data-ttu-id="f3942-177">String</span><span class="sxs-lookup"><span data-stu-id="f3942-177">String</span></span>|<span data-ttu-id="f3942-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f3942-178">The developer of the app.</span></span> <span data-ttu-id="f3942-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-180">notes</span><span class="sxs-lookup"><span data-stu-id="f3942-180">notes</span></span>|<span data-ttu-id="f3942-181">String</span><span class="sxs-lookup"><span data-stu-id="f3942-181">String</span></span>|<span data-ttu-id="f3942-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="f3942-182">Notes for the app.</span></span> <span data-ttu-id="f3942-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f3942-184">uploadState</span></span>|<span data-ttu-id="f3942-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f3942-185">Int32</span></span>|<span data-ttu-id="f3942-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="f3942-186">The upload state.</span></span> <span data-ttu-id="f3942-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="f3942-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="f3942-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="f3942-189">publishingState</span></span>|[<span data-ttu-id="f3942-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f3942-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f3942-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="f3942-191">The publishing state for the app.</span></span> <span data-ttu-id="f3942-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f3942-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f3942-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f3942-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f3942-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f3942-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f3942-195">isAssigned</span></span>|<span data-ttu-id="f3942-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3942-196">Boolean</span></span>|<span data-ttu-id="f3942-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="f3942-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f3942-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f3942-199">roleScopeTagIds</span></span>|<span data-ttu-id="f3942-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f3942-200">String collection</span></span>|<span data-ttu-id="f3942-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f3942-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f3942-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f3942-203">dependentAppCount</span></span>|<span data-ttu-id="f3942-204">Int32</span><span class="sxs-lookup"><span data-stu-id="f3942-204">Int32</span></span>|<span data-ttu-id="f3942-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="f3942-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f3942-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="f3942-207">supersedingAppCount</span></span>|<span data-ttu-id="f3942-208">Int32</span><span class="sxs-lookup"><span data-stu-id="f3942-208">Int32</span></span>|<span data-ttu-id="f3942-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="f3942-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="f3942-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="f3942-211">supersededAppCount</span></span>|<span data-ttu-id="f3942-212">Int32</span><span class="sxs-lookup"><span data-stu-id="f3942-212">Int32</span></span>|<span data-ttu-id="f3942-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="f3942-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="f3942-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3942-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f3942-215">committedContentVersion</span></span>|<span data-ttu-id="f3942-216">String</span><span class="sxs-lookup"><span data-stu-id="f3942-216">String</span></span>|<span data-ttu-id="f3942-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="f3942-217">The internal committed content version.</span></span> <span data-ttu-id="f3942-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f3942-219">fileName</span><span class="sxs-lookup"><span data-stu-id="f3942-219">fileName</span></span>|<span data-ttu-id="f3942-220">String</span><span class="sxs-lookup"><span data-stu-id="f3942-220">String</span></span>|<span data-ttu-id="f3942-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="f3942-221">The name of the main Lob application file.</span></span> <span data-ttu-id="f3942-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f3942-223">size</span><span class="sxs-lookup"><span data-stu-id="f3942-223">size</span></span>|<span data-ttu-id="f3942-224">Int64</span><span class="sxs-lookup"><span data-stu-id="f3942-224">Int64</span></span>|<span data-ttu-id="f3942-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="f3942-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="f3942-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f3942-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="f3942-227">applicableArchitectures</span></span>|[<span data-ttu-id="f3942-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="f3942-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="f3942-229">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="f3942-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="f3942-230">Унаследовано от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="f3942-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="f3942-231">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="f3942-231">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="f3942-232">identityName</span><span class="sxs-lookup"><span data-stu-id="f3942-232">identityName</span></span>|<span data-ttu-id="f3942-233">String</span><span class="sxs-lookup"><span data-stu-id="f3942-233">String</span></span>|<span data-ttu-id="f3942-234">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f3942-234">The Identity Name.</span></span> <span data-ttu-id="f3942-235">Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="f3942-235">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="f3942-236">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="f3942-236">identityPublisherHash</span></span>|<span data-ttu-id="f3942-237">String</span><span class="sxs-lookup"><span data-stu-id="f3942-237">String</span></span>|<span data-ttu-id="f3942-238">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="f3942-238">The Identity Publisher Hash.</span></span> <span data-ttu-id="f3942-239">Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="f3942-239">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="f3942-240">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f3942-240">identityResourceIdentifier</span></span>|<span data-ttu-id="f3942-241">String</span><span class="sxs-lookup"><span data-stu-id="f3942-241">String</span></span>|<span data-ttu-id="f3942-242">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="f3942-242">The Identity Resource Identifier.</span></span> <span data-ttu-id="f3942-243">Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="f3942-243">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="f3942-244">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f3942-244">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f3942-245">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f3942-245">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="f3942-246">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="f3942-246">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="f3942-247">Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="f3942-247">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="f3942-248">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="f3942-248">phoneProductIdentifier</span></span>|<span data-ttu-id="f3942-249">String</span><span class="sxs-lookup"><span data-stu-id="f3942-249">String</span></span>|<span data-ttu-id="f3942-250">Идентификатор продукта phone.</span><span class="sxs-lookup"><span data-stu-id="f3942-250">The Phone Product Identifier.</span></span> <span data-ttu-id="f3942-251">Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="f3942-251">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="f3942-252">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="f3942-252">phonePublisherId</span></span>|<span data-ttu-id="f3942-253">String</span><span class="sxs-lookup"><span data-stu-id="f3942-253">String</span></span>|<span data-ttu-id="f3942-254">Id издателя телефона. Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="f3942-254">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="f3942-255">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f3942-255">identityVersion</span></span>|<span data-ttu-id="f3942-256">String</span><span class="sxs-lookup"><span data-stu-id="f3942-256">String</span></span>|<span data-ttu-id="f3942-257">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f3942-257">The identity version.</span></span> <span data-ttu-id="f3942-258">Унаследованный от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="f3942-258">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="f3942-259">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="f3942-259">appXPackageInformationList</span></span>|<span data-ttu-id="f3942-260">[коллекция windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="f3942-260">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="f3942-261">Список сведений о пакете AppX.</span><span class="sxs-lookup"><span data-stu-id="f3942-261">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="f3942-262">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3942-262">Response</span></span>
<span data-ttu-id="f3942-263">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f3942-263">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3942-264">Пример</span><span class="sxs-lookup"><span data-stu-id="f3942-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3942-265">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3942-265">Request</span></span>
<span data-ttu-id="f3942-266">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3942-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2518

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
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
    "v10_2004": true,
    "v10_2H20": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
        "v10_2004": true,
        "v10_2H20": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f3942-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3942-267">Response</span></span>
<span data-ttu-id="f3942-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3942-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2690

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
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
    "v10_2004": true,
    "v10_2H20": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
        "v10_2004": true,
        "v10_2H20": true
      }
    }
  ]
}
```




