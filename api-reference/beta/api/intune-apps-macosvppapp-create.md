---
title: Создание Макосвппапп
description: Создание нового объекта Макосвппапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6258c478acf1a8c8f35a65969b6fd0f296670d34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012021"
---
# <a name="create-macosvppapp"></a><span data-ttu-id="3a9f0-103">Создание Макосвппапп</span><span class="sxs-lookup"><span data-stu-id="3a9f0-103">Create macOsVppApp</span></span>

<span data-ttu-id="3a9f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a9f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a9f0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a9f0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a9f0-107">Создание нового объекта [макосвппапп](../resources/intune-apps-macosvppapp.md) .</span><span class="sxs-lookup"><span data-stu-id="3a9f0-107">Create a new [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a9f0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a9f0-108">Prerequisites</span></span>
<span data-ttu-id="3a9f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a9f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a9f0-111">Permission type</span></span>|<span data-ttu-id="3a9f0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a9f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a9f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a9f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a9f0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9f0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3a9f0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a9f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a9f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-116">Not supported.</span></span>|
|<span data-ttu-id="3a9f0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3a9f0-117">Application</span></span>|<span data-ttu-id="3a9f0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a9f0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a9f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a9f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3a9f0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3a9f0-120">Request headers</span></span>
|<span data-ttu-id="3a9f0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a9f0-121">Header</span></span>|<span data-ttu-id="3a9f0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a9f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a9f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a9f0-123">Authorization</span></span>|<span data-ttu-id="3a9f0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a9f0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a9f0-125">Accept</span></span>|<span data-ttu-id="3a9f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a9f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a9f0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a9f0-127">Request body</span></span>
<span data-ttu-id="3a9f0-128">В тексте запроса добавьте представление объекта Макосвппапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-128">In the request body, supply a JSON representation for the macOsVppApp object.</span></span>

<span data-ttu-id="3a9f0-129">В следующей таблице приведены свойства, необходимые при создании Макосвппапп.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-129">The following table shows the properties that are required when you create the macOsVppApp.</span></span>

|<span data-ttu-id="3a9f0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a9f0-130">Property</span></span>|<span data-ttu-id="3a9f0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3a9f0-131">Type</span></span>|<span data-ttu-id="3a9f0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3a9f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a9f0-133">id</span><span class="sxs-lookup"><span data-stu-id="3a9f0-133">id</span></span>|<span data-ttu-id="3a9f0-134">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-134">String</span></span>|<span data-ttu-id="3a9f0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-135">Key of the entity.</span></span> <span data-ttu-id="3a9f0-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3a9f0-137">displayName</span></span>|<span data-ttu-id="3a9f0-138">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-138">String</span></span>|<span data-ttu-id="3a9f0-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3a9f0-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-141">description</span><span class="sxs-lookup"><span data-stu-id="3a9f0-141">description</span></span>|<span data-ttu-id="3a9f0-142">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-142">String</span></span>|<span data-ttu-id="3a9f0-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-143">The description of the app.</span></span> <span data-ttu-id="3a9f0-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3a9f0-145">publisher</span></span>|<span data-ttu-id="3a9f0-146">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-146">String</span></span>|<span data-ttu-id="3a9f0-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-147">The publisher of the app.</span></span> <span data-ttu-id="3a9f0-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3a9f0-149">largeIcon</span></span>|[<span data-ttu-id="3a9f0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3a9f0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3a9f0-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3a9f0-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a9f0-153">createdDateTime</span></span>|<span data-ttu-id="3a9f0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a9f0-154">DateTimeOffset</span></span>|<span data-ttu-id="3a9f0-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-155">The date and time the app was created.</span></span> <span data-ttu-id="3a9f0-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a9f0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3a9f0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a9f0-158">DateTimeOffset</span></span>|<span data-ttu-id="3a9f0-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="3a9f0-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3a9f0-161">isFeatured</span></span>|<span data-ttu-id="3a9f0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a9f0-162">Boolean</span></span>|<span data-ttu-id="3a9f0-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3a9f0-164">privacyInformationUrl</span></span>|<span data-ttu-id="3a9f0-165">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-165">String</span></span>|<span data-ttu-id="3a9f0-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-166">The privacy statement Url.</span></span> <span data-ttu-id="3a9f0-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3a9f0-168">informationUrl</span></span>|<span data-ttu-id="3a9f0-169">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-169">String</span></span>|<span data-ttu-id="3a9f0-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-170">The more information Url.</span></span> <span data-ttu-id="3a9f0-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-172">owner</span><span class="sxs-lookup"><span data-stu-id="3a9f0-172">owner</span></span>|<span data-ttu-id="3a9f0-173">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-173">String</span></span>|<span data-ttu-id="3a9f0-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-174">The owner of the app.</span></span> <span data-ttu-id="3a9f0-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-176">developer</span><span class="sxs-lookup"><span data-stu-id="3a9f0-176">developer</span></span>|<span data-ttu-id="3a9f0-177">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-177">String</span></span>|<span data-ttu-id="3a9f0-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-178">The developer of the app.</span></span> <span data-ttu-id="3a9f0-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-180">notes</span><span class="sxs-lookup"><span data-stu-id="3a9f0-180">notes</span></span>|<span data-ttu-id="3a9f0-181">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-181">String</span></span>|<span data-ttu-id="3a9f0-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-182">Notes for the app.</span></span> <span data-ttu-id="3a9f0-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="3a9f0-184">uploadState</span></span>|<span data-ttu-id="3a9f0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3a9f0-185">Int32</span></span>|<span data-ttu-id="3a9f0-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-186">The upload state.</span></span> <span data-ttu-id="3a9f0-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="3a9f0-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="3a9f0-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="3a9f0-189">publishingState</span></span>|[<span data-ttu-id="3a9f0-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="3a9f0-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3a9f0-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-191">The publishing state for the app.</span></span> <span data-ttu-id="3a9f0-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3a9f0-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="3a9f0-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3a9f0-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3a9f0-195">isAssigned</span></span>|<span data-ttu-id="3a9f0-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a9f0-196">Boolean</span></span>|<span data-ttu-id="3a9f0-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3a9f0-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a9f0-199">roleScopeTagIds</span></span>|<span data-ttu-id="3a9f0-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-200">String collection</span></span>|<span data-ttu-id="3a9f0-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3a9f0-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="3a9f0-203">dependentAppCount</span></span>|<span data-ttu-id="3a9f0-204">Int32</span><span class="sxs-lookup"><span data-stu-id="3a9f0-204">Int32</span></span>|<span data-ttu-id="3a9f0-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="3a9f0-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="3a9f0-207">supersedingAppCount</span></span>|<span data-ttu-id="3a9f0-208">Int32</span><span class="sxs-lookup"><span data-stu-id="3a9f0-208">Int32</span></span>|<span data-ttu-id="3a9f0-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="3a9f0-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="3a9f0-211">supersededAppCount</span></span>|<span data-ttu-id="3a9f0-212">Int32</span><span class="sxs-lookup"><span data-stu-id="3a9f0-212">Int32</span></span>|<span data-ttu-id="3a9f0-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="3a9f0-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3a9f0-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3a9f0-215">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3a9f0-215">usedLicenseCount</span></span>|<span data-ttu-id="3a9f0-216">Int32</span><span class="sxs-lookup"><span data-stu-id="3a9f0-216">Int32</span></span>|<span data-ttu-id="3a9f0-217">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-217">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="3a9f0-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3a9f0-218">totalLicenseCount</span></span>|<span data-ttu-id="3a9f0-219">Int32</span><span class="sxs-lookup"><span data-stu-id="3a9f0-219">Int32</span></span>|<span data-ttu-id="3a9f0-220">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-220">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="3a9f0-221">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="3a9f0-221">releaseDateTime</span></span>|<span data-ttu-id="3a9f0-222">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a9f0-222">DateTimeOffset</span></span>|<span data-ttu-id="3a9f0-223">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-223">The VPP application release date and time.</span></span>|
|<span data-ttu-id="3a9f0-224">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3a9f0-224">appStoreUrl</span></span>|<span data-ttu-id="3a9f0-225">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-225">String</span></span>|<span data-ttu-id="3a9f0-226">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-226">The store URL.</span></span>|
|<span data-ttu-id="3a9f0-227">licensingType</span><span class="sxs-lookup"><span data-stu-id="3a9f0-227">licensingType</span></span>|[<span data-ttu-id="3a9f0-228">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="3a9f0-228">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="3a9f0-229">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-229">The supported License Type.</span></span>|
|<span data-ttu-id="3a9f0-230">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="3a9f0-230">vppTokenOrganizationName</span></span>|<span data-ttu-id="3a9f0-231">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-231">String</span></span>|<span data-ttu-id="3a9f0-232">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-232">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="3a9f0-233">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="3a9f0-233">vppTokenAccountType</span></span>|[<span data-ttu-id="3a9f0-234">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="3a9f0-234">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="3a9f0-235">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-235">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="3a9f0-236">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-236">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="3a9f0-237">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-237">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="3a9f0-238">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="3a9f0-238">vppTokenAppleId</span></span>|<span data-ttu-id="3a9f0-239">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-239">String</span></span>|<span data-ttu-id="3a9f0-240">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-240">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3a9f0-241">bundleId</span><span class="sxs-lookup"><span data-stu-id="3a9f0-241">bundleId</span></span>|<span data-ttu-id="3a9f0-242">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-242">String</span></span>|<span data-ttu-id="3a9f0-243">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-243">The Identity Name.</span></span>|
|<span data-ttu-id="3a9f0-244">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="3a9f0-244">vppTokenId</span></span>|<span data-ttu-id="3a9f0-245">String</span><span class="sxs-lookup"><span data-stu-id="3a9f0-245">String</span></span>|<span data-ttu-id="3a9f0-246">Идентификатор токена VPP, связанного с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-246">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="3a9f0-247">ревокелиценсеактионресултс</span><span class="sxs-lookup"><span data-stu-id="3a9f0-247">revokeLicenseActionResults</span></span>|<span data-ttu-id="3a9f0-248">Коллекция [макосвппаппревокелиценсесактионресулт](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3a9f0-248">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="3a9f0-249">Результаты отзыва действий лицензии в этом приложении.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-249">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="3a9f0-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a9f0-250">Response</span></span>
<span data-ttu-id="3a9f0-251">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвппапп](../resources/intune-apps-macosvppapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-251">If successful, this method returns a `201 Created` response code and a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a9f0-252">Пример</span><span class="sxs-lookup"><span data-stu-id="3a9f0-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a9f0-253">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a9f0-253">Request</span></span>
<span data-ttu-id="3a9f0-254">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-254">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1926

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3a9f0-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a9f0-255">Response</span></span>
<span data-ttu-id="3a9f0-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a9f0-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2098

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
  "id": "10b95265-5265-10b9-6552-b9106552b910",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```






