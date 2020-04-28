---
title: Создание Андроидманажедсторевебапп
description: Создание нового объекта Андроидманажедсторевебапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c23d0df9033aa0f92c09ef6664776a154b3cfa3e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43417416"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="7d3dc-103">Создание Андроидманажедсторевебапп</span><span class="sxs-lookup"><span data-stu-id="7d3dc-103">Create androidManagedStoreWebApp</span></span>

<span data-ttu-id="7d3dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d3dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d3dc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d3dc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d3dc-107">Создание нового объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7d3dc-107">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d3dc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7d3dc-108">Prerequisites</span></span>
<span data-ttu-id="7d3dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d3dc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d3dc-111">Permission type</span></span>|<span data-ttu-id="7d3dc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d3dc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d3dc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d3dc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d3dc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d3dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-116">Not supported.</span></span>|
|<span data-ttu-id="7d3dc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d3dc-117">Application</span></span>|<span data-ttu-id="7d3dc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d3dc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d3dc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d3dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7d3dc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7d3dc-120">Request headers</span></span>
|<span data-ttu-id="7d3dc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d3dc-121">Header</span></span>|<span data-ttu-id="7d3dc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7d3dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d3dc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d3dc-123">Authorization</span></span>|<span data-ttu-id="7d3dc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d3dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d3dc-125">Accept</span></span>|<span data-ttu-id="7d3dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d3dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d3dc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7d3dc-127">Request body</span></span>
<span data-ttu-id="7d3dc-128">В тексте запроса добавьте представление объекта Андроидманажедсторевебапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-128">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="7d3dc-129">В следующей таблице приведены свойства, необходимые при создании Андроидманажедсторевебапп.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-129">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="7d3dc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d3dc-130">Property</span></span>|<span data-ttu-id="7d3dc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7d3dc-131">Type</span></span>|<span data-ttu-id="7d3dc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7d3dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d3dc-133">id</span><span class="sxs-lookup"><span data-stu-id="7d3dc-133">id</span></span>|<span data-ttu-id="7d3dc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7d3dc-134">String</span></span>|<span data-ttu-id="7d3dc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-135">Key of the entity.</span></span> <span data-ttu-id="7d3dc-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7d3dc-137">displayName</span></span>|<span data-ttu-id="7d3dc-138">Строка</span><span class="sxs-lookup"><span data-stu-id="7d3dc-138">String</span></span>|<span data-ttu-id="7d3dc-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7d3dc-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-141">description</span><span class="sxs-lookup"><span data-stu-id="7d3dc-141">description</span></span>|<span data-ttu-id="7d3dc-142">Строка</span><span class="sxs-lookup"><span data-stu-id="7d3dc-142">String</span></span>|<span data-ttu-id="7d3dc-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-143">The description of the app.</span></span> <span data-ttu-id="7d3dc-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-145">publisher</span><span class="sxs-lookup"><span data-stu-id="7d3dc-145">publisher</span></span>|<span data-ttu-id="7d3dc-146">String</span><span class="sxs-lookup"><span data-stu-id="7d3dc-146">String</span></span>|<span data-ttu-id="7d3dc-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-147">The publisher of the app.</span></span> <span data-ttu-id="7d3dc-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7d3dc-149">largeIcon</span></span>|[<span data-ttu-id="7d3dc-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7d3dc-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7d3dc-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7d3dc-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d3dc-153">createdDateTime</span></span>|<span data-ttu-id="7d3dc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d3dc-154">DateTimeOffset</span></span>|<span data-ttu-id="7d3dc-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-155">The date and time the app was created.</span></span> <span data-ttu-id="7d3dc-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d3dc-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7d3dc-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d3dc-158">DateTimeOffset</span></span>|<span data-ttu-id="7d3dc-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-159">The date and time the app was last modified.</span></span> <span data-ttu-id="7d3dc-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7d3dc-161">isFeatured</span></span>|<span data-ttu-id="7d3dc-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3dc-162">Boolean</span></span>|<span data-ttu-id="7d3dc-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7d3dc-164">privacyInformationUrl</span></span>|<span data-ttu-id="7d3dc-165">String</span><span class="sxs-lookup"><span data-stu-id="7d3dc-165">String</span></span>|<span data-ttu-id="7d3dc-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-166">The privacy statement Url.</span></span> <span data-ttu-id="7d3dc-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7d3dc-168">informationUrl</span></span>|<span data-ttu-id="7d3dc-169">String</span><span class="sxs-lookup"><span data-stu-id="7d3dc-169">String</span></span>|<span data-ttu-id="7d3dc-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-170">The more information Url.</span></span> <span data-ttu-id="7d3dc-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-172">owner</span><span class="sxs-lookup"><span data-stu-id="7d3dc-172">owner</span></span>|<span data-ttu-id="7d3dc-173">String</span><span class="sxs-lookup"><span data-stu-id="7d3dc-173">String</span></span>|<span data-ttu-id="7d3dc-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-174">The owner of the app.</span></span> <span data-ttu-id="7d3dc-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-176">developer</span><span class="sxs-lookup"><span data-stu-id="7d3dc-176">developer</span></span>|<span data-ttu-id="7d3dc-177">String</span><span class="sxs-lookup"><span data-stu-id="7d3dc-177">String</span></span>|<span data-ttu-id="7d3dc-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-178">The developer of the app.</span></span> <span data-ttu-id="7d3dc-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-180">notes</span><span class="sxs-lookup"><span data-stu-id="7d3dc-180">notes</span></span>|<span data-ttu-id="7d3dc-181">String</span><span class="sxs-lookup"><span data-stu-id="7d3dc-181">String</span></span>|<span data-ttu-id="7d3dc-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-182">Notes for the app.</span></span> <span data-ttu-id="7d3dc-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="7d3dc-184">uploadState</span></span>|<span data-ttu-id="7d3dc-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7d3dc-185">Int32</span></span>|<span data-ttu-id="7d3dc-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-186">The upload state.</span></span> <span data-ttu-id="7d3dc-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="7d3dc-188">publishingState</span></span>|[<span data-ttu-id="7d3dc-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="7d3dc-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7d3dc-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-190">The publishing state for the app.</span></span> <span data-ttu-id="7d3dc-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7d3dc-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="7d3dc-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7d3dc-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7d3dc-194">isAssigned</span></span>|<span data-ttu-id="7d3dc-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3dc-195">Boolean</span></span>|<span data-ttu-id="7d3dc-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7d3dc-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7d3dc-198">roleScopeTagIds</span></span>|<span data-ttu-id="7d3dc-199">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="7d3dc-199">String collection</span></span>|<span data-ttu-id="7d3dc-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7d3dc-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="7d3dc-202">dependentAppCount</span></span>|<span data-ttu-id="7d3dc-203">Int32</span><span class="sxs-lookup"><span data-stu-id="7d3dc-203">Int32</span></span>|<span data-ttu-id="7d3dc-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7d3dc-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7d3dc-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7d3dc-206">packageId</span><span class="sxs-lookup"><span data-stu-id="7d3dc-206">packageId</span></span>|<span data-ttu-id="7d3dc-207">String</span><span class="sxs-lookup"><span data-stu-id="7d3dc-207">String</span></span>|<span data-ttu-id="7d3dc-208">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-208">The package identifier.</span></span> <span data-ttu-id="7d3dc-209">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-209">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7d3dc-210">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="7d3dc-210">appIdentifier</span></span>|<span data-ttu-id="7d3dc-211">String</span><span class="sxs-lookup"><span data-stu-id="7d3dc-211">String</span></span>|<span data-ttu-id="7d3dc-212">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-212">The Identity Name.</span></span> <span data-ttu-id="7d3dc-213">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-213">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7d3dc-214">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7d3dc-214">usedLicenseCount</span></span>|<span data-ttu-id="7d3dc-215">Int32</span><span class="sxs-lookup"><span data-stu-id="7d3dc-215">Int32</span></span>|<span data-ttu-id="7d3dc-216">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-216">The number of VPP licenses in use.</span></span> <span data-ttu-id="7d3dc-217">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-217">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7d3dc-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7d3dc-218">totalLicenseCount</span></span>|<span data-ttu-id="7d3dc-219">Int32</span><span class="sxs-lookup"><span data-stu-id="7d3dc-219">Int32</span></span>|<span data-ttu-id="7d3dc-220">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-220">The total number of VPP licenses.</span></span> <span data-ttu-id="7d3dc-221">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-221">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7d3dc-222">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7d3dc-222">appStoreUrl</span></span>|<span data-ttu-id="7d3dc-223">String</span><span class="sxs-lookup"><span data-stu-id="7d3dc-223">String</span></span>|<span data-ttu-id="7d3dc-224">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-224">The Play for Work Store app URL.</span></span> <span data-ttu-id="7d3dc-225">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-225">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7d3dc-226">Частный</span><span class="sxs-lookup"><span data-stu-id="7d3dc-226">isPrivate</span></span>|<span data-ttu-id="7d3dc-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3dc-227">Boolean</span></span>|<span data-ttu-id="7d3dc-228">Указывает, доступно ли приложение только для указанных пользователей предприятия.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-228">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="7d3dc-229">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-229">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7d3dc-230">иссистемапп</span><span class="sxs-lookup"><span data-stu-id="7d3dc-230">isSystemApp</span></span>|<span data-ttu-id="7d3dc-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3dc-231">Boolean</span></span>|<span data-ttu-id="7d3dc-232">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-232">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="7d3dc-233">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-233">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7d3dc-234">апптраккс</span><span class="sxs-lookup"><span data-stu-id="7d3dc-234">appTracks</span></span>|<span data-ttu-id="7d3dc-235">Коллекция [андроидманажедстореапптракк](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-235">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="7d3dc-236">Дорожки, которые видимы для этого предприятия.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-236">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="7d3dc-237">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-237">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7d3dc-238">суппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="7d3dc-238">supportsOemConfig</span></span>|<span data-ttu-id="7d3dc-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d3dc-239">Boolean</span></span>|<span data-ttu-id="7d3dc-240">Поддерживает ли это приложение политику Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-240">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="7d3dc-241">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7d3dc-241">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7d3dc-242">Ответ</span><span class="sxs-lookup"><span data-stu-id="7d3dc-242">Response</span></span>
<span data-ttu-id="7d3dc-243">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-243">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d3dc-244">Пример</span><span class="sxs-lookup"><span data-stu-id="7d3dc-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d3dc-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d3dc-245">Request</span></span>
<span data-ttu-id="7d3dc-246">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1171

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

### <a name="response"></a><span data-ttu-id="7d3dc-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d3dc-247">Response</span></span>
<span data-ttu-id="7d3dc-p128">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d3dc-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1343

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



