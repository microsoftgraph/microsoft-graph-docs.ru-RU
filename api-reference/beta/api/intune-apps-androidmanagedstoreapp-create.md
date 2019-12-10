---
title: Создание Андроидманажедстореапп
description: Создание нового объекта Андроидманажедстореапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5d1cfa1d0c8abb1cdae737539eaa827afc25504
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39926679"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="4483c-103">Создание Андроидманажедстореапп</span><span class="sxs-lookup"><span data-stu-id="4483c-103">Create androidManagedStoreApp</span></span>

> <span data-ttu-id="4483c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4483c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4483c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4483c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4483c-106">Создание нового объекта [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="4483c-106">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4483c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4483c-107">Prerequisites</span></span>
<span data-ttu-id="4483c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4483c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4483c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4483c-110">Permission type</span></span>|<span data-ttu-id="4483c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4483c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4483c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4483c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4483c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4483c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4483c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4483c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4483c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4483c-115">Not supported.</span></span>|
|<span data-ttu-id="4483c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4483c-116">Application</span></span>|<span data-ttu-id="4483c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4483c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4483c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4483c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4483c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4483c-119">Request headers</span></span>
|<span data-ttu-id="4483c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4483c-120">Header</span></span>|<span data-ttu-id="4483c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4483c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4483c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4483c-122">Authorization</span></span>|<span data-ttu-id="4483c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4483c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4483c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4483c-124">Accept</span></span>|<span data-ttu-id="4483c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4483c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4483c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4483c-126">Request body</span></span>
<span data-ttu-id="4483c-127">В тексте запроса добавьте представление объекта Андроидманажедстореапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4483c-127">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="4483c-128">В следующей таблице приведены свойства, необходимые при создании Андроидманажедстореапп.</span><span class="sxs-lookup"><span data-stu-id="4483c-128">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="4483c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4483c-129">Property</span></span>|<span data-ttu-id="4483c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4483c-130">Type</span></span>|<span data-ttu-id="4483c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4483c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4483c-132">id</span><span class="sxs-lookup"><span data-stu-id="4483c-132">id</span></span>|<span data-ttu-id="4483c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4483c-133">String</span></span>|<span data-ttu-id="4483c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4483c-134">Key of the entity.</span></span> <span data-ttu-id="4483c-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4483c-136">displayName</span></span>|<span data-ttu-id="4483c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="4483c-137">String</span></span>|<span data-ttu-id="4483c-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="4483c-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4483c-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-140">description</span><span class="sxs-lookup"><span data-stu-id="4483c-140">description</span></span>|<span data-ttu-id="4483c-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4483c-141">String</span></span>|<span data-ttu-id="4483c-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="4483c-142">The description of the app.</span></span> <span data-ttu-id="4483c-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-144">publisher</span><span class="sxs-lookup"><span data-stu-id="4483c-144">publisher</span></span>|<span data-ttu-id="4483c-145">Строка</span><span class="sxs-lookup"><span data-stu-id="4483c-145">String</span></span>|<span data-ttu-id="4483c-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="4483c-146">The publisher of the app.</span></span> <span data-ttu-id="4483c-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4483c-148">largeIcon</span></span>|[<span data-ttu-id="4483c-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4483c-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4483c-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="4483c-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4483c-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4483c-152">createdDateTime</span></span>|<span data-ttu-id="4483c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4483c-153">DateTimeOffset</span></span>|<span data-ttu-id="4483c-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="4483c-154">The date and time the app was created.</span></span> <span data-ttu-id="4483c-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4483c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4483c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4483c-157">DateTimeOffset</span></span>|<span data-ttu-id="4483c-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="4483c-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4483c-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4483c-160">isFeatured</span></span>|<span data-ttu-id="4483c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4483c-161">Boolean</span></span>|<span data-ttu-id="4483c-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4483c-163">privacyInformationUrl</span></span>|<span data-ttu-id="4483c-164">Строка</span><span class="sxs-lookup"><span data-stu-id="4483c-164">String</span></span>|<span data-ttu-id="4483c-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4483c-165">The privacy statement Url.</span></span> <span data-ttu-id="4483c-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4483c-167">informationUrl</span></span>|<span data-ttu-id="4483c-168">Строка</span><span class="sxs-lookup"><span data-stu-id="4483c-168">String</span></span>|<span data-ttu-id="4483c-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="4483c-169">The more information Url.</span></span> <span data-ttu-id="4483c-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-171">owner</span><span class="sxs-lookup"><span data-stu-id="4483c-171">owner</span></span>|<span data-ttu-id="4483c-172">String</span><span class="sxs-lookup"><span data-stu-id="4483c-172">String</span></span>|<span data-ttu-id="4483c-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="4483c-173">The owner of the app.</span></span> <span data-ttu-id="4483c-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-175">developer</span><span class="sxs-lookup"><span data-stu-id="4483c-175">developer</span></span>|<span data-ttu-id="4483c-176">Строка</span><span class="sxs-lookup"><span data-stu-id="4483c-176">String</span></span>|<span data-ttu-id="4483c-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="4483c-177">The developer of the app.</span></span> <span data-ttu-id="4483c-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-179">notes</span><span class="sxs-lookup"><span data-stu-id="4483c-179">notes</span></span>|<span data-ttu-id="4483c-180">Строка</span><span class="sxs-lookup"><span data-stu-id="4483c-180">String</span></span>|<span data-ttu-id="4483c-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="4483c-181">Notes for the app.</span></span> <span data-ttu-id="4483c-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4483c-183">uploadState</span></span>|<span data-ttu-id="4483c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4483c-184">Int32</span></span>|<span data-ttu-id="4483c-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="4483c-185">The upload state.</span></span> <span data-ttu-id="4483c-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4483c-187">publishingState</span></span>|[<span data-ttu-id="4483c-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="4483c-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4483c-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="4483c-189">The publishing state for the app.</span></span> <span data-ttu-id="4483c-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="4483c-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4483c-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4483c-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4483c-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4483c-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4483c-193">isAssigned</span></span>|<span data-ttu-id="4483c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4483c-194">Boolean</span></span>|<span data-ttu-id="4483c-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="4483c-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4483c-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4483c-197">roleScopeTagIds</span></span>|<span data-ttu-id="4483c-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4483c-198">String collection</span></span>|<span data-ttu-id="4483c-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="4483c-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4483c-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="4483c-201">dependentAppCount</span></span>|<span data-ttu-id="4483c-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4483c-202">Int32</span></span>|<span data-ttu-id="4483c-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="4483c-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4483c-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4483c-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4483c-205">packageId</span><span class="sxs-lookup"><span data-stu-id="4483c-205">packageId</span></span>|<span data-ttu-id="4483c-206">Строка</span><span class="sxs-lookup"><span data-stu-id="4483c-206">String</span></span>|<span data-ttu-id="4483c-207">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="4483c-207">The package identifier.</span></span>|
|<span data-ttu-id="4483c-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="4483c-208">appIdentifier</span></span>|<span data-ttu-id="4483c-209">String</span><span class="sxs-lookup"><span data-stu-id="4483c-209">String</span></span>|<span data-ttu-id="4483c-210">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4483c-210">The Identity Name.</span></span>|
|<span data-ttu-id="4483c-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4483c-211">usedLicenseCount</span></span>|<span data-ttu-id="4483c-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4483c-212">Int32</span></span>|<span data-ttu-id="4483c-213">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="4483c-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="4483c-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4483c-214">totalLicenseCount</span></span>|<span data-ttu-id="4483c-215">Int32</span><span class="sxs-lookup"><span data-stu-id="4483c-215">Int32</span></span>|<span data-ttu-id="4483c-216">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="4483c-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="4483c-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4483c-217">appStoreUrl</span></span>|<span data-ttu-id="4483c-218">String</span><span class="sxs-lookup"><span data-stu-id="4483c-218">String</span></span>|<span data-ttu-id="4483c-219">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="4483c-219">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="4483c-220">Частный</span><span class="sxs-lookup"><span data-stu-id="4483c-220">isPrivate</span></span>|<span data-ttu-id="4483c-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="4483c-221">Boolean</span></span>|<span data-ttu-id="4483c-222">Указывает, доступно ли приложение только для указанных пользователей предприятия.</span><span class="sxs-lookup"><span data-stu-id="4483c-222">Indicates whether the app is only available to a given enterprise's users.</span></span>|
|<span data-ttu-id="4483c-223">иссистемапп</span><span class="sxs-lookup"><span data-stu-id="4483c-223">isSystemApp</span></span>|<span data-ttu-id="4483c-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="4483c-224">Boolean</span></span>|<span data-ttu-id="4483c-225">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="4483c-225">Indicates whether the app is a preinstalled system app.</span></span>|
|<span data-ttu-id="4483c-226">суппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="4483c-226">supportsOemConfig</span></span>|<span data-ttu-id="4483c-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="4483c-227">Boolean</span></span>|<span data-ttu-id="4483c-228">Поддерживает ли это приложение политику Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="4483c-228">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="4483c-229">Ответ</span><span class="sxs-lookup"><span data-stu-id="4483c-229">Response</span></span>
<span data-ttu-id="4483c-230">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4483c-230">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4483c-231">Пример</span><span class="sxs-lookup"><span data-stu-id="4483c-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="4483c-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="4483c-232">Request</span></span>
<span data-ttu-id="4483c-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4483c-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 984

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
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="4483c-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="4483c-234">Response</span></span>
<span data-ttu-id="4483c-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4483c-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1156

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
  "supportsOemConfig": true
}
```





