---
title: Создание Андроидманажедстореапп
description: Создание нового объекта Андроидманажедстореапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0cf9cee955c9e8c202adf7d2cd014a6162e23abb
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791220"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="75ff3-103">Создание Андроидманажедстореапп</span><span class="sxs-lookup"><span data-stu-id="75ff3-103">Create androidManagedStoreApp</span></span>

<span data-ttu-id="75ff3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75ff3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75ff3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75ff3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75ff3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75ff3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75ff3-107">Создание нового объекта [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="75ff3-107">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75ff3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="75ff3-108">Prerequisites</span></span>
<span data-ttu-id="75ff3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75ff3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75ff3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75ff3-111">Permission type</span></span>|<span data-ttu-id="75ff3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75ff3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75ff3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75ff3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75ff3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75ff3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="75ff3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75ff3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75ff3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75ff3-116">Not supported.</span></span>|
|<span data-ttu-id="75ff3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="75ff3-117">Application</span></span>|<span data-ttu-id="75ff3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75ff3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75ff3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75ff3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="75ff3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="75ff3-120">Request headers</span></span>
|<span data-ttu-id="75ff3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75ff3-121">Header</span></span>|<span data-ttu-id="75ff3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="75ff3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75ff3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75ff3-123">Authorization</span></span>|<span data-ttu-id="75ff3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75ff3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75ff3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="75ff3-125">Accept</span></span>|<span data-ttu-id="75ff3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75ff3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75ff3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75ff3-127">Request body</span></span>
<span data-ttu-id="75ff3-128">В тексте запроса добавьте представление объекта Андроидманажедстореапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75ff3-128">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="75ff3-129">В следующей таблице приведены свойства, необходимые при создании Андроидманажедстореапп.</span><span class="sxs-lookup"><span data-stu-id="75ff3-129">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="75ff3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="75ff3-130">Property</span></span>|<span data-ttu-id="75ff3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="75ff3-131">Type</span></span>|<span data-ttu-id="75ff3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="75ff3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75ff3-133">id</span><span class="sxs-lookup"><span data-stu-id="75ff3-133">id</span></span>|<span data-ttu-id="75ff3-134">String</span><span class="sxs-lookup"><span data-stu-id="75ff3-134">String</span></span>|<span data-ttu-id="75ff3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="75ff3-135">Key of the entity.</span></span> <span data-ttu-id="75ff3-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="75ff3-137">displayName</span></span>|<span data-ttu-id="75ff3-138">String</span><span class="sxs-lookup"><span data-stu-id="75ff3-138">String</span></span>|<span data-ttu-id="75ff3-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="75ff3-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="75ff3-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-141">description</span><span class="sxs-lookup"><span data-stu-id="75ff3-141">description</span></span>|<span data-ttu-id="75ff3-142">String</span><span class="sxs-lookup"><span data-stu-id="75ff3-142">String</span></span>|<span data-ttu-id="75ff3-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="75ff3-143">The description of the app.</span></span> <span data-ttu-id="75ff3-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-145">publisher</span><span class="sxs-lookup"><span data-stu-id="75ff3-145">publisher</span></span>|<span data-ttu-id="75ff3-146">String</span><span class="sxs-lookup"><span data-stu-id="75ff3-146">String</span></span>|<span data-ttu-id="75ff3-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="75ff3-147">The publisher of the app.</span></span> <span data-ttu-id="75ff3-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="75ff3-149">largeIcon</span></span>|[<span data-ttu-id="75ff3-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="75ff3-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="75ff3-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="75ff3-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="75ff3-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75ff3-153">createdDateTime</span></span>|<span data-ttu-id="75ff3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75ff3-154">DateTimeOffset</span></span>|<span data-ttu-id="75ff3-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="75ff3-155">The date and time the app was created.</span></span> <span data-ttu-id="75ff3-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75ff3-157">lastModifiedDateTime</span></span>|<span data-ttu-id="75ff3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75ff3-158">DateTimeOffset</span></span>|<span data-ttu-id="75ff3-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="75ff3-159">The date and time the app was last modified.</span></span> <span data-ttu-id="75ff3-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="75ff3-161">isFeatured</span></span>|<span data-ttu-id="75ff3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="75ff3-162">Boolean</span></span>|<span data-ttu-id="75ff3-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="75ff3-164">privacyInformationUrl</span></span>|<span data-ttu-id="75ff3-165">String</span><span class="sxs-lookup"><span data-stu-id="75ff3-165">String</span></span>|<span data-ttu-id="75ff3-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="75ff3-166">The privacy statement Url.</span></span> <span data-ttu-id="75ff3-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="75ff3-168">informationUrl</span></span>|<span data-ttu-id="75ff3-169">String</span><span class="sxs-lookup"><span data-stu-id="75ff3-169">String</span></span>|<span data-ttu-id="75ff3-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="75ff3-170">The more information Url.</span></span> <span data-ttu-id="75ff3-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-172">owner</span><span class="sxs-lookup"><span data-stu-id="75ff3-172">owner</span></span>|<span data-ttu-id="75ff3-173">String</span><span class="sxs-lookup"><span data-stu-id="75ff3-173">String</span></span>|<span data-ttu-id="75ff3-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="75ff3-174">The owner of the app.</span></span> <span data-ttu-id="75ff3-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-176">developer</span><span class="sxs-lookup"><span data-stu-id="75ff3-176">developer</span></span>|<span data-ttu-id="75ff3-177">String</span><span class="sxs-lookup"><span data-stu-id="75ff3-177">String</span></span>|<span data-ttu-id="75ff3-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="75ff3-178">The developer of the app.</span></span> <span data-ttu-id="75ff3-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-180">notes</span><span class="sxs-lookup"><span data-stu-id="75ff3-180">notes</span></span>|<span data-ttu-id="75ff3-181">String</span><span class="sxs-lookup"><span data-stu-id="75ff3-181">String</span></span>|<span data-ttu-id="75ff3-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="75ff3-182">Notes for the app.</span></span> <span data-ttu-id="75ff3-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="75ff3-184">uploadState</span></span>|<span data-ttu-id="75ff3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="75ff3-185">Int32</span></span>|<span data-ttu-id="75ff3-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="75ff3-186">The upload state.</span></span> <span data-ttu-id="75ff3-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="75ff3-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="75ff3-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="75ff3-189">publishingState</span></span>|[<span data-ttu-id="75ff3-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="75ff3-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="75ff3-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="75ff3-191">The publishing state for the app.</span></span> <span data-ttu-id="75ff3-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="75ff3-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="75ff3-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="75ff3-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="75ff3-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="75ff3-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="75ff3-195">isAssigned</span></span>|<span data-ttu-id="75ff3-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="75ff3-196">Boolean</span></span>|<span data-ttu-id="75ff3-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="75ff3-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="75ff3-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="75ff3-199">roleScopeTagIds</span></span>|<span data-ttu-id="75ff3-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="75ff3-200">String collection</span></span>|<span data-ttu-id="75ff3-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="75ff3-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="75ff3-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="75ff3-203">dependentAppCount</span></span>|<span data-ttu-id="75ff3-204">Int32</span><span class="sxs-lookup"><span data-stu-id="75ff3-204">Int32</span></span>|<span data-ttu-id="75ff3-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="75ff3-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="75ff3-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75ff3-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75ff3-207">packageId</span><span class="sxs-lookup"><span data-stu-id="75ff3-207">packageId</span></span>|<span data-ttu-id="75ff3-208">String</span><span class="sxs-lookup"><span data-stu-id="75ff3-208">String</span></span>|<span data-ttu-id="75ff3-209">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="75ff3-209">The package identifier.</span></span>|
|<span data-ttu-id="75ff3-210">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="75ff3-210">appIdentifier</span></span>|<span data-ttu-id="75ff3-211">String</span><span class="sxs-lookup"><span data-stu-id="75ff3-211">String</span></span>|<span data-ttu-id="75ff3-212">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="75ff3-212">The Identity Name.</span></span>|
|<span data-ttu-id="75ff3-213">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="75ff3-213">usedLicenseCount</span></span>|<span data-ttu-id="75ff3-214">Int32</span><span class="sxs-lookup"><span data-stu-id="75ff3-214">Int32</span></span>|<span data-ttu-id="75ff3-215">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="75ff3-215">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="75ff3-216">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="75ff3-216">totalLicenseCount</span></span>|<span data-ttu-id="75ff3-217">Int32</span><span class="sxs-lookup"><span data-stu-id="75ff3-217">Int32</span></span>|<span data-ttu-id="75ff3-218">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="75ff3-218">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="75ff3-219">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="75ff3-219">appStoreUrl</span></span>|<span data-ttu-id="75ff3-220">String</span><span class="sxs-lookup"><span data-stu-id="75ff3-220">String</span></span>|<span data-ttu-id="75ff3-221">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="75ff3-221">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="75ff3-222">Частный</span><span class="sxs-lookup"><span data-stu-id="75ff3-222">isPrivate</span></span>|<span data-ttu-id="75ff3-223">Логический</span><span class="sxs-lookup"><span data-stu-id="75ff3-223">Boolean</span></span>|<span data-ttu-id="75ff3-224">Указывает, доступно ли приложение только для указанных пользователей предприятия.</span><span class="sxs-lookup"><span data-stu-id="75ff3-224">Indicates whether the app is only available to a given enterprise's users.</span></span>|
|<span data-ttu-id="75ff3-225">иссистемапп</span><span class="sxs-lookup"><span data-stu-id="75ff3-225">isSystemApp</span></span>|<span data-ttu-id="75ff3-226">Логический</span><span class="sxs-lookup"><span data-stu-id="75ff3-226">Boolean</span></span>|<span data-ttu-id="75ff3-227">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="75ff3-227">Indicates whether the app is a preinstalled system app.</span></span>|
|<span data-ttu-id="75ff3-228">апптраккс</span><span class="sxs-lookup"><span data-stu-id="75ff3-228">appTracks</span></span>|<span data-ttu-id="75ff3-229">Коллекция [андроидманажедстореапптракк](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="75ff3-229">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="75ff3-230">Дорожки, которые видимы для этого предприятия.</span><span class="sxs-lookup"><span data-stu-id="75ff3-230">The tracks that are visible to this enterprise.</span></span>|
|<span data-ttu-id="75ff3-231">суппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="75ff3-231">supportsOemConfig</span></span>|<span data-ttu-id="75ff3-232">Логический</span><span class="sxs-lookup"><span data-stu-id="75ff3-232">Boolean</span></span>|<span data-ttu-id="75ff3-233">Поддерживает ли это приложение политику Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="75ff3-233">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="75ff3-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="75ff3-234">Response</span></span>
<span data-ttu-id="75ff3-235">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="75ff3-235">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75ff3-236">Пример</span><span class="sxs-lookup"><span data-stu-id="75ff3-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="75ff3-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="75ff3-237">Request</span></span>
<span data-ttu-id="75ff3-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75ff3-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1168

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="75ff3-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="75ff3-239">Response</span></span>
<span data-ttu-id="75ff3-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75ff3-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1340

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```



