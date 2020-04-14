---
title: Обновление Андроидфорворкапп
description: Обновление свойств объекта Андроидфорворкапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 90b162629711ff6fa120552dde36dc0447f93321
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417766"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="f3419-103">Обновление Андроидфорворкапп</span><span class="sxs-lookup"><span data-stu-id="f3419-103">Update androidForWorkApp</span></span>

<span data-ttu-id="f3419-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3419-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3419-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3419-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3419-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3419-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3419-107">Обновление свойств объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f3419-107">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3419-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3419-108">Prerequisites</span></span>
<span data-ttu-id="f3419-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3419-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3419-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3419-111">Permission type</span></span>|<span data-ttu-id="f3419-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3419-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3419-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3419-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3419-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3419-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3419-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3419-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3419-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3419-116">Not supported.</span></span>|
|<span data-ttu-id="f3419-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3419-117">Application</span></span>|<span data-ttu-id="f3419-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3419-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3419-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3419-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f3419-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3419-120">Request headers</span></span>
|<span data-ttu-id="f3419-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3419-121">Header</span></span>|<span data-ttu-id="f3419-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3419-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3419-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3419-123">Authorization</span></span>|<span data-ttu-id="f3419-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3419-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3419-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3419-125">Accept</span></span>|<span data-ttu-id="f3419-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3419-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3419-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3419-127">Request body</span></span>
<span data-ttu-id="f3419-128">В тексте запроса добавьте представление объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3419-128">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="f3419-129">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-129">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="f3419-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3419-130">Property</span></span>|<span data-ttu-id="f3419-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f3419-131">Type</span></span>|<span data-ttu-id="f3419-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f3419-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3419-133">id</span><span class="sxs-lookup"><span data-stu-id="f3419-133">id</span></span>|<span data-ttu-id="f3419-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f3419-134">String</span></span>|<span data-ttu-id="f3419-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f3419-135">Key of the entity.</span></span> <span data-ttu-id="f3419-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f3419-137">displayName</span></span>|<span data-ttu-id="f3419-138">Строка</span><span class="sxs-lookup"><span data-stu-id="f3419-138">String</span></span>|<span data-ttu-id="f3419-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="f3419-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f3419-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-141">description</span><span class="sxs-lookup"><span data-stu-id="f3419-141">description</span></span>|<span data-ttu-id="f3419-142">Строка</span><span class="sxs-lookup"><span data-stu-id="f3419-142">String</span></span>|<span data-ttu-id="f3419-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f3419-143">The description of the app.</span></span> <span data-ttu-id="f3419-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f3419-145">publisher</span></span>|<span data-ttu-id="f3419-146">String</span><span class="sxs-lookup"><span data-stu-id="f3419-146">String</span></span>|<span data-ttu-id="f3419-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f3419-147">The publisher of the app.</span></span> <span data-ttu-id="f3419-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f3419-149">largeIcon</span></span>|[<span data-ttu-id="f3419-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f3419-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f3419-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f3419-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f3419-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3419-153">createdDateTime</span></span>|<span data-ttu-id="f3419-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3419-154">DateTimeOffset</span></span>|<span data-ttu-id="f3419-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f3419-155">The date and time the app was created.</span></span> <span data-ttu-id="f3419-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3419-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f3419-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3419-158">DateTimeOffset</span></span>|<span data-ttu-id="f3419-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f3419-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f3419-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f3419-161">isFeatured</span></span>|<span data-ttu-id="f3419-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3419-162">Boolean</span></span>|<span data-ttu-id="f3419-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f3419-164">privacyInformationUrl</span></span>|<span data-ttu-id="f3419-165">String</span><span class="sxs-lookup"><span data-stu-id="f3419-165">String</span></span>|<span data-ttu-id="f3419-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f3419-166">The privacy statement Url.</span></span> <span data-ttu-id="f3419-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f3419-168">informationUrl</span></span>|<span data-ttu-id="f3419-169">String</span><span class="sxs-lookup"><span data-stu-id="f3419-169">String</span></span>|<span data-ttu-id="f3419-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f3419-170">The more information Url.</span></span> <span data-ttu-id="f3419-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-172">owner</span><span class="sxs-lookup"><span data-stu-id="f3419-172">owner</span></span>|<span data-ttu-id="f3419-173">String</span><span class="sxs-lookup"><span data-stu-id="f3419-173">String</span></span>|<span data-ttu-id="f3419-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f3419-174">The owner of the app.</span></span> <span data-ttu-id="f3419-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-176">developer</span><span class="sxs-lookup"><span data-stu-id="f3419-176">developer</span></span>|<span data-ttu-id="f3419-177">String</span><span class="sxs-lookup"><span data-stu-id="f3419-177">String</span></span>|<span data-ttu-id="f3419-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f3419-178">The developer of the app.</span></span> <span data-ttu-id="f3419-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-180">notes</span><span class="sxs-lookup"><span data-stu-id="f3419-180">notes</span></span>|<span data-ttu-id="f3419-181">String</span><span class="sxs-lookup"><span data-stu-id="f3419-181">String</span></span>|<span data-ttu-id="f3419-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="f3419-182">Notes for the app.</span></span> <span data-ttu-id="f3419-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f3419-184">uploadState</span></span>|<span data-ttu-id="f3419-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f3419-185">Int32</span></span>|<span data-ttu-id="f3419-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="f3419-186">The upload state.</span></span> <span data-ttu-id="f3419-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f3419-188">publishingState</span></span>|[<span data-ttu-id="f3419-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="f3419-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f3419-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="f3419-190">The publishing state for the app.</span></span> <span data-ttu-id="f3419-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f3419-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f3419-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f3419-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f3419-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f3419-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f3419-194">isAssigned</span></span>|<span data-ttu-id="f3419-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3419-195">Boolean</span></span>|<span data-ttu-id="f3419-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="f3419-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f3419-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f3419-198">roleScopeTagIds</span></span>|<span data-ttu-id="f3419-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f3419-199">String collection</span></span>|<span data-ttu-id="f3419-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f3419-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f3419-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="f3419-202">dependentAppCount</span></span>|<span data-ttu-id="f3419-203">Int32</span><span class="sxs-lookup"><span data-stu-id="f3419-203">Int32</span></span>|<span data-ttu-id="f3419-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="f3419-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f3419-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3419-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3419-206">packageId</span><span class="sxs-lookup"><span data-stu-id="f3419-206">packageId</span></span>|<span data-ttu-id="f3419-207">String</span><span class="sxs-lookup"><span data-stu-id="f3419-207">String</span></span>|<span data-ttu-id="f3419-208">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="f3419-208">The package identifier.</span></span>|
|<span data-ttu-id="f3419-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="f3419-209">appIdentifier</span></span>|<span data-ttu-id="f3419-210">String</span><span class="sxs-lookup"><span data-stu-id="f3419-210">String</span></span>|<span data-ttu-id="f3419-211">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f3419-211">The Identity Name.</span></span>|
|<span data-ttu-id="f3419-212">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f3419-212">usedLicenseCount</span></span>|<span data-ttu-id="f3419-213">Int32</span><span class="sxs-lookup"><span data-stu-id="f3419-213">Int32</span></span>|<span data-ttu-id="f3419-214">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="f3419-214">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="f3419-215">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f3419-215">totalLicenseCount</span></span>|<span data-ttu-id="f3419-216">Int32</span><span class="sxs-lookup"><span data-stu-id="f3419-216">Int32</span></span>|<span data-ttu-id="f3419-217">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="f3419-217">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="f3419-218">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f3419-218">appStoreUrl</span></span>|<span data-ttu-id="f3419-219">String</span><span class="sxs-lookup"><span data-stu-id="f3419-219">String</span></span>|<span data-ttu-id="f3419-220">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="f3419-220">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="f3419-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3419-221">Response</span></span>
<span data-ttu-id="f3419-222">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3419-222">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3419-223">Пример</span><span class="sxs-lookup"><span data-stu-id="f3419-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3419-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3419-224">Request</span></span>
<span data-ttu-id="f3419-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3419-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 903

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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="f3419-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3419-226">Response</span></span>
<span data-ttu-id="f3419-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3419-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1075

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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```



