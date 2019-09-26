---
title: Обновление Андроидфорворкапп
description: Обновление свойств объекта Андроидфорворкапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 858210d808d42efa11db42834f655a48ba6f1f0d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37178161"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="4e804-103">Обновление Андроидфорворкапп</span><span class="sxs-lookup"><span data-stu-id="4e804-103">Update androidForWorkApp</span></span>

> <span data-ttu-id="4e804-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e804-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e804-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e804-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e804-106">Обновление свойств объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="4e804-106">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e804-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4e804-107">Prerequisites</span></span>
<span data-ttu-id="4e804-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e804-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e804-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e804-110">Permission type</span></span>|<span data-ttu-id="4e804-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e804-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e804-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e804-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e804-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e804-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4e804-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e804-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e804-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e804-115">Not supported.</span></span>|
|<span data-ttu-id="4e804-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e804-116">Application</span></span>|<span data-ttu-id="4e804-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e804-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e804-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e804-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4e804-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e804-119">Request headers</span></span>
|<span data-ttu-id="4e804-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e804-120">Header</span></span>|<span data-ttu-id="4e804-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4e804-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e804-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e804-122">Authorization</span></span>|<span data-ttu-id="4e804-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e804-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e804-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4e804-124">Accept</span></span>|<span data-ttu-id="4e804-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e804-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e804-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4e804-126">Request body</span></span>
<span data-ttu-id="4e804-127">В тексте запроса добавьте представление объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e804-127">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="4e804-128">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-128">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="4e804-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e804-129">Property</span></span>|<span data-ttu-id="4e804-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4e804-130">Type</span></span>|<span data-ttu-id="4e804-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4e804-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e804-132">id</span><span class="sxs-lookup"><span data-stu-id="4e804-132">id</span></span>|<span data-ttu-id="4e804-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4e804-133">String</span></span>|<span data-ttu-id="4e804-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4e804-134">Key of the entity.</span></span> <span data-ttu-id="4e804-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4e804-136">displayName</span></span>|<span data-ttu-id="4e804-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4e804-137">String</span></span>|<span data-ttu-id="4e804-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="4e804-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4e804-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-140">description</span><span class="sxs-lookup"><span data-stu-id="4e804-140">description</span></span>|<span data-ttu-id="4e804-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4e804-141">String</span></span>|<span data-ttu-id="4e804-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="4e804-142">The description of the app.</span></span> <span data-ttu-id="4e804-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4e804-144">publisher</span></span>|<span data-ttu-id="4e804-145">String.</span><span class="sxs-lookup"><span data-stu-id="4e804-145">String</span></span>|<span data-ttu-id="4e804-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="4e804-146">The publisher of the app.</span></span> <span data-ttu-id="4e804-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4e804-148">largeIcon</span></span>|[<span data-ttu-id="4e804-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4e804-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4e804-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="4e804-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4e804-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e804-152">createdDateTime</span></span>|<span data-ttu-id="4e804-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e804-153">DateTimeOffset</span></span>|<span data-ttu-id="4e804-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="4e804-154">The date and time the app was created.</span></span> <span data-ttu-id="4e804-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e804-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4e804-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e804-157">DateTimeOffset</span></span>|<span data-ttu-id="4e804-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="4e804-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4e804-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4e804-160">isFeatured</span></span>|<span data-ttu-id="4e804-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e804-161">Boolean</span></span>|<span data-ttu-id="4e804-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4e804-163">privacyInformationUrl</span></span>|<span data-ttu-id="4e804-164">String.</span><span class="sxs-lookup"><span data-stu-id="4e804-164">String</span></span>|<span data-ttu-id="4e804-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4e804-165">The privacy statement Url.</span></span> <span data-ttu-id="4e804-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4e804-167">informationUrl</span></span>|<span data-ttu-id="4e804-168">String.</span><span class="sxs-lookup"><span data-stu-id="4e804-168">String</span></span>|<span data-ttu-id="4e804-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="4e804-169">The more information Url.</span></span> <span data-ttu-id="4e804-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-171">owner</span><span class="sxs-lookup"><span data-stu-id="4e804-171">owner</span></span>|<span data-ttu-id="4e804-172">String</span><span class="sxs-lookup"><span data-stu-id="4e804-172">String</span></span>|<span data-ttu-id="4e804-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="4e804-173">The owner of the app.</span></span> <span data-ttu-id="4e804-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-175">developer</span><span class="sxs-lookup"><span data-stu-id="4e804-175">developer</span></span>|<span data-ttu-id="4e804-176">String.</span><span class="sxs-lookup"><span data-stu-id="4e804-176">String</span></span>|<span data-ttu-id="4e804-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="4e804-177">The developer of the app.</span></span> <span data-ttu-id="4e804-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-179">notes</span><span class="sxs-lookup"><span data-stu-id="4e804-179">notes</span></span>|<span data-ttu-id="4e804-180">String.</span><span class="sxs-lookup"><span data-stu-id="4e804-180">String</span></span>|<span data-ttu-id="4e804-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="4e804-181">Notes for the app.</span></span> <span data-ttu-id="4e804-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4e804-183">uploadState</span></span>|<span data-ttu-id="4e804-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4e804-184">Int32</span></span>|<span data-ttu-id="4e804-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="4e804-185">The upload state.</span></span> <span data-ttu-id="4e804-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4e804-187">publishingState</span></span>|[<span data-ttu-id="4e804-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="4e804-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4e804-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="4e804-189">The publishing state for the app.</span></span> <span data-ttu-id="4e804-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="4e804-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4e804-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4e804-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4e804-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4e804-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4e804-193">isAssigned</span></span>|<span data-ttu-id="4e804-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e804-194">Boolean</span></span>|<span data-ttu-id="4e804-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="4e804-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4e804-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4e804-197">roleScopeTagIds</span></span>|<span data-ttu-id="4e804-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4e804-198">String collection</span></span>|<span data-ttu-id="4e804-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="4e804-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4e804-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="4e804-201">dependentAppCount</span></span>|<span data-ttu-id="4e804-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4e804-202">Int32</span></span>|<span data-ttu-id="4e804-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="4e804-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4e804-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e804-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4e804-205">packageId</span><span class="sxs-lookup"><span data-stu-id="4e804-205">packageId</span></span>|<span data-ttu-id="4e804-206">String.</span><span class="sxs-lookup"><span data-stu-id="4e804-206">String</span></span>|<span data-ttu-id="4e804-207">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="4e804-207">The package identifier.</span></span>|
|<span data-ttu-id="4e804-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="4e804-208">appIdentifier</span></span>|<span data-ttu-id="4e804-209">String</span><span class="sxs-lookup"><span data-stu-id="4e804-209">String</span></span>|<span data-ttu-id="4e804-210">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4e804-210">The Identity Name.</span></span>|
|<span data-ttu-id="4e804-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4e804-211">usedLicenseCount</span></span>|<span data-ttu-id="4e804-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4e804-212">Int32</span></span>|<span data-ttu-id="4e804-213">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="4e804-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="4e804-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4e804-214">totalLicenseCount</span></span>|<span data-ttu-id="4e804-215">Int32</span><span class="sxs-lookup"><span data-stu-id="4e804-215">Int32</span></span>|<span data-ttu-id="4e804-216">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="4e804-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="4e804-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4e804-217">appStoreUrl</span></span>|<span data-ttu-id="4e804-218">String</span><span class="sxs-lookup"><span data-stu-id="4e804-218">String</span></span>|<span data-ttu-id="4e804-219">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="4e804-219">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="4e804-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e804-220">Response</span></span>
<span data-ttu-id="4e804-221">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e804-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e804-222">Пример</span><span class="sxs-lookup"><span data-stu-id="4e804-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e804-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e804-223">Request</span></span>
<span data-ttu-id="4e804-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e804-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4e804-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e804-225">Response</span></span>
<span data-ttu-id="4e804-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e804-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




