---
title: Создание Андроидманажедстореапп
description: Создание нового объекта Андроидманажедстореапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 758456e0e02780ce3cf839df75953abee72bf8e4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445948"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="95c50-103">Создание Андроидманажедстореапп</span><span class="sxs-lookup"><span data-stu-id="95c50-103">Create androidManagedStoreApp</span></span>

<span data-ttu-id="95c50-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="95c50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95c50-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95c50-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95c50-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95c50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95c50-107">Создание нового объекта [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="95c50-107">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95c50-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="95c50-108">Prerequisites</span></span>
<span data-ttu-id="95c50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95c50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95c50-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95c50-111">Permission type</span></span>|<span data-ttu-id="95c50-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95c50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95c50-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95c50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95c50-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95c50-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95c50-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95c50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95c50-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95c50-116">Not supported.</span></span>|
|<span data-ttu-id="95c50-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95c50-117">Application</span></span>|<span data-ttu-id="95c50-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95c50-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95c50-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95c50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="95c50-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="95c50-120">Request headers</span></span>
|<span data-ttu-id="95c50-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95c50-121">Header</span></span>|<span data-ttu-id="95c50-122">Значение</span><span class="sxs-lookup"><span data-stu-id="95c50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95c50-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95c50-123">Authorization</span></span>|<span data-ttu-id="95c50-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95c50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95c50-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95c50-125">Accept</span></span>|<span data-ttu-id="95c50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95c50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95c50-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95c50-127">Request body</span></span>
<span data-ttu-id="95c50-128">В тексте запроса добавьте представление объекта Андроидманажедстореапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95c50-128">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="95c50-129">В следующей таблице приведены свойства, необходимые при создании Андроидманажедстореапп.</span><span class="sxs-lookup"><span data-stu-id="95c50-129">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="95c50-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="95c50-130">Property</span></span>|<span data-ttu-id="95c50-131">Тип</span><span class="sxs-lookup"><span data-stu-id="95c50-131">Type</span></span>|<span data-ttu-id="95c50-132">Описание</span><span class="sxs-lookup"><span data-stu-id="95c50-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95c50-133">id</span><span class="sxs-lookup"><span data-stu-id="95c50-133">id</span></span>|<span data-ttu-id="95c50-134">Строка</span><span class="sxs-lookup"><span data-stu-id="95c50-134">String</span></span>|<span data-ttu-id="95c50-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="95c50-135">Key of the entity.</span></span> <span data-ttu-id="95c50-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-137">displayName</span><span class="sxs-lookup"><span data-stu-id="95c50-137">displayName</span></span>|<span data-ttu-id="95c50-138">Строка</span><span class="sxs-lookup"><span data-stu-id="95c50-138">String</span></span>|<span data-ttu-id="95c50-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="95c50-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="95c50-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-141">description</span><span class="sxs-lookup"><span data-stu-id="95c50-141">description</span></span>|<span data-ttu-id="95c50-142">Строка</span><span class="sxs-lookup"><span data-stu-id="95c50-142">String</span></span>|<span data-ttu-id="95c50-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="95c50-143">The description of the app.</span></span> <span data-ttu-id="95c50-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-145">publisher</span><span class="sxs-lookup"><span data-stu-id="95c50-145">publisher</span></span>|<span data-ttu-id="95c50-146">String</span><span class="sxs-lookup"><span data-stu-id="95c50-146">String</span></span>|<span data-ttu-id="95c50-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="95c50-147">The publisher of the app.</span></span> <span data-ttu-id="95c50-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="95c50-149">largeIcon</span></span>|[<span data-ttu-id="95c50-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="95c50-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="95c50-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="95c50-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="95c50-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95c50-153">createdDateTime</span></span>|<span data-ttu-id="95c50-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95c50-154">DateTimeOffset</span></span>|<span data-ttu-id="95c50-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="95c50-155">The date and time the app was created.</span></span> <span data-ttu-id="95c50-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95c50-157">lastModifiedDateTime</span></span>|<span data-ttu-id="95c50-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95c50-158">DateTimeOffset</span></span>|<span data-ttu-id="95c50-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="95c50-159">The date and time the app was last modified.</span></span> <span data-ttu-id="95c50-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="95c50-161">isFeatured</span></span>|<span data-ttu-id="95c50-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="95c50-162">Boolean</span></span>|<span data-ttu-id="95c50-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="95c50-164">privacyInformationUrl</span></span>|<span data-ttu-id="95c50-165">String</span><span class="sxs-lookup"><span data-stu-id="95c50-165">String</span></span>|<span data-ttu-id="95c50-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="95c50-166">The privacy statement Url.</span></span> <span data-ttu-id="95c50-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="95c50-168">informationUrl</span></span>|<span data-ttu-id="95c50-169">String</span><span class="sxs-lookup"><span data-stu-id="95c50-169">String</span></span>|<span data-ttu-id="95c50-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="95c50-170">The more information Url.</span></span> <span data-ttu-id="95c50-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-172">owner</span><span class="sxs-lookup"><span data-stu-id="95c50-172">owner</span></span>|<span data-ttu-id="95c50-173">String</span><span class="sxs-lookup"><span data-stu-id="95c50-173">String</span></span>|<span data-ttu-id="95c50-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="95c50-174">The owner of the app.</span></span> <span data-ttu-id="95c50-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-176">developer</span><span class="sxs-lookup"><span data-stu-id="95c50-176">developer</span></span>|<span data-ttu-id="95c50-177">String</span><span class="sxs-lookup"><span data-stu-id="95c50-177">String</span></span>|<span data-ttu-id="95c50-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="95c50-178">The developer of the app.</span></span> <span data-ttu-id="95c50-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-180">notes</span><span class="sxs-lookup"><span data-stu-id="95c50-180">notes</span></span>|<span data-ttu-id="95c50-181">String</span><span class="sxs-lookup"><span data-stu-id="95c50-181">String</span></span>|<span data-ttu-id="95c50-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="95c50-182">Notes for the app.</span></span> <span data-ttu-id="95c50-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="95c50-184">uploadState</span></span>|<span data-ttu-id="95c50-185">Int32</span><span class="sxs-lookup"><span data-stu-id="95c50-185">Int32</span></span>|<span data-ttu-id="95c50-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="95c50-186">The upload state.</span></span> <span data-ttu-id="95c50-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="95c50-188">publishingState</span></span>|[<span data-ttu-id="95c50-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="95c50-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="95c50-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="95c50-190">The publishing state for the app.</span></span> <span data-ttu-id="95c50-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="95c50-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="95c50-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="95c50-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="95c50-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="95c50-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="95c50-194">isAssigned</span></span>|<span data-ttu-id="95c50-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="95c50-195">Boolean</span></span>|<span data-ttu-id="95c50-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="95c50-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="95c50-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95c50-198">roleScopeTagIds</span></span>|<span data-ttu-id="95c50-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="95c50-199">String collection</span></span>|<span data-ttu-id="95c50-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="95c50-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="95c50-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="95c50-202">dependentAppCount</span></span>|<span data-ttu-id="95c50-203">Int32</span><span class="sxs-lookup"><span data-stu-id="95c50-203">Int32</span></span>|<span data-ttu-id="95c50-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="95c50-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="95c50-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95c50-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="95c50-206">packageId</span><span class="sxs-lookup"><span data-stu-id="95c50-206">packageId</span></span>|<span data-ttu-id="95c50-207">String</span><span class="sxs-lookup"><span data-stu-id="95c50-207">String</span></span>|<span data-ttu-id="95c50-208">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="95c50-208">The package identifier.</span></span>|
|<span data-ttu-id="95c50-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="95c50-209">appIdentifier</span></span>|<span data-ttu-id="95c50-210">String</span><span class="sxs-lookup"><span data-stu-id="95c50-210">String</span></span>|<span data-ttu-id="95c50-211">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="95c50-211">The Identity Name.</span></span>|
|<span data-ttu-id="95c50-212">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="95c50-212">usedLicenseCount</span></span>|<span data-ttu-id="95c50-213">Int32</span><span class="sxs-lookup"><span data-stu-id="95c50-213">Int32</span></span>|<span data-ttu-id="95c50-214">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="95c50-214">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="95c50-215">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="95c50-215">totalLicenseCount</span></span>|<span data-ttu-id="95c50-216">Int32</span><span class="sxs-lookup"><span data-stu-id="95c50-216">Int32</span></span>|<span data-ttu-id="95c50-217">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="95c50-217">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="95c50-218">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="95c50-218">appStoreUrl</span></span>|<span data-ttu-id="95c50-219">String</span><span class="sxs-lookup"><span data-stu-id="95c50-219">String</span></span>|<span data-ttu-id="95c50-220">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="95c50-220">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="95c50-221">Частный</span><span class="sxs-lookup"><span data-stu-id="95c50-221">isPrivate</span></span>|<span data-ttu-id="95c50-222">Логический</span><span class="sxs-lookup"><span data-stu-id="95c50-222">Boolean</span></span>|<span data-ttu-id="95c50-223">Указывает, доступно ли приложение только для указанных пользователей предприятия.</span><span class="sxs-lookup"><span data-stu-id="95c50-223">Indicates whether the app is only available to a given enterprise's users.</span></span>|
|<span data-ttu-id="95c50-224">иссистемапп</span><span class="sxs-lookup"><span data-stu-id="95c50-224">isSystemApp</span></span>|<span data-ttu-id="95c50-225">Логический</span><span class="sxs-lookup"><span data-stu-id="95c50-225">Boolean</span></span>|<span data-ttu-id="95c50-226">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="95c50-226">Indicates whether the app is a preinstalled system app.</span></span>|
|<span data-ttu-id="95c50-227">суппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="95c50-227">supportsOemConfig</span></span>|<span data-ttu-id="95c50-228">Логический</span><span class="sxs-lookup"><span data-stu-id="95c50-228">Boolean</span></span>|<span data-ttu-id="95c50-229">Поддерживает ли это приложение политику Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="95c50-229">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="95c50-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="95c50-230">Response</span></span>
<span data-ttu-id="95c50-231">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95c50-231">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95c50-232">Пример</span><span class="sxs-lookup"><span data-stu-id="95c50-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="95c50-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="95c50-233">Request</span></span>
<span data-ttu-id="95c50-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95c50-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="95c50-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="95c50-235">Response</span></span>
<span data-ttu-id="95c50-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95c50-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





