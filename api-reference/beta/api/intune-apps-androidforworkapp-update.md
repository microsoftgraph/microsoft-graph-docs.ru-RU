---
title: Обновление Андроидфорворкапп
description: Обновление свойств объекта Андроидфорворкапп.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 43aee40395ab9ca4c9f5b4f575e0611e432fc029
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762373"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="6fe38-103">Обновление Андроидфорворкапп</span><span class="sxs-lookup"><span data-stu-id="6fe38-103">Update androidForWorkApp</span></span>

> <span data-ttu-id="6fe38-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fe38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fe38-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6fe38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fe38-106">Обновление свойств объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="6fe38-106">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6fe38-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6fe38-107">Prerequisites</span></span>
<span data-ttu-id="6fe38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fe38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fe38-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fe38-110">Permission type</span></span>|<span data-ttu-id="6fe38-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fe38-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fe38-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fe38-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6fe38-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fe38-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6fe38-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fe38-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fe38-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fe38-115">Not supported.</span></span>|
|<span data-ttu-id="6fe38-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6fe38-116">Application</span></span>|<span data-ttu-id="6fe38-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fe38-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fe38-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fe38-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="6fe38-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6fe38-119">Request headers</span></span>
|<span data-ttu-id="6fe38-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6fe38-120">Header</span></span>|<span data-ttu-id="6fe38-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6fe38-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6fe38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fe38-122">Authorization</span></span>|<span data-ttu-id="6fe38-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fe38-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6fe38-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6fe38-124">Accept</span></span>|<span data-ttu-id="6fe38-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6fe38-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fe38-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6fe38-126">Request body</span></span>
<span data-ttu-id="6fe38-127">В тексте запроса добавьте представление объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fe38-127">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="6fe38-128">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-128">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="6fe38-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fe38-129">Property</span></span>|<span data-ttu-id="6fe38-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6fe38-130">Type</span></span>|<span data-ttu-id="6fe38-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6fe38-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fe38-132">id</span><span class="sxs-lookup"><span data-stu-id="6fe38-132">id</span></span>|<span data-ttu-id="6fe38-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6fe38-133">String</span></span>|<span data-ttu-id="6fe38-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6fe38-134">Key of the entity.</span></span> <span data-ttu-id="6fe38-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6fe38-136">displayName</span></span>|<span data-ttu-id="6fe38-137">Строка</span><span class="sxs-lookup"><span data-stu-id="6fe38-137">String</span></span>|<span data-ttu-id="6fe38-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="6fe38-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6fe38-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-140">description</span><span class="sxs-lookup"><span data-stu-id="6fe38-140">description</span></span>|<span data-ttu-id="6fe38-141">Строка</span><span class="sxs-lookup"><span data-stu-id="6fe38-141">String</span></span>|<span data-ttu-id="6fe38-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="6fe38-142">The description of the app.</span></span> <span data-ttu-id="6fe38-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-144">publisher</span><span class="sxs-lookup"><span data-stu-id="6fe38-144">publisher</span></span>|<span data-ttu-id="6fe38-145">String</span><span class="sxs-lookup"><span data-stu-id="6fe38-145">String</span></span>|<span data-ttu-id="6fe38-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="6fe38-146">The publisher of the app.</span></span> <span data-ttu-id="6fe38-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6fe38-148">largeIcon</span></span>|[<span data-ttu-id="6fe38-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6fe38-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6fe38-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="6fe38-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6fe38-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fe38-152">createdDateTime</span></span>|<span data-ttu-id="6fe38-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fe38-153">DateTimeOffset</span></span>|<span data-ttu-id="6fe38-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="6fe38-154">The date and time the app was created.</span></span> <span data-ttu-id="6fe38-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fe38-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6fe38-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fe38-157">DateTimeOffset</span></span>|<span data-ttu-id="6fe38-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="6fe38-158">The date and time the app was last modified.</span></span> <span data-ttu-id="6fe38-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6fe38-160">isFeatured</span></span>|<span data-ttu-id="6fe38-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fe38-161">Boolean</span></span>|<span data-ttu-id="6fe38-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6fe38-163">privacyInformationUrl</span></span>|<span data-ttu-id="6fe38-164">String</span><span class="sxs-lookup"><span data-stu-id="6fe38-164">String</span></span>|<span data-ttu-id="6fe38-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="6fe38-165">The privacy statement Url.</span></span> <span data-ttu-id="6fe38-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6fe38-167">informationUrl</span></span>|<span data-ttu-id="6fe38-168">String</span><span class="sxs-lookup"><span data-stu-id="6fe38-168">String</span></span>|<span data-ttu-id="6fe38-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="6fe38-169">The more information Url.</span></span> <span data-ttu-id="6fe38-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-171">owner</span><span class="sxs-lookup"><span data-stu-id="6fe38-171">owner</span></span>|<span data-ttu-id="6fe38-172">String</span><span class="sxs-lookup"><span data-stu-id="6fe38-172">String</span></span>|<span data-ttu-id="6fe38-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="6fe38-173">The owner of the app.</span></span> <span data-ttu-id="6fe38-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-175">developer</span><span class="sxs-lookup"><span data-stu-id="6fe38-175">developer</span></span>|<span data-ttu-id="6fe38-176">String</span><span class="sxs-lookup"><span data-stu-id="6fe38-176">String</span></span>|<span data-ttu-id="6fe38-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="6fe38-177">The developer of the app.</span></span> <span data-ttu-id="6fe38-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-179">notes</span><span class="sxs-lookup"><span data-stu-id="6fe38-179">notes</span></span>|<span data-ttu-id="6fe38-180">String</span><span class="sxs-lookup"><span data-stu-id="6fe38-180">String</span></span>|<span data-ttu-id="6fe38-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="6fe38-181">Notes for the app.</span></span> <span data-ttu-id="6fe38-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="6fe38-183">uploadState</span></span>|<span data-ttu-id="6fe38-184">Int32</span><span class="sxs-lookup"><span data-stu-id="6fe38-184">Int32</span></span>|<span data-ttu-id="6fe38-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="6fe38-185">The upload state.</span></span> <span data-ttu-id="6fe38-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="6fe38-187">publishingState</span></span>|[<span data-ttu-id="6fe38-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="6fe38-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6fe38-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="6fe38-189">The publishing state for the app.</span></span> <span data-ttu-id="6fe38-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="6fe38-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6fe38-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="6fe38-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6fe38-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6fe38-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6fe38-193">isAssigned</span></span>|<span data-ttu-id="6fe38-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6fe38-194">Boolean</span></span>|<span data-ttu-id="6fe38-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="6fe38-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6fe38-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6fe38-197">roleScopeTagIds</span></span>|<span data-ttu-id="6fe38-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6fe38-198">String collection</span></span>|<span data-ttu-id="6fe38-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="6fe38-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6fe38-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="6fe38-201">dependentAppCount</span></span>|<span data-ttu-id="6fe38-202">Int32</span><span class="sxs-lookup"><span data-stu-id="6fe38-202">Int32</span></span>|<span data-ttu-id="6fe38-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="6fe38-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6fe38-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6fe38-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6fe38-205">packageId</span><span class="sxs-lookup"><span data-stu-id="6fe38-205">packageId</span></span>|<span data-ttu-id="6fe38-206">String</span><span class="sxs-lookup"><span data-stu-id="6fe38-206">String</span></span>|<span data-ttu-id="6fe38-207">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="6fe38-207">The package identifier.</span></span>|
|<span data-ttu-id="6fe38-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="6fe38-208">appIdentifier</span></span>|<span data-ttu-id="6fe38-209">String</span><span class="sxs-lookup"><span data-stu-id="6fe38-209">String</span></span>|<span data-ttu-id="6fe38-210">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="6fe38-210">The Identity Name.</span></span>|
|<span data-ttu-id="6fe38-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6fe38-211">usedLicenseCount</span></span>|<span data-ttu-id="6fe38-212">Int32</span><span class="sxs-lookup"><span data-stu-id="6fe38-212">Int32</span></span>|<span data-ttu-id="6fe38-213">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="6fe38-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="6fe38-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6fe38-214">totalLicenseCount</span></span>|<span data-ttu-id="6fe38-215">Int32</span><span class="sxs-lookup"><span data-stu-id="6fe38-215">Int32</span></span>|<span data-ttu-id="6fe38-216">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="6fe38-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="6fe38-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6fe38-217">appStoreUrl</span></span>|<span data-ttu-id="6fe38-218">String</span><span class="sxs-lookup"><span data-stu-id="6fe38-218">String</span></span>|<span data-ttu-id="6fe38-219">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="6fe38-219">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="6fe38-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fe38-220">Response</span></span>
<span data-ttu-id="6fe38-221">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6fe38-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6fe38-222">Пример</span><span class="sxs-lookup"><span data-stu-id="6fe38-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fe38-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fe38-223">Request</span></span>
<span data-ttu-id="6fe38-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6fe38-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6fe38-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fe38-225">Response</span></span>
<span data-ttu-id="6fe38-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6fe38-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




