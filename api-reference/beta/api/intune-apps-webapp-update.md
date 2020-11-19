---
title: Update webApp
description: Обновление свойств объекта webApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b79d6e177ad779d7e383dcd716063d2df5898cd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247428"
---
# <a name="update-webapp"></a><span data-ttu-id="9ac0b-103">Update webApp</span><span class="sxs-lookup"><span data-stu-id="9ac0b-103">Update webApp</span></span>

<span data-ttu-id="9ac0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ac0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ac0b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ac0b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ac0b-107">Обновление свойств объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-107">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ac0b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9ac0b-108">Prerequisites</span></span>
<span data-ttu-id="9ac0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ac0b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ac0b-111">Permission type</span></span>|<span data-ttu-id="9ac0b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ac0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ac0b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ac0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ac0b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ac0b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ac0b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ac0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ac0b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-116">Not supported.</span></span>|
|<span data-ttu-id="9ac0b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9ac0b-117">Application</span></span>|<span data-ttu-id="9ac0b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ac0b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ac0b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ac0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9ac0b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9ac0b-120">Request headers</span></span>
|<span data-ttu-id="9ac0b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ac0b-121">Header</span></span>|<span data-ttu-id="9ac0b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9ac0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ac0b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ac0b-123">Authorization</span></span>|<span data-ttu-id="9ac0b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ac0b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9ac0b-125">Accept</span></span>|<span data-ttu-id="9ac0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ac0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ac0b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ac0b-127">Request body</span></span>
<span data-ttu-id="9ac0b-128">В тексте запроса добавьте представление объекта [webApp](../resources/intune-apps-webapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-128">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="9ac0b-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-129">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="9ac0b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ac0b-130">Property</span></span>|<span data-ttu-id="9ac0b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9ac0b-131">Type</span></span>|<span data-ttu-id="9ac0b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9ac0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ac0b-133">id</span><span class="sxs-lookup"><span data-stu-id="9ac0b-133">id</span></span>|<span data-ttu-id="9ac0b-134">String</span><span class="sxs-lookup"><span data-stu-id="9ac0b-134">String</span></span>|<span data-ttu-id="9ac0b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-135">Key of the entity.</span></span> <span data-ttu-id="9ac0b-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9ac0b-137">displayName</span></span>|<span data-ttu-id="9ac0b-138">String</span><span class="sxs-lookup"><span data-stu-id="9ac0b-138">String</span></span>|<span data-ttu-id="9ac0b-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9ac0b-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-141">description</span><span class="sxs-lookup"><span data-stu-id="9ac0b-141">description</span></span>|<span data-ttu-id="9ac0b-142">String</span><span class="sxs-lookup"><span data-stu-id="9ac0b-142">String</span></span>|<span data-ttu-id="9ac0b-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-143">The description of the app.</span></span> <span data-ttu-id="9ac0b-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-145">publisher</span><span class="sxs-lookup"><span data-stu-id="9ac0b-145">publisher</span></span>|<span data-ttu-id="9ac0b-146">String</span><span class="sxs-lookup"><span data-stu-id="9ac0b-146">String</span></span>|<span data-ttu-id="9ac0b-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-147">The publisher of the app.</span></span> <span data-ttu-id="9ac0b-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9ac0b-149">largeIcon</span></span>|[<span data-ttu-id="9ac0b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ac0b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9ac0b-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9ac0b-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac0b-153">createdDateTime</span></span>|<span data-ttu-id="9ac0b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac0b-154">DateTimeOffset</span></span>|<span data-ttu-id="9ac0b-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-155">The date and time the app was created.</span></span> <span data-ttu-id="9ac0b-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac0b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9ac0b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac0b-158">DateTimeOffset</span></span>|<span data-ttu-id="9ac0b-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9ac0b-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9ac0b-161">isFeatured</span></span>|<span data-ttu-id="9ac0b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ac0b-162">Boolean</span></span>|<span data-ttu-id="9ac0b-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9ac0b-164">privacyInformationUrl</span></span>|<span data-ttu-id="9ac0b-165">String</span><span class="sxs-lookup"><span data-stu-id="9ac0b-165">String</span></span>|<span data-ttu-id="9ac0b-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-166">The privacy statement Url.</span></span> <span data-ttu-id="9ac0b-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9ac0b-168">informationUrl</span></span>|<span data-ttu-id="9ac0b-169">String</span><span class="sxs-lookup"><span data-stu-id="9ac0b-169">String</span></span>|<span data-ttu-id="9ac0b-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-170">The more information Url.</span></span> <span data-ttu-id="9ac0b-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-172">owner</span><span class="sxs-lookup"><span data-stu-id="9ac0b-172">owner</span></span>|<span data-ttu-id="9ac0b-173">String</span><span class="sxs-lookup"><span data-stu-id="9ac0b-173">String</span></span>|<span data-ttu-id="9ac0b-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-174">The owner of the app.</span></span> <span data-ttu-id="9ac0b-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-176">developer</span><span class="sxs-lookup"><span data-stu-id="9ac0b-176">developer</span></span>|<span data-ttu-id="9ac0b-177">String</span><span class="sxs-lookup"><span data-stu-id="9ac0b-177">String</span></span>|<span data-ttu-id="9ac0b-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-178">The developer of the app.</span></span> <span data-ttu-id="9ac0b-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-180">notes</span><span class="sxs-lookup"><span data-stu-id="9ac0b-180">notes</span></span>|<span data-ttu-id="9ac0b-181">String</span><span class="sxs-lookup"><span data-stu-id="9ac0b-181">String</span></span>|<span data-ttu-id="9ac0b-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-182">Notes for the app.</span></span> <span data-ttu-id="9ac0b-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9ac0b-184">uploadState</span></span>|<span data-ttu-id="9ac0b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9ac0b-185">Int32</span></span>|<span data-ttu-id="9ac0b-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-186">The upload state.</span></span> <span data-ttu-id="9ac0b-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="9ac0b-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="9ac0b-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="9ac0b-189">publishingState</span></span>|[<span data-ttu-id="9ac0b-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9ac0b-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9ac0b-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-191">The publishing state for the app.</span></span> <span data-ttu-id="9ac0b-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9ac0b-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="9ac0b-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9ac0b-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9ac0b-195">isAssigned</span></span>|<span data-ttu-id="9ac0b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ac0b-196">Boolean</span></span>|<span data-ttu-id="9ac0b-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9ac0b-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ac0b-199">roleScopeTagIds</span></span>|<span data-ttu-id="9ac0b-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9ac0b-200">String collection</span></span>|<span data-ttu-id="9ac0b-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9ac0b-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="9ac0b-203">dependentAppCount</span></span>|<span data-ttu-id="9ac0b-204">Int32</span><span class="sxs-lookup"><span data-stu-id="9ac0b-204">Int32</span></span>|<span data-ttu-id="9ac0b-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9ac0b-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="9ac0b-207">supersedingAppCount</span></span>|<span data-ttu-id="9ac0b-208">Int32</span><span class="sxs-lookup"><span data-stu-id="9ac0b-208">Int32</span></span>|<span data-ttu-id="9ac0b-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="9ac0b-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="9ac0b-211">supersededAppCount</span></span>|<span data-ttu-id="9ac0b-212">Int32</span><span class="sxs-lookup"><span data-stu-id="9ac0b-212">Int32</span></span>|<span data-ttu-id="9ac0b-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="9ac0b-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ac0b-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ac0b-215">appUrl</span><span class="sxs-lookup"><span data-stu-id="9ac0b-215">appUrl</span></span>|<span data-ttu-id="9ac0b-216">String</span><span class="sxs-lookup"><span data-stu-id="9ac0b-216">String</span></span>|<span data-ttu-id="9ac0b-217">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-217">The web app URL.</span></span>|
|<span data-ttu-id="9ac0b-218">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="9ac0b-218">useManagedBrowser</span></span>|<span data-ttu-id="9ac0b-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ac0b-219">Boolean</span></span>|<span data-ttu-id="9ac0b-220">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-220">Whether or not to use managed browser.</span></span> <span data-ttu-id="9ac0b-221">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-221">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="9ac0b-222">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ac0b-222">Response</span></span>
<span data-ttu-id="9ac0b-223">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [webApp](../resources/intune-apps-webapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-223">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ac0b-224">Пример</span><span class="sxs-lookup"><span data-stu-id="9ac0b-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ac0b-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ac0b-225">Request</span></span>
<span data-ttu-id="9ac0b-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 836

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="9ac0b-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ac0b-227">Response</span></span>
<span data-ttu-id="9ac0b-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ac0b-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1008

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```




