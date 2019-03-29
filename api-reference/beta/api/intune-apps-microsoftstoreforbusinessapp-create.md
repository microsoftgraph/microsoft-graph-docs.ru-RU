---
title: Create microsoftStoreForBusinessApp
description: Создание объекта microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39a5ff6c11a30b7fea7d93875e344fddfa6febe3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978789"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="e4437-103">Create microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="e4437-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="e4437-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4437-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4437-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4437-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4437-106">Создание объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4437-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e4437-107">Prerequisites</span></span>
<span data-ttu-id="e4437-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4437-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4437-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4437-110">Permission type</span></span>|<span data-ttu-id="e4437-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4437-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4437-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4437-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4437-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4437-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e4437-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4437-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4437-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4437-115">Not supported.</span></span>|
|<span data-ttu-id="e4437-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4437-116">Application</span></span>|<span data-ttu-id="e4437-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4437-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4437-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4437-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e4437-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4437-119">Request headers</span></span>
|<span data-ttu-id="e4437-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4437-120">Header</span></span>|<span data-ttu-id="e4437-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e4437-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4437-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4437-122">Authorization</span></span>|<span data-ttu-id="e4437-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4437-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4437-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e4437-124">Accept</span></span>|<span data-ttu-id="e4437-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4437-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4437-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4437-126">Request body</span></span>
<span data-ttu-id="e4437-127">В тексте запроса добавьте представление объекта microsoftStoreForBusinessApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4437-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="e4437-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="e4437-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="e4437-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4437-129">Property</span></span>|<span data-ttu-id="e4437-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e4437-130">Type</span></span>|<span data-ttu-id="e4437-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e4437-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4437-132">id</span><span class="sxs-lookup"><span data-stu-id="e4437-132">id</span></span>|<span data-ttu-id="e4437-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e4437-133">String</span></span>|<span data-ttu-id="e4437-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e4437-134">Key of the entity.</span></span> <span data-ttu-id="e4437-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e4437-136">displayName</span></span>|<span data-ttu-id="e4437-137">String</span><span class="sxs-lookup"><span data-stu-id="e4437-137">String</span></span>|<span data-ttu-id="e4437-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e4437-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e4437-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-140">description</span><span class="sxs-lookup"><span data-stu-id="e4437-140">description</span></span>|<span data-ttu-id="e4437-141">String</span><span class="sxs-lookup"><span data-stu-id="e4437-141">String</span></span>|<span data-ttu-id="e4437-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e4437-142">The description of the app.</span></span> <span data-ttu-id="e4437-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e4437-144">publisher</span></span>|<span data-ttu-id="e4437-145">String</span><span class="sxs-lookup"><span data-stu-id="e4437-145">String</span></span>|<span data-ttu-id="e4437-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e4437-146">The publisher of the app.</span></span> <span data-ttu-id="e4437-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e4437-148">largeIcon</span></span>|[<span data-ttu-id="e4437-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e4437-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e4437-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e4437-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e4437-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4437-152">createdDateTime</span></span>|<span data-ttu-id="e4437-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4437-153">DateTimeOffset</span></span>|<span data-ttu-id="e4437-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e4437-154">The date and time the app was created.</span></span> <span data-ttu-id="e4437-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4437-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e4437-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4437-157">DateTimeOffset</span></span>|<span data-ttu-id="e4437-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e4437-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e4437-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e4437-160">isFeatured</span></span>|<span data-ttu-id="e4437-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4437-161">Boolean</span></span>|<span data-ttu-id="e4437-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e4437-163">privacyInformationUrl</span></span>|<span data-ttu-id="e4437-164">String</span><span class="sxs-lookup"><span data-stu-id="e4437-164">String</span></span>|<span data-ttu-id="e4437-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e4437-165">The privacy statement Url.</span></span> <span data-ttu-id="e4437-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e4437-167">informationUrl</span></span>|<span data-ttu-id="e4437-168">String</span><span class="sxs-lookup"><span data-stu-id="e4437-168">String</span></span>|<span data-ttu-id="e4437-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e4437-169">The more information Url.</span></span> <span data-ttu-id="e4437-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-171">owner</span><span class="sxs-lookup"><span data-stu-id="e4437-171">owner</span></span>|<span data-ttu-id="e4437-172">String</span><span class="sxs-lookup"><span data-stu-id="e4437-172">String</span></span>|<span data-ttu-id="e4437-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e4437-173">The owner of the app.</span></span> <span data-ttu-id="e4437-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-175">developer</span><span class="sxs-lookup"><span data-stu-id="e4437-175">developer</span></span>|<span data-ttu-id="e4437-176">String</span><span class="sxs-lookup"><span data-stu-id="e4437-176">String</span></span>|<span data-ttu-id="e4437-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e4437-177">The developer of the app.</span></span> <span data-ttu-id="e4437-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-179">notes</span><span class="sxs-lookup"><span data-stu-id="e4437-179">notes</span></span>|<span data-ttu-id="e4437-180">String</span><span class="sxs-lookup"><span data-stu-id="e4437-180">String</span></span>|<span data-ttu-id="e4437-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="e4437-181">Notes for the app.</span></span> <span data-ttu-id="e4437-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e4437-183">uploadState</span></span>|<span data-ttu-id="e4437-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e4437-184">Int32</span></span>|<span data-ttu-id="e4437-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="e4437-185">The upload state.</span></span> <span data-ttu-id="e4437-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e4437-187">publishingState</span></span>|[<span data-ttu-id="e4437-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="e4437-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e4437-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="e4437-189">The publishing state for the app.</span></span> <span data-ttu-id="e4437-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e4437-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e4437-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e4437-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e4437-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e4437-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e4437-193">isAssigned</span></span>|<span data-ttu-id="e4437-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4437-194">Boolean</span></span>|<span data-ttu-id="e4437-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="e4437-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e4437-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e4437-197">roleScopeTagIds</span></span>|<span data-ttu-id="e4437-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e4437-198">String collection</span></span>|<span data-ttu-id="e4437-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e4437-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e4437-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4437-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4437-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e4437-201">usedLicenseCount</span></span>|<span data-ttu-id="e4437-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e4437-202">Int32</span></span>|<span data-ttu-id="e4437-203">Количество используемых лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e4437-203">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="e4437-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e4437-204">totalLicenseCount</span></span>|<span data-ttu-id="e4437-205">Int32</span><span class="sxs-lookup"><span data-stu-id="e4437-205">Int32</span></span>|<span data-ttu-id="e4437-206">Общее количество лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e4437-206">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="e4437-207">productKey</span><span class="sxs-lookup"><span data-stu-id="e4437-207">productKey</span></span>|<span data-ttu-id="e4437-208">Строка</span><span class="sxs-lookup"><span data-stu-id="e4437-208">String</span></span>|<span data-ttu-id="e4437-209">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="e4437-209">The app product key</span></span>|
|<span data-ttu-id="e4437-210">licenseType</span><span class="sxs-lookup"><span data-stu-id="e4437-210">licenseType</span></span>|[<span data-ttu-id="e4437-211">Микрософтсторефорбусинесслиценсетипе</span><span class="sxs-lookup"><span data-stu-id="e4437-211">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="e4437-212">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="e4437-212">The app license type.</span></span> <span data-ttu-id="e4437-213">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="e4437-213">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="e4437-214">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="e4437-214">packageIdentityName</span></span>|<span data-ttu-id="e4437-215">String</span><span class="sxs-lookup"><span data-stu-id="e4437-215">String</span></span>|<span data-ttu-id="e4437-216">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="e4437-216">The app package identifier</span></span>|
|<span data-ttu-id="e4437-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="e4437-217">licensingType</span></span>|[<span data-ttu-id="e4437-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="e4437-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="e4437-219">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="e4437-219">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="e4437-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4437-220">Response</span></span>
<span data-ttu-id="e4437-221">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e4437-221">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4437-222">Пример</span><span class="sxs-lookup"><span data-stu-id="e4437-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4437-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4437-223">Request</span></span>
<span data-ttu-id="e4437-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4437-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1105

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

### <a name="response"></a><span data-ttu-id="e4437-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4437-225">Response</span></span>
<span data-ttu-id="e4437-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4437-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1277

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




