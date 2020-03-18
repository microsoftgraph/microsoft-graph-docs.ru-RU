---
title: Создание Андроидманажедсторевебапп
description: Создание нового объекта Андроидманажедсторевебапп.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bb71488437b40c050c77d72dd9e62320223b016b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762205"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="92751-103">Создание Андроидманажедсторевебапп</span><span class="sxs-lookup"><span data-stu-id="92751-103">Create androidManagedStoreWebApp</span></span>

> <span data-ttu-id="92751-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92751-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92751-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92751-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92751-106">Создание нового объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="92751-106">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92751-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="92751-107">Prerequisites</span></span>
<span data-ttu-id="92751-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92751-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92751-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92751-110">Permission type</span></span>|<span data-ttu-id="92751-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92751-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92751-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92751-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92751-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92751-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="92751-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92751-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92751-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92751-115">Not supported.</span></span>|
|<span data-ttu-id="92751-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="92751-116">Application</span></span>|<span data-ttu-id="92751-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92751-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92751-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92751-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="92751-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92751-119">Request headers</span></span>
|<span data-ttu-id="92751-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92751-120">Header</span></span>|<span data-ttu-id="92751-121">Значение</span><span class="sxs-lookup"><span data-stu-id="92751-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92751-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92751-122">Authorization</span></span>|<span data-ttu-id="92751-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92751-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92751-124">Accept</span><span class="sxs-lookup"><span data-stu-id="92751-124">Accept</span></span>|<span data-ttu-id="92751-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92751-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92751-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="92751-126">Request body</span></span>
<span data-ttu-id="92751-127">В тексте запроса добавьте представление объекта Андроидманажедсторевебапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92751-127">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="92751-128">В следующей таблице приведены свойства, необходимые при создании Андроидманажедсторевебапп.</span><span class="sxs-lookup"><span data-stu-id="92751-128">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="92751-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="92751-129">Property</span></span>|<span data-ttu-id="92751-130">Тип</span><span class="sxs-lookup"><span data-stu-id="92751-130">Type</span></span>|<span data-ttu-id="92751-131">Описание</span><span class="sxs-lookup"><span data-stu-id="92751-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92751-132">id</span><span class="sxs-lookup"><span data-stu-id="92751-132">id</span></span>|<span data-ttu-id="92751-133">Строка</span><span class="sxs-lookup"><span data-stu-id="92751-133">String</span></span>|<span data-ttu-id="92751-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="92751-134">Key of the entity.</span></span> <span data-ttu-id="92751-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-136">displayName</span><span class="sxs-lookup"><span data-stu-id="92751-136">displayName</span></span>|<span data-ttu-id="92751-137">Строка</span><span class="sxs-lookup"><span data-stu-id="92751-137">String</span></span>|<span data-ttu-id="92751-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="92751-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="92751-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-140">description</span><span class="sxs-lookup"><span data-stu-id="92751-140">description</span></span>|<span data-ttu-id="92751-141">Строка</span><span class="sxs-lookup"><span data-stu-id="92751-141">String</span></span>|<span data-ttu-id="92751-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="92751-142">The description of the app.</span></span> <span data-ttu-id="92751-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-144">publisher</span><span class="sxs-lookup"><span data-stu-id="92751-144">publisher</span></span>|<span data-ttu-id="92751-145">String</span><span class="sxs-lookup"><span data-stu-id="92751-145">String</span></span>|<span data-ttu-id="92751-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="92751-146">The publisher of the app.</span></span> <span data-ttu-id="92751-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="92751-148">largeIcon</span></span>|[<span data-ttu-id="92751-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="92751-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="92751-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="92751-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="92751-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92751-152">createdDateTime</span></span>|<span data-ttu-id="92751-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92751-153">DateTimeOffset</span></span>|<span data-ttu-id="92751-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="92751-154">The date and time the app was created.</span></span> <span data-ttu-id="92751-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92751-156">lastModifiedDateTime</span></span>|<span data-ttu-id="92751-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92751-157">DateTimeOffset</span></span>|<span data-ttu-id="92751-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="92751-158">The date and time the app was last modified.</span></span> <span data-ttu-id="92751-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="92751-160">isFeatured</span></span>|<span data-ttu-id="92751-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="92751-161">Boolean</span></span>|<span data-ttu-id="92751-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="92751-163">privacyInformationUrl</span></span>|<span data-ttu-id="92751-164">String</span><span class="sxs-lookup"><span data-stu-id="92751-164">String</span></span>|<span data-ttu-id="92751-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="92751-165">The privacy statement Url.</span></span> <span data-ttu-id="92751-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="92751-167">informationUrl</span></span>|<span data-ttu-id="92751-168">String</span><span class="sxs-lookup"><span data-stu-id="92751-168">String</span></span>|<span data-ttu-id="92751-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="92751-169">The more information Url.</span></span> <span data-ttu-id="92751-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-171">owner</span><span class="sxs-lookup"><span data-stu-id="92751-171">owner</span></span>|<span data-ttu-id="92751-172">String</span><span class="sxs-lookup"><span data-stu-id="92751-172">String</span></span>|<span data-ttu-id="92751-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="92751-173">The owner of the app.</span></span> <span data-ttu-id="92751-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-175">developer</span><span class="sxs-lookup"><span data-stu-id="92751-175">developer</span></span>|<span data-ttu-id="92751-176">String</span><span class="sxs-lookup"><span data-stu-id="92751-176">String</span></span>|<span data-ttu-id="92751-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="92751-177">The developer of the app.</span></span> <span data-ttu-id="92751-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-179">notes</span><span class="sxs-lookup"><span data-stu-id="92751-179">notes</span></span>|<span data-ttu-id="92751-180">String</span><span class="sxs-lookup"><span data-stu-id="92751-180">String</span></span>|<span data-ttu-id="92751-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="92751-181">Notes for the app.</span></span> <span data-ttu-id="92751-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="92751-183">uploadState</span></span>|<span data-ttu-id="92751-184">Int32</span><span class="sxs-lookup"><span data-stu-id="92751-184">Int32</span></span>|<span data-ttu-id="92751-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="92751-185">The upload state.</span></span> <span data-ttu-id="92751-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="92751-187">publishingState</span></span>|[<span data-ttu-id="92751-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="92751-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="92751-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="92751-189">The publishing state for the app.</span></span> <span data-ttu-id="92751-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="92751-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="92751-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="92751-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="92751-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="92751-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="92751-193">isAssigned</span></span>|<span data-ttu-id="92751-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="92751-194">Boolean</span></span>|<span data-ttu-id="92751-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="92751-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="92751-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92751-197">roleScopeTagIds</span></span>|<span data-ttu-id="92751-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="92751-198">String collection</span></span>|<span data-ttu-id="92751-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="92751-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="92751-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="92751-201">dependentAppCount</span></span>|<span data-ttu-id="92751-202">Int32</span><span class="sxs-lookup"><span data-stu-id="92751-202">Int32</span></span>|<span data-ttu-id="92751-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="92751-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="92751-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="92751-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="92751-205">packageId</span><span class="sxs-lookup"><span data-stu-id="92751-205">packageId</span></span>|<span data-ttu-id="92751-206">String</span><span class="sxs-lookup"><span data-stu-id="92751-206">String</span></span>|<span data-ttu-id="92751-207">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="92751-207">The package identifier.</span></span> <span data-ttu-id="92751-208">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="92751-208">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="92751-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="92751-209">appIdentifier</span></span>|<span data-ttu-id="92751-210">String</span><span class="sxs-lookup"><span data-stu-id="92751-210">String</span></span>|<span data-ttu-id="92751-211">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="92751-211">The Identity Name.</span></span> <span data-ttu-id="92751-212">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="92751-212">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="92751-213">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="92751-213">usedLicenseCount</span></span>|<span data-ttu-id="92751-214">Int32</span><span class="sxs-lookup"><span data-stu-id="92751-214">Int32</span></span>|<span data-ttu-id="92751-215">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="92751-215">The number of VPP licenses in use.</span></span> <span data-ttu-id="92751-216">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="92751-216">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="92751-217">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="92751-217">totalLicenseCount</span></span>|<span data-ttu-id="92751-218">Int32</span><span class="sxs-lookup"><span data-stu-id="92751-218">Int32</span></span>|<span data-ttu-id="92751-219">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="92751-219">The total number of VPP licenses.</span></span> <span data-ttu-id="92751-220">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="92751-220">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="92751-221">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="92751-221">appStoreUrl</span></span>|<span data-ttu-id="92751-222">String</span><span class="sxs-lookup"><span data-stu-id="92751-222">String</span></span>|<span data-ttu-id="92751-223">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="92751-223">The Play for Work Store app URL.</span></span> <span data-ttu-id="92751-224">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="92751-224">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="92751-225">Частный</span><span class="sxs-lookup"><span data-stu-id="92751-225">isPrivate</span></span>|<span data-ttu-id="92751-226">Логический</span><span class="sxs-lookup"><span data-stu-id="92751-226">Boolean</span></span>|<span data-ttu-id="92751-227">Указывает, доступно ли приложение только для указанных пользователей предприятия.</span><span class="sxs-lookup"><span data-stu-id="92751-227">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="92751-228">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="92751-228">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="92751-229">иссистемапп</span><span class="sxs-lookup"><span data-stu-id="92751-229">isSystemApp</span></span>|<span data-ttu-id="92751-230">Логический</span><span class="sxs-lookup"><span data-stu-id="92751-230">Boolean</span></span>|<span data-ttu-id="92751-231">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="92751-231">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="92751-232">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="92751-232">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="92751-233">суппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="92751-233">supportsOemConfig</span></span>|<span data-ttu-id="92751-234">Логический</span><span class="sxs-lookup"><span data-stu-id="92751-234">Boolean</span></span>|<span data-ttu-id="92751-235">Поддерживает ли это приложение политику Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="92751-235">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="92751-236">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="92751-236">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="92751-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="92751-237">Response</span></span>
<span data-ttu-id="92751-238">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92751-238">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92751-239">Пример</span><span class="sxs-lookup"><span data-stu-id="92751-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="92751-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="92751-240">Request</span></span>
<span data-ttu-id="92751-241">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92751-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 987

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="92751-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="92751-242">Response</span></span>
<span data-ttu-id="92751-p127">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92751-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1159

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
  "id": "e54aecbd-ecbd-e54a-bdec-4ae5bdec4ae5",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "supportsOemConfig": true
}
```




