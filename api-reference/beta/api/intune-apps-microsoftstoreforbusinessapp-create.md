---
title: Create microsoftStoreForBusinessApp
description: Создание объекта microsoftStoreForBusinessApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 15592dbce6bb1fc2665dbfcbc5fc9075cc1420c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961247"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="1bf58-103">Create microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="1bf58-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="1bf58-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bf58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bf58-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bf58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bf58-106">Создание объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bf58-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1bf58-107">Prerequisites</span></span>
<span data-ttu-id="1bf58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bf58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bf58-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bf58-110">Permission type</span></span>|<span data-ttu-id="1bf58-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bf58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bf58-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bf58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1bf58-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bf58-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1bf58-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bf58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bf58-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bf58-115">Not supported.</span></span>|
|<span data-ttu-id="1bf58-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bf58-116">Application</span></span>|<span data-ttu-id="1bf58-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bf58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bf58-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bf58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1bf58-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bf58-119">Request headers</span></span>
|<span data-ttu-id="1bf58-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1bf58-120">Header</span></span>|<span data-ttu-id="1bf58-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1bf58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bf58-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1bf58-122">Authorization</span></span>|<span data-ttu-id="1bf58-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bf58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bf58-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1bf58-124">Accept</span></span>|<span data-ttu-id="1bf58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1bf58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bf58-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1bf58-126">Request body</span></span>
<span data-ttu-id="1bf58-127">В тексте запроса добавьте представление объекта microsoftStoreForBusinessApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bf58-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="1bf58-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="1bf58-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="1bf58-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bf58-129">Property</span></span>|<span data-ttu-id="1bf58-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1bf58-130">Type</span></span>|<span data-ttu-id="1bf58-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1bf58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bf58-132">id</span><span class="sxs-lookup"><span data-stu-id="1bf58-132">id</span></span>|<span data-ttu-id="1bf58-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1bf58-133">String</span></span>|<span data-ttu-id="1bf58-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1bf58-134">Key of the entity.</span></span> <span data-ttu-id="1bf58-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1bf58-136">displayName</span></span>|<span data-ttu-id="1bf58-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1bf58-137">String</span></span>|<span data-ttu-id="1bf58-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="1bf58-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1bf58-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-140">description</span><span class="sxs-lookup"><span data-stu-id="1bf58-140">description</span></span>|<span data-ttu-id="1bf58-141">String</span><span class="sxs-lookup"><span data-stu-id="1bf58-141">String</span></span>|<span data-ttu-id="1bf58-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf58-142">The description of the app.</span></span> <span data-ttu-id="1bf58-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-144">publisher</span><span class="sxs-lookup"><span data-stu-id="1bf58-144">publisher</span></span>|<span data-ttu-id="1bf58-145">String</span><span class="sxs-lookup"><span data-stu-id="1bf58-145">String</span></span>|<span data-ttu-id="1bf58-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf58-146">The publisher of the app.</span></span> <span data-ttu-id="1bf58-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1bf58-148">largeIcon</span></span>|[<span data-ttu-id="1bf58-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1bf58-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1bf58-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="1bf58-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1bf58-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1bf58-152">createdDateTime</span></span>|<span data-ttu-id="1bf58-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bf58-153">DateTimeOffset</span></span>|<span data-ttu-id="1bf58-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf58-154">The date and time the app was created.</span></span> <span data-ttu-id="1bf58-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1bf58-156">lastModifiedDateTime</span></span>|<span data-ttu-id="1bf58-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bf58-157">DateTimeOffset</span></span>|<span data-ttu-id="1bf58-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf58-158">The date and time the app was last modified.</span></span> <span data-ttu-id="1bf58-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1bf58-160">isFeatured</span></span>|<span data-ttu-id="1bf58-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bf58-161">Boolean</span></span>|<span data-ttu-id="1bf58-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1bf58-163">privacyInformationUrl</span></span>|<span data-ttu-id="1bf58-164">String</span><span class="sxs-lookup"><span data-stu-id="1bf58-164">String</span></span>|<span data-ttu-id="1bf58-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="1bf58-165">The privacy statement Url.</span></span> <span data-ttu-id="1bf58-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1bf58-167">informationUrl</span></span>|<span data-ttu-id="1bf58-168">String</span><span class="sxs-lookup"><span data-stu-id="1bf58-168">String</span></span>|<span data-ttu-id="1bf58-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="1bf58-169">The more information Url.</span></span> <span data-ttu-id="1bf58-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-171">owner</span><span class="sxs-lookup"><span data-stu-id="1bf58-171">owner</span></span>|<span data-ttu-id="1bf58-172">String</span><span class="sxs-lookup"><span data-stu-id="1bf58-172">String</span></span>|<span data-ttu-id="1bf58-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf58-173">The owner of the app.</span></span> <span data-ttu-id="1bf58-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-175">developer</span><span class="sxs-lookup"><span data-stu-id="1bf58-175">developer</span></span>|<span data-ttu-id="1bf58-176">String</span><span class="sxs-lookup"><span data-stu-id="1bf58-176">String</span></span>|<span data-ttu-id="1bf58-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf58-177">The developer of the app.</span></span> <span data-ttu-id="1bf58-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-179">notes</span><span class="sxs-lookup"><span data-stu-id="1bf58-179">notes</span></span>|<span data-ttu-id="1bf58-180">String</span><span class="sxs-lookup"><span data-stu-id="1bf58-180">String</span></span>|<span data-ttu-id="1bf58-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf58-181">Notes for the app.</span></span> <span data-ttu-id="1bf58-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="1bf58-183">uploadState</span></span>|<span data-ttu-id="1bf58-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1bf58-184">Int32</span></span>|<span data-ttu-id="1bf58-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="1bf58-185">The upload state.</span></span> <span data-ttu-id="1bf58-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="1bf58-187">publishingState</span></span>|[<span data-ttu-id="1bf58-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="1bf58-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1bf58-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf58-189">The publishing state for the app.</span></span> <span data-ttu-id="1bf58-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="1bf58-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1bf58-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1bf58-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1bf58-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1bf58-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1bf58-193">isAssigned</span></span>|<span data-ttu-id="1bf58-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bf58-194">Boolean</span></span>|<span data-ttu-id="1bf58-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="1bf58-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1bf58-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1bf58-197">roleScopeTagIds</span></span>|<span data-ttu-id="1bf58-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1bf58-198">String collection</span></span>|<span data-ttu-id="1bf58-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf58-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1bf58-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="1bf58-201">dependentAppCount</span></span>|<span data-ttu-id="1bf58-202">Int32</span><span class="sxs-lookup"><span data-stu-id="1bf58-202">Int32</span></span>|<span data-ttu-id="1bf58-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf58-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="1bf58-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bf58-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1bf58-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1bf58-205">usedLicenseCount</span></span>|<span data-ttu-id="1bf58-206">Int32</span><span class="sxs-lookup"><span data-stu-id="1bf58-206">Int32</span></span>|<span data-ttu-id="1bf58-207">Количество используемых лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1bf58-207">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="1bf58-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1bf58-208">totalLicenseCount</span></span>|<span data-ttu-id="1bf58-209">Int32</span><span class="sxs-lookup"><span data-stu-id="1bf58-209">Int32</span></span>|<span data-ttu-id="1bf58-210">Общее количество лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1bf58-210">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="1bf58-211">productKey</span><span class="sxs-lookup"><span data-stu-id="1bf58-211">productKey</span></span>|<span data-ttu-id="1bf58-212">Строка</span><span class="sxs-lookup"><span data-stu-id="1bf58-212">String</span></span>|<span data-ttu-id="1bf58-213">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf58-213">The app product key</span></span>|
|<span data-ttu-id="1bf58-214">licenseType</span><span class="sxs-lookup"><span data-stu-id="1bf58-214">licenseType</span></span>|[<span data-ttu-id="1bf58-215">Микрософтсторефорбусинесслиценсетипе</span><span class="sxs-lookup"><span data-stu-id="1bf58-215">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="1bf58-216">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="1bf58-216">The app license type.</span></span> <span data-ttu-id="1bf58-217">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="1bf58-217">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="1bf58-218">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="1bf58-218">packageIdentityName</span></span>|<span data-ttu-id="1bf58-219">String</span><span class="sxs-lookup"><span data-stu-id="1bf58-219">String</span></span>|<span data-ttu-id="1bf58-220">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="1bf58-220">The app package identifier</span></span>|
|<span data-ttu-id="1bf58-221">licensingType</span><span class="sxs-lookup"><span data-stu-id="1bf58-221">licensingType</span></span>|[<span data-ttu-id="1bf58-222">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="1bf58-222">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="1bf58-223">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="1bf58-223">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="1bf58-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="1bf58-224">Response</span></span>
<span data-ttu-id="1bf58-225">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1bf58-225">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bf58-226">Пример</span><span class="sxs-lookup"><span data-stu-id="1bf58-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bf58-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bf58-227">Request</span></span>
<span data-ttu-id="1bf58-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bf58-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1132

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```

### <a name="response"></a><span data-ttu-id="1bf58-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bf58-229">Response</span></span>
<span data-ttu-id="1bf58-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bf58-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1304

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```





