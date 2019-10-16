---
title: Обновление Андроидфорворкапп
description: Обновление свойств объекта Андроидфорворкапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a10786c42c53965608d45b5cbc45a9dc7f6aa324
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535543"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="8dd25-103">Обновление Андроидфорворкапп</span><span class="sxs-lookup"><span data-stu-id="8dd25-103">Update androidForWorkApp</span></span>

> <span data-ttu-id="8dd25-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dd25-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dd25-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8dd25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dd25-106">Обновление свойств объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8dd25-106">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8dd25-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8dd25-107">Prerequisites</span></span>
<span data-ttu-id="8dd25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dd25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dd25-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8dd25-110">Permission type</span></span>|<span data-ttu-id="8dd25-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8dd25-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dd25-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8dd25-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8dd25-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dd25-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8dd25-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8dd25-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dd25-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8dd25-115">Not supported.</span></span>|
|<span data-ttu-id="8dd25-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8dd25-116">Application</span></span>|<span data-ttu-id="8dd25-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dd25-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dd25-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8dd25-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8dd25-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8dd25-119">Request headers</span></span>
|<span data-ttu-id="8dd25-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8dd25-120">Header</span></span>|<span data-ttu-id="8dd25-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8dd25-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8dd25-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8dd25-122">Authorization</span></span>|<span data-ttu-id="8dd25-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8dd25-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8dd25-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8dd25-124">Accept</span></span>|<span data-ttu-id="8dd25-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8dd25-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dd25-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8dd25-126">Request body</span></span>
<span data-ttu-id="8dd25-127">В тексте запроса добавьте представление объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8dd25-127">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="8dd25-128">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-128">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="8dd25-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8dd25-129">Property</span></span>|<span data-ttu-id="8dd25-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8dd25-130">Type</span></span>|<span data-ttu-id="8dd25-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8dd25-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dd25-132">id</span><span class="sxs-lookup"><span data-stu-id="8dd25-132">id</span></span>|<span data-ttu-id="8dd25-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8dd25-133">String</span></span>|<span data-ttu-id="8dd25-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8dd25-134">Key of the entity.</span></span> <span data-ttu-id="8dd25-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8dd25-136">displayName</span></span>|<span data-ttu-id="8dd25-137">Строка</span><span class="sxs-lookup"><span data-stu-id="8dd25-137">String</span></span>|<span data-ttu-id="8dd25-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="8dd25-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8dd25-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-140">description</span><span class="sxs-lookup"><span data-stu-id="8dd25-140">description</span></span>|<span data-ttu-id="8dd25-141">Строка</span><span class="sxs-lookup"><span data-stu-id="8dd25-141">String</span></span>|<span data-ttu-id="8dd25-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="8dd25-142">The description of the app.</span></span> <span data-ttu-id="8dd25-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-144">publisher</span><span class="sxs-lookup"><span data-stu-id="8dd25-144">publisher</span></span>|<span data-ttu-id="8dd25-145">String</span><span class="sxs-lookup"><span data-stu-id="8dd25-145">String</span></span>|<span data-ttu-id="8dd25-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="8dd25-146">The publisher of the app.</span></span> <span data-ttu-id="8dd25-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8dd25-148">largeIcon</span></span>|[<span data-ttu-id="8dd25-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8dd25-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8dd25-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="8dd25-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8dd25-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8dd25-152">createdDateTime</span></span>|<span data-ttu-id="8dd25-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dd25-153">DateTimeOffset</span></span>|<span data-ttu-id="8dd25-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="8dd25-154">The date and time the app was created.</span></span> <span data-ttu-id="8dd25-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8dd25-156">lastModifiedDateTime</span></span>|<span data-ttu-id="8dd25-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dd25-157">DateTimeOffset</span></span>|<span data-ttu-id="8dd25-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="8dd25-158">The date and time the app was last modified.</span></span> <span data-ttu-id="8dd25-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8dd25-160">isFeatured</span></span>|<span data-ttu-id="8dd25-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dd25-161">Boolean</span></span>|<span data-ttu-id="8dd25-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8dd25-163">privacyInformationUrl</span></span>|<span data-ttu-id="8dd25-164">String</span><span class="sxs-lookup"><span data-stu-id="8dd25-164">String</span></span>|<span data-ttu-id="8dd25-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8dd25-165">The privacy statement Url.</span></span> <span data-ttu-id="8dd25-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8dd25-167">informationUrl</span></span>|<span data-ttu-id="8dd25-168">String</span><span class="sxs-lookup"><span data-stu-id="8dd25-168">String</span></span>|<span data-ttu-id="8dd25-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="8dd25-169">The more information Url.</span></span> <span data-ttu-id="8dd25-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-171">owner</span><span class="sxs-lookup"><span data-stu-id="8dd25-171">owner</span></span>|<span data-ttu-id="8dd25-172">String</span><span class="sxs-lookup"><span data-stu-id="8dd25-172">String</span></span>|<span data-ttu-id="8dd25-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="8dd25-173">The owner of the app.</span></span> <span data-ttu-id="8dd25-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-175">developer</span><span class="sxs-lookup"><span data-stu-id="8dd25-175">developer</span></span>|<span data-ttu-id="8dd25-176">String</span><span class="sxs-lookup"><span data-stu-id="8dd25-176">String</span></span>|<span data-ttu-id="8dd25-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="8dd25-177">The developer of the app.</span></span> <span data-ttu-id="8dd25-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-179">notes</span><span class="sxs-lookup"><span data-stu-id="8dd25-179">notes</span></span>|<span data-ttu-id="8dd25-180">String</span><span class="sxs-lookup"><span data-stu-id="8dd25-180">String</span></span>|<span data-ttu-id="8dd25-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="8dd25-181">Notes for the app.</span></span> <span data-ttu-id="8dd25-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="8dd25-183">uploadState</span></span>|<span data-ttu-id="8dd25-184">Int32</span><span class="sxs-lookup"><span data-stu-id="8dd25-184">Int32</span></span>|<span data-ttu-id="8dd25-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="8dd25-185">The upload state.</span></span> <span data-ttu-id="8dd25-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="8dd25-187">publishingState</span></span>|[<span data-ttu-id="8dd25-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="8dd25-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8dd25-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="8dd25-189">The publishing state for the app.</span></span> <span data-ttu-id="8dd25-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="8dd25-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8dd25-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8dd25-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8dd25-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8dd25-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8dd25-193">isAssigned</span></span>|<span data-ttu-id="8dd25-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dd25-194">Boolean</span></span>|<span data-ttu-id="8dd25-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="8dd25-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8dd25-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8dd25-197">roleScopeTagIds</span></span>|<span data-ttu-id="8dd25-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8dd25-198">String collection</span></span>|<span data-ttu-id="8dd25-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="8dd25-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8dd25-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="8dd25-201">dependentAppCount</span></span>|<span data-ttu-id="8dd25-202">Int32</span><span class="sxs-lookup"><span data-stu-id="8dd25-202">Int32</span></span>|<span data-ttu-id="8dd25-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="8dd25-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8dd25-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8dd25-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8dd25-205">packageId</span><span class="sxs-lookup"><span data-stu-id="8dd25-205">packageId</span></span>|<span data-ttu-id="8dd25-206">String</span><span class="sxs-lookup"><span data-stu-id="8dd25-206">String</span></span>|<span data-ttu-id="8dd25-207">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="8dd25-207">The package identifier.</span></span>|
|<span data-ttu-id="8dd25-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="8dd25-208">appIdentifier</span></span>|<span data-ttu-id="8dd25-209">String</span><span class="sxs-lookup"><span data-stu-id="8dd25-209">String</span></span>|<span data-ttu-id="8dd25-210">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="8dd25-210">The Identity Name.</span></span>|
|<span data-ttu-id="8dd25-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8dd25-211">usedLicenseCount</span></span>|<span data-ttu-id="8dd25-212">Int32</span><span class="sxs-lookup"><span data-stu-id="8dd25-212">Int32</span></span>|<span data-ttu-id="8dd25-213">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="8dd25-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="8dd25-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8dd25-214">totalLicenseCount</span></span>|<span data-ttu-id="8dd25-215">Int32</span><span class="sxs-lookup"><span data-stu-id="8dd25-215">Int32</span></span>|<span data-ttu-id="8dd25-216">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="8dd25-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="8dd25-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8dd25-217">appStoreUrl</span></span>|<span data-ttu-id="8dd25-218">String</span><span class="sxs-lookup"><span data-stu-id="8dd25-218">String</span></span>|<span data-ttu-id="8dd25-219">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="8dd25-219">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="8dd25-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dd25-220">Response</span></span>
<span data-ttu-id="8dd25-221">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8dd25-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dd25-222">Пример</span><span class="sxs-lookup"><span data-stu-id="8dd25-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="8dd25-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="8dd25-223">Request</span></span>
<span data-ttu-id="8dd25-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8dd25-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8dd25-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="8dd25-225">Response</span></span>
<span data-ttu-id="8dd25-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8dd25-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






