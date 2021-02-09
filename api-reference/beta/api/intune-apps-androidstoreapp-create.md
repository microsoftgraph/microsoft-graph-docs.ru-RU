---
title: Создание объекта androidStoreApp
description: Создание объекта androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c5d03ffc0585572496f10aaffd4d6bdc41a570b9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157444"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="21675-103">Создание объекта androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="21675-103">Create androidStoreApp</span></span>

<span data-ttu-id="21675-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21675-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21675-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21675-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21675-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21675-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21675-107">Создание объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-107">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21675-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="21675-108">Prerequisites</span></span>
<span data-ttu-id="21675-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21675-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21675-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21675-111">Permission type</span></span>|<span data-ttu-id="21675-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21675-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21675-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21675-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21675-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21675-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="21675-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21675-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21675-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21675-116">Not supported.</span></span>|
|<span data-ttu-id="21675-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21675-117">Application</span></span>|<span data-ttu-id="21675-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21675-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21675-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21675-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="21675-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="21675-120">Request headers</span></span>
|<span data-ttu-id="21675-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21675-121">Header</span></span>|<span data-ttu-id="21675-122">Значение</span><span class="sxs-lookup"><span data-stu-id="21675-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21675-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21675-123">Authorization</span></span>|<span data-ttu-id="21675-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="21675-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21675-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21675-125">Accept</span></span>|<span data-ttu-id="21675-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21675-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21675-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="21675-127">Request body</span></span>
<span data-ttu-id="21675-128">В тексте запроса добавьте представление объекта androidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21675-128">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="21675-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="21675-129">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="21675-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="21675-130">Property</span></span>|<span data-ttu-id="21675-131">Тип</span><span class="sxs-lookup"><span data-stu-id="21675-131">Type</span></span>|<span data-ttu-id="21675-132">Описание</span><span class="sxs-lookup"><span data-stu-id="21675-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21675-133">id</span><span class="sxs-lookup"><span data-stu-id="21675-133">id</span></span>|<span data-ttu-id="21675-134">String</span><span class="sxs-lookup"><span data-stu-id="21675-134">String</span></span>|<span data-ttu-id="21675-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="21675-135">Key of the entity.</span></span> <span data-ttu-id="21675-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-137">displayName</span><span class="sxs-lookup"><span data-stu-id="21675-137">displayName</span></span>|<span data-ttu-id="21675-138">String</span><span class="sxs-lookup"><span data-stu-id="21675-138">String</span></span>|<span data-ttu-id="21675-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="21675-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="21675-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-141">description</span><span class="sxs-lookup"><span data-stu-id="21675-141">description</span></span>|<span data-ttu-id="21675-142">String</span><span class="sxs-lookup"><span data-stu-id="21675-142">String</span></span>|<span data-ttu-id="21675-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="21675-143">The description of the app.</span></span> <span data-ttu-id="21675-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-145">publisher</span><span class="sxs-lookup"><span data-stu-id="21675-145">publisher</span></span>|<span data-ttu-id="21675-146">String</span><span class="sxs-lookup"><span data-stu-id="21675-146">String</span></span>|<span data-ttu-id="21675-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="21675-147">The publisher of the app.</span></span> <span data-ttu-id="21675-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="21675-149">largeIcon</span></span>|[<span data-ttu-id="21675-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="21675-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="21675-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="21675-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="21675-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21675-153">createdDateTime</span></span>|<span data-ttu-id="21675-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21675-154">DateTimeOffset</span></span>|<span data-ttu-id="21675-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="21675-155">The date and time the app was created.</span></span> <span data-ttu-id="21675-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21675-157">lastModifiedDateTime</span></span>|<span data-ttu-id="21675-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21675-158">DateTimeOffset</span></span>|<span data-ttu-id="21675-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="21675-159">The date and time the app was last modified.</span></span> <span data-ttu-id="21675-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="21675-161">isFeatured</span></span>|<span data-ttu-id="21675-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="21675-162">Boolean</span></span>|<span data-ttu-id="21675-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="21675-164">privacyInformationUrl</span></span>|<span data-ttu-id="21675-165">String</span><span class="sxs-lookup"><span data-stu-id="21675-165">String</span></span>|<span data-ttu-id="21675-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="21675-166">The privacy statement Url.</span></span> <span data-ttu-id="21675-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="21675-168">informationUrl</span></span>|<span data-ttu-id="21675-169">String</span><span class="sxs-lookup"><span data-stu-id="21675-169">String</span></span>|<span data-ttu-id="21675-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="21675-170">The more information Url.</span></span> <span data-ttu-id="21675-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-172">owner</span><span class="sxs-lookup"><span data-stu-id="21675-172">owner</span></span>|<span data-ttu-id="21675-173">String</span><span class="sxs-lookup"><span data-stu-id="21675-173">String</span></span>|<span data-ttu-id="21675-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="21675-174">The owner of the app.</span></span> <span data-ttu-id="21675-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-176">developer</span><span class="sxs-lookup"><span data-stu-id="21675-176">developer</span></span>|<span data-ttu-id="21675-177">String</span><span class="sxs-lookup"><span data-stu-id="21675-177">String</span></span>|<span data-ttu-id="21675-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="21675-178">The developer of the app.</span></span> <span data-ttu-id="21675-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-180">notes</span><span class="sxs-lookup"><span data-stu-id="21675-180">notes</span></span>|<span data-ttu-id="21675-181">String</span><span class="sxs-lookup"><span data-stu-id="21675-181">String</span></span>|<span data-ttu-id="21675-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="21675-182">Notes for the app.</span></span> <span data-ttu-id="21675-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="21675-184">uploadState</span></span>|<span data-ttu-id="21675-185">Int32</span><span class="sxs-lookup"><span data-stu-id="21675-185">Int32</span></span>|<span data-ttu-id="21675-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="21675-186">The upload state.</span></span> <span data-ttu-id="21675-187">Возможные значения: 0- `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="21675-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="21675-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="21675-189">publishingState</span></span>|[<span data-ttu-id="21675-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="21675-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="21675-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="21675-191">The publishing state for the app.</span></span> <span data-ttu-id="21675-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="21675-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="21675-193">Наследуется от [mobileApp.](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="21675-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="21675-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="21675-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="21675-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="21675-195">isAssigned</span></span>|<span data-ttu-id="21675-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="21675-196">Boolean</span></span>|<span data-ttu-id="21675-197">Значение, указывающее, назначено ли приложению хотя бы одна группа.</span><span class="sxs-lookup"><span data-stu-id="21675-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="21675-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="21675-199">roleScopeTagIds</span></span>|<span data-ttu-id="21675-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="21675-200">String collection</span></span>|<span data-ttu-id="21675-201">Список ид тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="21675-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="21675-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="21675-203">dependentAppCount</span></span>|<span data-ttu-id="21675-204">Int32</span><span class="sxs-lookup"><span data-stu-id="21675-204">Int32</span></span>|<span data-ttu-id="21675-205">Общее количество зависимостей, которые есть у этого приложения.</span><span class="sxs-lookup"><span data-stu-id="21675-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="21675-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="21675-207">supersedingAppCount</span></span>|<span data-ttu-id="21675-208">Int32</span><span class="sxs-lookup"><span data-stu-id="21675-208">Int32</span></span>|<span data-ttu-id="21675-209">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="21675-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="21675-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="21675-211">supersededAppCount</span></span>|<span data-ttu-id="21675-212">Int32</span><span class="sxs-lookup"><span data-stu-id="21675-212">Int32</span></span>|<span data-ttu-id="21675-213">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="21675-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="21675-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="21675-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="21675-215">packageId</span><span class="sxs-lookup"><span data-stu-id="21675-215">packageId</span></span>|<span data-ttu-id="21675-216">String</span><span class="sxs-lookup"><span data-stu-id="21675-216">String</span></span>|<span data-ttu-id="21675-217">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="21675-217">The package identifier.</span></span>|
|<span data-ttu-id="21675-218">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="21675-218">appIdentifier</span></span>|<span data-ttu-id="21675-219">String</span><span class="sxs-lookup"><span data-stu-id="21675-219">String</span></span>|<span data-ttu-id="21675-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="21675-220">The Identity Name.</span></span>|
|<span data-ttu-id="21675-221">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="21675-221">appStoreUrl</span></span>|<span data-ttu-id="21675-222">String</span><span class="sxs-lookup"><span data-stu-id="21675-222">String</span></span>|<span data-ttu-id="21675-223">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="21675-223">The Android app store URL.</span></span>|
|<span data-ttu-id="21675-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="21675-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="21675-225">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="21675-225">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="21675-226">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="21675-226">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="21675-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="21675-227">Response</span></span>
<span data-ttu-id="21675-228">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="21675-228">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21675-229">Пример</span><span class="sxs-lookup"><span data-stu-id="21675-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="21675-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="21675-230">Request</span></span>
<span data-ttu-id="21675-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21675-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1327

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="21675-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="21675-232">Response</span></span>
<span data-ttu-id="21675-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21675-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1499

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```




