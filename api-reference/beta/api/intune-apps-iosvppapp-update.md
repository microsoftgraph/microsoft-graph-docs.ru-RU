---
title: Update iosVppApp
description: Обновление свойств объекта iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f7d3f27c4304fa7b2becd5ed3db4801b80a3c963
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43416732"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="92f64-103">Update iosVppApp</span><span class="sxs-lookup"><span data-stu-id="92f64-103">Update iosVppApp</span></span>

<span data-ttu-id="92f64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92f64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92f64-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92f64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92f64-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92f64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92f64-107">Обновление свойств объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-107">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92f64-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="92f64-108">Prerequisites</span></span>
<span data-ttu-id="92f64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92f64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92f64-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92f64-111">Permission type</span></span>|<span data-ttu-id="92f64-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92f64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92f64-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92f64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92f64-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92f64-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="92f64-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92f64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92f64-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92f64-116">Not supported.</span></span>|
|<span data-ttu-id="92f64-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92f64-117">Application</span></span>|<span data-ttu-id="92f64-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92f64-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92f64-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92f64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="92f64-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92f64-120">Request headers</span></span>
|<span data-ttu-id="92f64-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92f64-121">Header</span></span>|<span data-ttu-id="92f64-122">Значение</span><span class="sxs-lookup"><span data-stu-id="92f64-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92f64-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92f64-123">Authorization</span></span>|<span data-ttu-id="92f64-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92f64-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92f64-125">Accept</span><span class="sxs-lookup"><span data-stu-id="92f64-125">Accept</span></span>|<span data-ttu-id="92f64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92f64-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92f64-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="92f64-127">Request body</span></span>
<span data-ttu-id="92f64-128">В теле запроса добавьте представление объекта [iosVppApp](../resources/intune-apps-iosvppapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92f64-128">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="92f64-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-129">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="92f64-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="92f64-130">Property</span></span>|<span data-ttu-id="92f64-131">Тип</span><span class="sxs-lookup"><span data-stu-id="92f64-131">Type</span></span>|<span data-ttu-id="92f64-132">Описание</span><span class="sxs-lookup"><span data-stu-id="92f64-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92f64-133">id</span><span class="sxs-lookup"><span data-stu-id="92f64-133">id</span></span>|<span data-ttu-id="92f64-134">String</span><span class="sxs-lookup"><span data-stu-id="92f64-134">String</span></span>|<span data-ttu-id="92f64-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="92f64-135">Key of the entity.</span></span> <span data-ttu-id="92f64-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-137">displayName</span><span class="sxs-lookup"><span data-stu-id="92f64-137">displayName</span></span>|<span data-ttu-id="92f64-138">Строка</span><span class="sxs-lookup"><span data-stu-id="92f64-138">String</span></span>|<span data-ttu-id="92f64-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="92f64-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="92f64-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-141">description</span><span class="sxs-lookup"><span data-stu-id="92f64-141">description</span></span>|<span data-ttu-id="92f64-142">Строка</span><span class="sxs-lookup"><span data-stu-id="92f64-142">String</span></span>|<span data-ttu-id="92f64-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="92f64-143">The description of the app.</span></span> <span data-ttu-id="92f64-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-145">publisher</span><span class="sxs-lookup"><span data-stu-id="92f64-145">publisher</span></span>|<span data-ttu-id="92f64-146">String</span><span class="sxs-lookup"><span data-stu-id="92f64-146">String</span></span>|<span data-ttu-id="92f64-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="92f64-147">The publisher of the app.</span></span> <span data-ttu-id="92f64-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="92f64-149">largeIcon</span></span>|[<span data-ttu-id="92f64-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="92f64-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="92f64-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="92f64-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="92f64-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92f64-153">createdDateTime</span></span>|<span data-ttu-id="92f64-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92f64-154">DateTimeOffset</span></span>|<span data-ttu-id="92f64-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="92f64-155">The date and time the app was created.</span></span> <span data-ttu-id="92f64-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92f64-157">lastModifiedDateTime</span></span>|<span data-ttu-id="92f64-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92f64-158">DateTimeOffset</span></span>|<span data-ttu-id="92f64-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="92f64-159">The date and time the app was last modified.</span></span> <span data-ttu-id="92f64-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="92f64-161">isFeatured</span></span>|<span data-ttu-id="92f64-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="92f64-162">Boolean</span></span>|<span data-ttu-id="92f64-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="92f64-164">privacyInformationUrl</span></span>|<span data-ttu-id="92f64-165">String</span><span class="sxs-lookup"><span data-stu-id="92f64-165">String</span></span>|<span data-ttu-id="92f64-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="92f64-166">The privacy statement Url.</span></span> <span data-ttu-id="92f64-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="92f64-168">informationUrl</span></span>|<span data-ttu-id="92f64-169">String</span><span class="sxs-lookup"><span data-stu-id="92f64-169">String</span></span>|<span data-ttu-id="92f64-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="92f64-170">The more information Url.</span></span> <span data-ttu-id="92f64-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-172">owner</span><span class="sxs-lookup"><span data-stu-id="92f64-172">owner</span></span>|<span data-ttu-id="92f64-173">String</span><span class="sxs-lookup"><span data-stu-id="92f64-173">String</span></span>|<span data-ttu-id="92f64-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="92f64-174">The owner of the app.</span></span> <span data-ttu-id="92f64-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-176">developer</span><span class="sxs-lookup"><span data-stu-id="92f64-176">developer</span></span>|<span data-ttu-id="92f64-177">String</span><span class="sxs-lookup"><span data-stu-id="92f64-177">String</span></span>|<span data-ttu-id="92f64-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="92f64-178">The developer of the app.</span></span> <span data-ttu-id="92f64-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-180">notes</span><span class="sxs-lookup"><span data-stu-id="92f64-180">notes</span></span>|<span data-ttu-id="92f64-181">String</span><span class="sxs-lookup"><span data-stu-id="92f64-181">String</span></span>|<span data-ttu-id="92f64-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="92f64-182">Notes for the app.</span></span> <span data-ttu-id="92f64-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="92f64-184">uploadState</span></span>|<span data-ttu-id="92f64-185">Int32</span><span class="sxs-lookup"><span data-stu-id="92f64-185">Int32</span></span>|<span data-ttu-id="92f64-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="92f64-186">The upload state.</span></span> <span data-ttu-id="92f64-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="92f64-188">publishingState</span></span>|[<span data-ttu-id="92f64-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="92f64-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="92f64-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="92f64-190">The publishing state for the app.</span></span> <span data-ttu-id="92f64-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="92f64-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="92f64-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="92f64-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="92f64-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="92f64-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="92f64-194">isAssigned</span></span>|<span data-ttu-id="92f64-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="92f64-195">Boolean</span></span>|<span data-ttu-id="92f64-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="92f64-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="92f64-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92f64-198">roleScopeTagIds</span></span>|<span data-ttu-id="92f64-199">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="92f64-199">String collection</span></span>|<span data-ttu-id="92f64-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="92f64-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="92f64-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="92f64-202">dependentAppCount</span></span>|<span data-ttu-id="92f64-203">Int32</span><span class="sxs-lookup"><span data-stu-id="92f64-203">Int32</span></span>|<span data-ttu-id="92f64-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="92f64-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="92f64-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92f64-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92f64-206">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="92f64-206">usedLicenseCount</span></span>|<span data-ttu-id="92f64-207">Int32</span><span class="sxs-lookup"><span data-stu-id="92f64-207">Int32</span></span>|<span data-ttu-id="92f64-208">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="92f64-208">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="92f64-209">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="92f64-209">totalLicenseCount</span></span>|<span data-ttu-id="92f64-210">Int32</span><span class="sxs-lookup"><span data-stu-id="92f64-210">Int32</span></span>|<span data-ttu-id="92f64-211">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="92f64-211">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="92f64-212">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="92f64-212">releaseDateTime</span></span>|<span data-ttu-id="92f64-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92f64-213">DateTimeOffset</span></span>|<span data-ttu-id="92f64-214">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="92f64-214">The VPP application release date and time.</span></span>|
|<span data-ttu-id="92f64-215">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="92f64-215">appStoreUrl</span></span>|<span data-ttu-id="92f64-216">String</span><span class="sxs-lookup"><span data-stu-id="92f64-216">String</span></span>|<span data-ttu-id="92f64-217">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="92f64-217">The store URL.</span></span>|
|<span data-ttu-id="92f64-218">licensingType</span><span class="sxs-lookup"><span data-stu-id="92f64-218">licensingType</span></span>|[<span data-ttu-id="92f64-219">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="92f64-219">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="92f64-220">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="92f64-220">The supported License Type.</span></span>|
|<span data-ttu-id="92f64-221">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="92f64-221">applicableDeviceType</span></span>|[<span data-ttu-id="92f64-222">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="92f64-222">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="92f64-223">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="92f64-223">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="92f64-224">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="92f64-224">vppTokenOrganizationName</span></span>|<span data-ttu-id="92f64-225">String</span><span class="sxs-lookup"><span data-stu-id="92f64-225">String</span></span>|<span data-ttu-id="92f64-226">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="92f64-226">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="92f64-227">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="92f64-227">vppTokenAccountType</span></span>|[<span data-ttu-id="92f64-228">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="92f64-228">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="92f64-229">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="92f64-229">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="92f64-230">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="92f64-230">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="92f64-231">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="92f64-231">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="92f64-232">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="92f64-232">vppTokenAppleId</span></span>|<span data-ttu-id="92f64-233">String</span><span class="sxs-lookup"><span data-stu-id="92f64-233">String</span></span>|<span data-ttu-id="92f64-234">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="92f64-234">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="92f64-235">bundleId</span><span class="sxs-lookup"><span data-stu-id="92f64-235">bundleId</span></span>|<span data-ttu-id="92f64-236">String</span><span class="sxs-lookup"><span data-stu-id="92f64-236">String</span></span>|<span data-ttu-id="92f64-237">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="92f64-237">The Identity Name.</span></span>|
|<span data-ttu-id="92f64-238">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="92f64-238">vppTokenId</span></span>|<span data-ttu-id="92f64-239">String</span><span class="sxs-lookup"><span data-stu-id="92f64-239">String</span></span>|<span data-ttu-id="92f64-240">Идентификатор токена VPP, связанного с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="92f64-240">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="92f64-241">ревокелиценсеактионресултс</span><span class="sxs-lookup"><span data-stu-id="92f64-241">revokeLicenseActionResults</span></span>|<span data-ttu-id="92f64-242">Коллекция [иосвппаппревокелиценсесактионресулт](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="92f64-242">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="92f64-243">Результаты отзыва действий лицензии в этом приложении.</span><span class="sxs-lookup"><span data-stu-id="92f64-243">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="92f64-244">Ответ</span><span class="sxs-lookup"><span data-stu-id="92f64-244">Response</span></span>
<span data-ttu-id="92f64-245">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="92f64-245">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92f64-246">Пример</span><span class="sxs-lookup"><span data-stu-id="92f64-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="92f64-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="92f64-247">Request</span></span>
<span data-ttu-id="92f64-248">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92f64-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1999

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="92f64-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="92f64-249">Response</span></span>
<span data-ttu-id="92f64-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92f64-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2171

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```



