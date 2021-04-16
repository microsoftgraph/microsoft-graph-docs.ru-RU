---
title: Обновление windowsPhone81AppX
description: Обновление свойств объекта WindowsPhone81AppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92d576a87f8440cb263900dd57b664a358393ee4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51862941"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="c4640-103">Обновление windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="c4640-103">Update windowsPhone81AppX</span></span>

<span data-ttu-id="c4640-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4640-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4640-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4640-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4640-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4640-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4640-107">Обновление свойств объекта [WindowsPhone81AppX.](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="c4640-107">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4640-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c4640-108">Prerequisites</span></span>
<span data-ttu-id="c4640-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4640-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4640-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4640-111">Permission type</span></span>|<span data-ttu-id="c4640-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4640-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4640-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4640-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4640-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4640-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c4640-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4640-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4640-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4640-116">Not supported.</span></span>|
|<span data-ttu-id="c4640-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c4640-117">Application</span></span>|<span data-ttu-id="c4640-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4640-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4640-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4640-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="c4640-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c4640-120">Request headers</span></span>
|<span data-ttu-id="c4640-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4640-121">Header</span></span>|<span data-ttu-id="c4640-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c4640-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4640-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4640-123">Authorization</span></span>|<span data-ttu-id="c4640-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4640-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4640-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c4640-125">Accept</span></span>|<span data-ttu-id="c4640-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4640-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4640-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4640-127">Request body</span></span>
<span data-ttu-id="c4640-128">В теле запроса поставляем представление JSON для [объекта WindowsPhone81AppX.](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="c4640-128">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="c4640-129">В следующей таблице показаны свойства, необходимые при создании [windowsPhone81AppX.](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="c4640-129">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="c4640-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4640-130">Property</span></span>|<span data-ttu-id="c4640-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c4640-131">Type</span></span>|<span data-ttu-id="c4640-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c4640-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4640-133">id</span><span class="sxs-lookup"><span data-stu-id="c4640-133">id</span></span>|<span data-ttu-id="c4640-134">String</span><span class="sxs-lookup"><span data-stu-id="c4640-134">String</span></span>|<span data-ttu-id="c4640-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c4640-135">Key of the entity.</span></span> <span data-ttu-id="c4640-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c4640-137">displayName</span></span>|<span data-ttu-id="c4640-138">String</span><span class="sxs-lookup"><span data-stu-id="c4640-138">String</span></span>|<span data-ttu-id="c4640-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c4640-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c4640-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-141">description</span><span class="sxs-lookup"><span data-stu-id="c4640-141">description</span></span>|<span data-ttu-id="c4640-142">String</span><span class="sxs-lookup"><span data-stu-id="c4640-142">String</span></span>|<span data-ttu-id="c4640-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c4640-143">The description of the app.</span></span> <span data-ttu-id="c4640-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c4640-145">publisher</span></span>|<span data-ttu-id="c4640-146">String</span><span class="sxs-lookup"><span data-stu-id="c4640-146">String</span></span>|<span data-ttu-id="c4640-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c4640-147">The publisher of the app.</span></span> <span data-ttu-id="c4640-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c4640-149">largeIcon</span></span>|[<span data-ttu-id="c4640-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c4640-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c4640-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="c4640-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c4640-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4640-153">createdDateTime</span></span>|<span data-ttu-id="c4640-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4640-154">DateTimeOffset</span></span>|<span data-ttu-id="c4640-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="c4640-155">The date and time the app was created.</span></span> <span data-ttu-id="c4640-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4640-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c4640-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4640-158">DateTimeOffset</span></span>|<span data-ttu-id="c4640-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="c4640-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c4640-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c4640-161">isFeatured</span></span>|<span data-ttu-id="c4640-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4640-162">Boolean</span></span>|<span data-ttu-id="c4640-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c4640-164">privacyInformationUrl</span></span>|<span data-ttu-id="c4640-165">String</span><span class="sxs-lookup"><span data-stu-id="c4640-165">String</span></span>|<span data-ttu-id="c4640-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c4640-166">The privacy statement Url.</span></span> <span data-ttu-id="c4640-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c4640-168">informationUrl</span></span>|<span data-ttu-id="c4640-169">String</span><span class="sxs-lookup"><span data-stu-id="c4640-169">String</span></span>|<span data-ttu-id="c4640-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="c4640-170">The more information Url.</span></span> <span data-ttu-id="c4640-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-172">owner</span><span class="sxs-lookup"><span data-stu-id="c4640-172">owner</span></span>|<span data-ttu-id="c4640-173">String</span><span class="sxs-lookup"><span data-stu-id="c4640-173">String</span></span>|<span data-ttu-id="c4640-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="c4640-174">The owner of the app.</span></span> <span data-ttu-id="c4640-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-176">developer</span><span class="sxs-lookup"><span data-stu-id="c4640-176">developer</span></span>|<span data-ttu-id="c4640-177">String</span><span class="sxs-lookup"><span data-stu-id="c4640-177">String</span></span>|<span data-ttu-id="c4640-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="c4640-178">The developer of the app.</span></span> <span data-ttu-id="c4640-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-180">notes</span><span class="sxs-lookup"><span data-stu-id="c4640-180">notes</span></span>|<span data-ttu-id="c4640-181">String</span><span class="sxs-lookup"><span data-stu-id="c4640-181">String</span></span>|<span data-ttu-id="c4640-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="c4640-182">Notes for the app.</span></span> <span data-ttu-id="c4640-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c4640-184">uploadState</span></span>|<span data-ttu-id="c4640-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c4640-185">Int32</span></span>|<span data-ttu-id="c4640-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="c4640-186">The upload state.</span></span> <span data-ttu-id="c4640-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="c4640-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="c4640-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="c4640-189">publishingState</span></span>|[<span data-ttu-id="c4640-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c4640-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c4640-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="c4640-191">The publishing state for the app.</span></span> <span data-ttu-id="c4640-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="c4640-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c4640-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="c4640-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c4640-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c4640-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c4640-195">isAssigned</span></span>|<span data-ttu-id="c4640-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4640-196">Boolean</span></span>|<span data-ttu-id="c4640-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="c4640-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c4640-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4640-199">roleScopeTagIds</span></span>|<span data-ttu-id="c4640-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c4640-200">String collection</span></span>|<span data-ttu-id="c4640-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="c4640-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c4640-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="c4640-203">dependentAppCount</span></span>|<span data-ttu-id="c4640-204">Int32</span><span class="sxs-lookup"><span data-stu-id="c4640-204">Int32</span></span>|<span data-ttu-id="c4640-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="c4640-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="c4640-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="c4640-207">supersedingAppCount</span></span>|<span data-ttu-id="c4640-208">Int32</span><span class="sxs-lookup"><span data-stu-id="c4640-208">Int32</span></span>|<span data-ttu-id="c4640-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="c4640-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="c4640-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="c4640-211">supersededAppCount</span></span>|<span data-ttu-id="c4640-212">Int32</span><span class="sxs-lookup"><span data-stu-id="c4640-212">Int32</span></span>|<span data-ttu-id="c4640-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="c4640-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="c4640-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c4640-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c4640-215">committedContentVersion</span></span>|<span data-ttu-id="c4640-216">String</span><span class="sxs-lookup"><span data-stu-id="c4640-216">String</span></span>|<span data-ttu-id="c4640-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="c4640-217">The internal committed content version.</span></span> <span data-ttu-id="c4640-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c4640-219">fileName</span><span class="sxs-lookup"><span data-stu-id="c4640-219">fileName</span></span>|<span data-ttu-id="c4640-220">String</span><span class="sxs-lookup"><span data-stu-id="c4640-220">String</span></span>|<span data-ttu-id="c4640-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="c4640-221">The name of the main Lob application file.</span></span> <span data-ttu-id="c4640-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c4640-223">size</span><span class="sxs-lookup"><span data-stu-id="c4640-223">size</span></span>|<span data-ttu-id="c4640-224">Int64</span><span class="sxs-lookup"><span data-stu-id="c4640-224">Int64</span></span>|<span data-ttu-id="c4640-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="c4640-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="c4640-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c4640-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c4640-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="c4640-227">applicableArchitectures</span></span>|[<span data-ttu-id="c4640-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="c4640-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="c4640-229">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="c4640-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="c4640-230">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="c4640-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="c4640-231">identityName</span><span class="sxs-lookup"><span data-stu-id="c4640-231">identityName</span></span>|<span data-ttu-id="c4640-232">String</span><span class="sxs-lookup"><span data-stu-id="c4640-232">String</span></span>|<span data-ttu-id="c4640-233">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c4640-233">The Identity Name.</span></span>|
|<span data-ttu-id="c4640-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="c4640-234">identityPublisherHash</span></span>|<span data-ttu-id="c4640-235">String</span><span class="sxs-lookup"><span data-stu-id="c4640-235">String</span></span>|<span data-ttu-id="c4640-236">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="c4640-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="c4640-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c4640-237">identityResourceIdentifier</span></span>|<span data-ttu-id="c4640-238">String</span><span class="sxs-lookup"><span data-stu-id="c4640-238">String</span></span>|<span data-ttu-id="c4640-239">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="c4640-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="c4640-240">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c4640-240">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c4640-241">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c4640-241">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="c4640-242">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="c4640-242">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c4640-243">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="c4640-243">phoneProductIdentifier</span></span>|<span data-ttu-id="c4640-244">String</span><span class="sxs-lookup"><span data-stu-id="c4640-244">String</span></span>|<span data-ttu-id="c4640-245">Идентификатор продукта phone.</span><span class="sxs-lookup"><span data-stu-id="c4640-245">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="c4640-246">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="c4640-246">phonePublisherId</span></span>|<span data-ttu-id="c4640-247">String</span><span class="sxs-lookup"><span data-stu-id="c4640-247">String</span></span>|<span data-ttu-id="c4640-248">ID издателя телефонов.</span><span class="sxs-lookup"><span data-stu-id="c4640-248">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="c4640-249">identityVersion</span><span class="sxs-lookup"><span data-stu-id="c4640-249">identityVersion</span></span>|<span data-ttu-id="c4640-250">String</span><span class="sxs-lookup"><span data-stu-id="c4640-250">String</span></span>|<span data-ttu-id="c4640-251">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c4640-251">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="c4640-252">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4640-252">Response</span></span>
<span data-ttu-id="c4640-253">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4640-253">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4640-254">Пример</span><span class="sxs-lookup"><span data-stu-id="c4640-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4640-255">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4640-255">Request</span></span>
<span data-ttu-id="c4640-256">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4640-256">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1639

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="c4640-257">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4640-257">Response</span></span>
<span data-ttu-id="c4640-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4640-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1811

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
  "identityVersion": "Identity Version value"
}
```




