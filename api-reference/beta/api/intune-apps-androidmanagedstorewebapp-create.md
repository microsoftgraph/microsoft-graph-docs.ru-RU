---
title: Создание Андроидманажедсторевебапп
description: Создание нового объекта Андроидманажедсторевебапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd6b656729bcd5fcbeda2308966cf2581368c3e4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445864"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="d7d67-103">Создание Андроидманажедсторевебапп</span><span class="sxs-lookup"><span data-stu-id="d7d67-103">Create androidManagedStoreWebApp</span></span>

<span data-ttu-id="d7d67-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d7d67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7d67-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7d67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7d67-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7d67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7d67-107">Создание нового объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="d7d67-107">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7d67-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d7d67-108">Prerequisites</span></span>
<span data-ttu-id="d7d67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7d67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7d67-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7d67-111">Permission type</span></span>|<span data-ttu-id="d7d67-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7d67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7d67-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7d67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7d67-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7d67-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d7d67-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7d67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7d67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7d67-116">Not supported.</span></span>|
|<span data-ttu-id="d7d67-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7d67-117">Application</span></span>|<span data-ttu-id="d7d67-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7d67-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7d67-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7d67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d7d67-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d7d67-120">Request headers</span></span>
|<span data-ttu-id="d7d67-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7d67-121">Header</span></span>|<span data-ttu-id="d7d67-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d7d67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7d67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7d67-123">Authorization</span></span>|<span data-ttu-id="d7d67-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7d67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7d67-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7d67-125">Accept</span></span>|<span data-ttu-id="d7d67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7d67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7d67-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7d67-127">Request body</span></span>
<span data-ttu-id="d7d67-128">В тексте запроса добавьте представление объекта Андроидманажедсторевебапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7d67-128">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="d7d67-129">В следующей таблице приведены свойства, необходимые при создании Андроидманажедсторевебапп.</span><span class="sxs-lookup"><span data-stu-id="d7d67-129">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="d7d67-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7d67-130">Property</span></span>|<span data-ttu-id="d7d67-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d7d67-131">Type</span></span>|<span data-ttu-id="d7d67-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d7d67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7d67-133">id</span><span class="sxs-lookup"><span data-stu-id="d7d67-133">id</span></span>|<span data-ttu-id="d7d67-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d7d67-134">String</span></span>|<span data-ttu-id="d7d67-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d7d67-135">Key of the entity.</span></span> <span data-ttu-id="d7d67-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d7d67-137">displayName</span></span>|<span data-ttu-id="d7d67-138">Строка</span><span class="sxs-lookup"><span data-stu-id="d7d67-138">String</span></span>|<span data-ttu-id="d7d67-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d7d67-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d7d67-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-141">description</span><span class="sxs-lookup"><span data-stu-id="d7d67-141">description</span></span>|<span data-ttu-id="d7d67-142">Строка</span><span class="sxs-lookup"><span data-stu-id="d7d67-142">String</span></span>|<span data-ttu-id="d7d67-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d67-143">The description of the app.</span></span> <span data-ttu-id="d7d67-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d7d67-145">publisher</span></span>|<span data-ttu-id="d7d67-146">String</span><span class="sxs-lookup"><span data-stu-id="d7d67-146">String</span></span>|<span data-ttu-id="d7d67-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d67-147">The publisher of the app.</span></span> <span data-ttu-id="d7d67-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d7d67-149">largeIcon</span></span>|[<span data-ttu-id="d7d67-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d7d67-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d7d67-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d7d67-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d7d67-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7d67-153">createdDateTime</span></span>|<span data-ttu-id="d7d67-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7d67-154">DateTimeOffset</span></span>|<span data-ttu-id="d7d67-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d67-155">The date and time the app was created.</span></span> <span data-ttu-id="d7d67-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7d67-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d7d67-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7d67-158">DateTimeOffset</span></span>|<span data-ttu-id="d7d67-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d67-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d7d67-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d7d67-161">isFeatured</span></span>|<span data-ttu-id="d7d67-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7d67-162">Boolean</span></span>|<span data-ttu-id="d7d67-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d7d67-164">privacyInformationUrl</span></span>|<span data-ttu-id="d7d67-165">String</span><span class="sxs-lookup"><span data-stu-id="d7d67-165">String</span></span>|<span data-ttu-id="d7d67-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d7d67-166">The privacy statement Url.</span></span> <span data-ttu-id="d7d67-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d7d67-168">informationUrl</span></span>|<span data-ttu-id="d7d67-169">String</span><span class="sxs-lookup"><span data-stu-id="d7d67-169">String</span></span>|<span data-ttu-id="d7d67-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d7d67-170">The more information Url.</span></span> <span data-ttu-id="d7d67-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-172">owner</span><span class="sxs-lookup"><span data-stu-id="d7d67-172">owner</span></span>|<span data-ttu-id="d7d67-173">String</span><span class="sxs-lookup"><span data-stu-id="d7d67-173">String</span></span>|<span data-ttu-id="d7d67-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d67-174">The owner of the app.</span></span> <span data-ttu-id="d7d67-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-176">developer</span><span class="sxs-lookup"><span data-stu-id="d7d67-176">developer</span></span>|<span data-ttu-id="d7d67-177">String</span><span class="sxs-lookup"><span data-stu-id="d7d67-177">String</span></span>|<span data-ttu-id="d7d67-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d67-178">The developer of the app.</span></span> <span data-ttu-id="d7d67-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-180">notes</span><span class="sxs-lookup"><span data-stu-id="d7d67-180">notes</span></span>|<span data-ttu-id="d7d67-181">String</span><span class="sxs-lookup"><span data-stu-id="d7d67-181">String</span></span>|<span data-ttu-id="d7d67-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d67-182">Notes for the app.</span></span> <span data-ttu-id="d7d67-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d7d67-184">uploadState</span></span>|<span data-ttu-id="d7d67-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d7d67-185">Int32</span></span>|<span data-ttu-id="d7d67-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="d7d67-186">The upload state.</span></span> <span data-ttu-id="d7d67-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d7d67-188">publishingState</span></span>|[<span data-ttu-id="d7d67-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="d7d67-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d7d67-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d67-190">The publishing state for the app.</span></span> <span data-ttu-id="d7d67-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d7d67-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d7d67-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="d7d67-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d7d67-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d7d67-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d7d67-194">isAssigned</span></span>|<span data-ttu-id="d7d67-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7d67-195">Boolean</span></span>|<span data-ttu-id="d7d67-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="d7d67-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d7d67-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d7d67-198">roleScopeTagIds</span></span>|<span data-ttu-id="d7d67-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d7d67-199">String collection</span></span>|<span data-ttu-id="d7d67-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d67-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d7d67-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="d7d67-202">dependentAppCount</span></span>|<span data-ttu-id="d7d67-203">Int32</span><span class="sxs-lookup"><span data-stu-id="d7d67-203">Int32</span></span>|<span data-ttu-id="d7d67-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="d7d67-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d7d67-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7d67-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d7d67-206">packageId</span><span class="sxs-lookup"><span data-stu-id="d7d67-206">packageId</span></span>|<span data-ttu-id="d7d67-207">String</span><span class="sxs-lookup"><span data-stu-id="d7d67-207">String</span></span>|<span data-ttu-id="d7d67-208">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="d7d67-208">The package identifier.</span></span> <span data-ttu-id="d7d67-209">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7d67-209">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d7d67-210">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d7d67-210">appIdentifier</span></span>|<span data-ttu-id="d7d67-211">String</span><span class="sxs-lookup"><span data-stu-id="d7d67-211">String</span></span>|<span data-ttu-id="d7d67-212">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d7d67-212">The Identity Name.</span></span> <span data-ttu-id="d7d67-213">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7d67-213">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d7d67-214">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d7d67-214">usedLicenseCount</span></span>|<span data-ttu-id="d7d67-215">Int32</span><span class="sxs-lookup"><span data-stu-id="d7d67-215">Int32</span></span>|<span data-ttu-id="d7d67-216">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="d7d67-216">The number of VPP licenses in use.</span></span> <span data-ttu-id="d7d67-217">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7d67-217">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d7d67-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="d7d67-218">totalLicenseCount</span></span>|<span data-ttu-id="d7d67-219">Int32</span><span class="sxs-lookup"><span data-stu-id="d7d67-219">Int32</span></span>|<span data-ttu-id="d7d67-220">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="d7d67-220">The total number of VPP licenses.</span></span> <span data-ttu-id="d7d67-221">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7d67-221">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d7d67-222">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d7d67-222">appStoreUrl</span></span>|<span data-ttu-id="d7d67-223">String</span><span class="sxs-lookup"><span data-stu-id="d7d67-223">String</span></span>|<span data-ttu-id="d7d67-224">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="d7d67-224">The Play for Work Store app URL.</span></span> <span data-ttu-id="d7d67-225">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7d67-225">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d7d67-226">Частный</span><span class="sxs-lookup"><span data-stu-id="d7d67-226">isPrivate</span></span>|<span data-ttu-id="d7d67-227">Логический</span><span class="sxs-lookup"><span data-stu-id="d7d67-227">Boolean</span></span>|<span data-ttu-id="d7d67-228">Указывает, доступно ли приложение только для указанных пользователей предприятия.</span><span class="sxs-lookup"><span data-stu-id="d7d67-228">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="d7d67-229">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7d67-229">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d7d67-230">иссистемапп</span><span class="sxs-lookup"><span data-stu-id="d7d67-230">isSystemApp</span></span>|<span data-ttu-id="d7d67-231">Логический</span><span class="sxs-lookup"><span data-stu-id="d7d67-231">Boolean</span></span>|<span data-ttu-id="d7d67-232">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="d7d67-232">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="d7d67-233">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7d67-233">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="d7d67-234">суппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="d7d67-234">supportsOemConfig</span></span>|<span data-ttu-id="d7d67-235">Логический</span><span class="sxs-lookup"><span data-stu-id="d7d67-235">Boolean</span></span>|<span data-ttu-id="d7d67-236">Поддерживает ли это приложение политику Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="d7d67-236">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="d7d67-237">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7d67-237">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d7d67-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7d67-238">Response</span></span>
<span data-ttu-id="d7d67-239">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7d67-239">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7d67-240">Пример</span><span class="sxs-lookup"><span data-stu-id="d7d67-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7d67-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7d67-241">Request</span></span>
<span data-ttu-id="d7d67-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7d67-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d7d67-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7d67-243">Response</span></span>
<span data-ttu-id="d7d67-p127">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7d67-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





