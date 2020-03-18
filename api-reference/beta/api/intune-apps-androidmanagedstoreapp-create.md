---
title: Создание Андроидманажедстореапп
description: Создание нового объекта Андроидманажедстореапп.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b33eae221380f75b80bd17def157e1f2a507830e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42762268"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="2e3e8-103">Создание Андроидманажедстореапп</span><span class="sxs-lookup"><span data-stu-id="2e3e8-103">Create androidManagedStoreApp</span></span>

> <span data-ttu-id="2e3e8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e3e8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e3e8-106">Создание нового объекта [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="2e3e8-106">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e3e8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2e3e8-107">Prerequisites</span></span>
<span data-ttu-id="2e3e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e3e8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e3e8-110">Permission type</span></span>|<span data-ttu-id="2e3e8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e3e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e3e8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e3e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e3e8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e3e8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2e3e8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e3e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e3e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-115">Not supported.</span></span>|
|<span data-ttu-id="2e3e8-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2e3e8-116">Application</span></span>|<span data-ttu-id="2e3e8-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e3e8-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e3e8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e3e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2e3e8-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2e3e8-119">Request headers</span></span>
|<span data-ttu-id="2e3e8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e3e8-120">Header</span></span>|<span data-ttu-id="2e3e8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2e3e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e3e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e3e8-122">Authorization</span></span>|<span data-ttu-id="2e3e8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e3e8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2e3e8-124">Accept</span></span>|<span data-ttu-id="2e3e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e3e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e3e8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e3e8-126">Request body</span></span>
<span data-ttu-id="2e3e8-127">В тексте запроса добавьте представление объекта Андроидманажедстореапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-127">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="2e3e8-128">В следующей таблице приведены свойства, необходимые при создании Андроидманажедстореапп.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-128">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="2e3e8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e3e8-129">Property</span></span>|<span data-ttu-id="2e3e8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2e3e8-130">Type</span></span>|<span data-ttu-id="2e3e8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2e3e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e3e8-132">id</span><span class="sxs-lookup"><span data-stu-id="2e3e8-132">id</span></span>|<span data-ttu-id="2e3e8-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2e3e8-133">String</span></span>|<span data-ttu-id="2e3e8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-134">Key of the entity.</span></span> <span data-ttu-id="2e3e8-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2e3e8-136">displayName</span></span>|<span data-ttu-id="2e3e8-137">Строка</span><span class="sxs-lookup"><span data-stu-id="2e3e8-137">String</span></span>|<span data-ttu-id="2e3e8-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2e3e8-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-140">description</span><span class="sxs-lookup"><span data-stu-id="2e3e8-140">description</span></span>|<span data-ttu-id="2e3e8-141">Строка</span><span class="sxs-lookup"><span data-stu-id="2e3e8-141">String</span></span>|<span data-ttu-id="2e3e8-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-142">The description of the app.</span></span> <span data-ttu-id="2e3e8-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-144">publisher</span><span class="sxs-lookup"><span data-stu-id="2e3e8-144">publisher</span></span>|<span data-ttu-id="2e3e8-145">String</span><span class="sxs-lookup"><span data-stu-id="2e3e8-145">String</span></span>|<span data-ttu-id="2e3e8-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-146">The publisher of the app.</span></span> <span data-ttu-id="2e3e8-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2e3e8-148">largeIcon</span></span>|[<span data-ttu-id="2e3e8-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2e3e8-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2e3e8-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2e3e8-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e3e8-152">createdDateTime</span></span>|<span data-ttu-id="2e3e8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e3e8-153">DateTimeOffset</span></span>|<span data-ttu-id="2e3e8-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-154">The date and time the app was created.</span></span> <span data-ttu-id="2e3e8-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e3e8-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2e3e8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e3e8-157">DateTimeOffset</span></span>|<span data-ttu-id="2e3e8-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2e3e8-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2e3e8-160">isFeatured</span></span>|<span data-ttu-id="2e3e8-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e3e8-161">Boolean</span></span>|<span data-ttu-id="2e3e8-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2e3e8-163">privacyInformationUrl</span></span>|<span data-ttu-id="2e3e8-164">String</span><span class="sxs-lookup"><span data-stu-id="2e3e8-164">String</span></span>|<span data-ttu-id="2e3e8-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-165">The privacy statement Url.</span></span> <span data-ttu-id="2e3e8-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2e3e8-167">informationUrl</span></span>|<span data-ttu-id="2e3e8-168">String</span><span class="sxs-lookup"><span data-stu-id="2e3e8-168">String</span></span>|<span data-ttu-id="2e3e8-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-169">The more information Url.</span></span> <span data-ttu-id="2e3e8-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-171">owner</span><span class="sxs-lookup"><span data-stu-id="2e3e8-171">owner</span></span>|<span data-ttu-id="2e3e8-172">String</span><span class="sxs-lookup"><span data-stu-id="2e3e8-172">String</span></span>|<span data-ttu-id="2e3e8-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-173">The owner of the app.</span></span> <span data-ttu-id="2e3e8-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-175">developer</span><span class="sxs-lookup"><span data-stu-id="2e3e8-175">developer</span></span>|<span data-ttu-id="2e3e8-176">String</span><span class="sxs-lookup"><span data-stu-id="2e3e8-176">String</span></span>|<span data-ttu-id="2e3e8-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-177">The developer of the app.</span></span> <span data-ttu-id="2e3e8-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-179">notes</span><span class="sxs-lookup"><span data-stu-id="2e3e8-179">notes</span></span>|<span data-ttu-id="2e3e8-180">String</span><span class="sxs-lookup"><span data-stu-id="2e3e8-180">String</span></span>|<span data-ttu-id="2e3e8-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-181">Notes for the app.</span></span> <span data-ttu-id="2e3e8-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="2e3e8-183">uploadState</span></span>|<span data-ttu-id="2e3e8-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3e8-184">Int32</span></span>|<span data-ttu-id="2e3e8-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-185">The upload state.</span></span> <span data-ttu-id="2e3e8-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="2e3e8-187">publishingState</span></span>|[<span data-ttu-id="2e3e8-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="2e3e8-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2e3e8-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-189">The publishing state for the app.</span></span> <span data-ttu-id="2e3e8-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2e3e8-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="2e3e8-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2e3e8-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2e3e8-193">isAssigned</span></span>|<span data-ttu-id="2e3e8-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e3e8-194">Boolean</span></span>|<span data-ttu-id="2e3e8-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2e3e8-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2e3e8-197">roleScopeTagIds</span></span>|<span data-ttu-id="2e3e8-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2e3e8-198">String collection</span></span>|<span data-ttu-id="2e3e8-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2e3e8-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="2e3e8-201">dependentAppCount</span></span>|<span data-ttu-id="2e3e8-202">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3e8-202">Int32</span></span>|<span data-ttu-id="2e3e8-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="2e3e8-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e3e8-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2e3e8-205">packageId</span><span class="sxs-lookup"><span data-stu-id="2e3e8-205">packageId</span></span>|<span data-ttu-id="2e3e8-206">String</span><span class="sxs-lookup"><span data-stu-id="2e3e8-206">String</span></span>|<span data-ttu-id="2e3e8-207">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-207">The package identifier.</span></span>|
|<span data-ttu-id="2e3e8-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="2e3e8-208">appIdentifier</span></span>|<span data-ttu-id="2e3e8-209">String</span><span class="sxs-lookup"><span data-stu-id="2e3e8-209">String</span></span>|<span data-ttu-id="2e3e8-210">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-210">The Identity Name.</span></span>|
|<span data-ttu-id="2e3e8-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2e3e8-211">usedLicenseCount</span></span>|<span data-ttu-id="2e3e8-212">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3e8-212">Int32</span></span>|<span data-ttu-id="2e3e8-213">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="2e3e8-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2e3e8-214">totalLicenseCount</span></span>|<span data-ttu-id="2e3e8-215">Int32</span><span class="sxs-lookup"><span data-stu-id="2e3e8-215">Int32</span></span>|<span data-ttu-id="2e3e8-216">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="2e3e8-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2e3e8-217">appStoreUrl</span></span>|<span data-ttu-id="2e3e8-218">String</span><span class="sxs-lookup"><span data-stu-id="2e3e8-218">String</span></span>|<span data-ttu-id="2e3e8-219">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-219">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="2e3e8-220">Частный</span><span class="sxs-lookup"><span data-stu-id="2e3e8-220">isPrivate</span></span>|<span data-ttu-id="2e3e8-221">Логический</span><span class="sxs-lookup"><span data-stu-id="2e3e8-221">Boolean</span></span>|<span data-ttu-id="2e3e8-222">Указывает, доступно ли приложение только для указанных пользователей предприятия.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-222">Indicates whether the app is only available to a given enterprise's users.</span></span>|
|<span data-ttu-id="2e3e8-223">иссистемапп</span><span class="sxs-lookup"><span data-stu-id="2e3e8-223">isSystemApp</span></span>|<span data-ttu-id="2e3e8-224">Логический</span><span class="sxs-lookup"><span data-stu-id="2e3e8-224">Boolean</span></span>|<span data-ttu-id="2e3e8-225">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-225">Indicates whether the app is a preinstalled system app.</span></span>|
|<span data-ttu-id="2e3e8-226">суппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="2e3e8-226">supportsOemConfig</span></span>|<span data-ttu-id="2e3e8-227">Логический</span><span class="sxs-lookup"><span data-stu-id="2e3e8-227">Boolean</span></span>|<span data-ttu-id="2e3e8-228">Поддерживает ли это приложение политику Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-228">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="2e3e8-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e3e8-229">Response</span></span>
<span data-ttu-id="2e3e8-230">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-230">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e3e8-231">Пример</span><span class="sxs-lookup"><span data-stu-id="2e3e8-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e3e8-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e3e8-232">Request</span></span>
<span data-ttu-id="2e3e8-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2e3e8-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e3e8-234">Response</span></span>
<span data-ttu-id="2e3e8-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e3e8-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




