---
title: Создание windowsAppX
description: Создание нового объекта windowsAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9e727755634baa5b8e25fe91ece5bf833ab64793
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976664"
---
# <a name="create-windowsappx"></a><span data-ttu-id="ace94-103">Создание windowsAppX</span><span class="sxs-lookup"><span data-stu-id="ace94-103">Create windowsAppX</span></span>

<span data-ttu-id="ace94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ace94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ace94-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ace94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ace94-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ace94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ace94-107">Создание нового объекта [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="ace94-107">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ace94-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ace94-108">Prerequisites</span></span>
<span data-ttu-id="ace94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ace94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ace94-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ace94-111">Permission type</span></span>|<span data-ttu-id="ace94-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ace94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ace94-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ace94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ace94-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ace94-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ace94-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ace94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ace94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ace94-116">Not supported.</span></span>|
|<span data-ttu-id="ace94-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ace94-117">Application</span></span>|<span data-ttu-id="ace94-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ace94-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ace94-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ace94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ace94-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ace94-120">Request headers</span></span>
|<span data-ttu-id="ace94-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ace94-121">Header</span></span>|<span data-ttu-id="ace94-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ace94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ace94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ace94-123">Authorization</span></span>|<span data-ttu-id="ace94-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ace94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ace94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ace94-125">Accept</span></span>|<span data-ttu-id="ace94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ace94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ace94-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ace94-127">Request body</span></span>
<span data-ttu-id="ace94-128">В тексте запроса добавьте представление объекта windowsAppX в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ace94-128">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="ace94-129">В следующей таблице приведены свойства, необходимые при создании windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="ace94-129">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="ace94-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ace94-130">Property</span></span>|<span data-ttu-id="ace94-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ace94-131">Type</span></span>|<span data-ttu-id="ace94-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ace94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ace94-133">id</span><span class="sxs-lookup"><span data-stu-id="ace94-133">id</span></span>|<span data-ttu-id="ace94-134">String</span><span class="sxs-lookup"><span data-stu-id="ace94-134">String</span></span>|<span data-ttu-id="ace94-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ace94-135">Key of the entity.</span></span> <span data-ttu-id="ace94-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ace94-137">displayName</span></span>|<span data-ttu-id="ace94-138">String</span><span class="sxs-lookup"><span data-stu-id="ace94-138">String</span></span>|<span data-ttu-id="ace94-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ace94-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ace94-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-141">description</span><span class="sxs-lookup"><span data-stu-id="ace94-141">description</span></span>|<span data-ttu-id="ace94-142">String</span><span class="sxs-lookup"><span data-stu-id="ace94-142">String</span></span>|<span data-ttu-id="ace94-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ace94-143">The description of the app.</span></span> <span data-ttu-id="ace94-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ace94-145">publisher</span></span>|<span data-ttu-id="ace94-146">String</span><span class="sxs-lookup"><span data-stu-id="ace94-146">String</span></span>|<span data-ttu-id="ace94-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ace94-147">The publisher of the app.</span></span> <span data-ttu-id="ace94-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ace94-149">largeIcon</span></span>|[<span data-ttu-id="ace94-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ace94-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ace94-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ace94-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ace94-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ace94-153">createdDateTime</span></span>|<span data-ttu-id="ace94-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ace94-154">DateTimeOffset</span></span>|<span data-ttu-id="ace94-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ace94-155">The date and time the app was created.</span></span> <span data-ttu-id="ace94-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ace94-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ace94-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ace94-158">DateTimeOffset</span></span>|<span data-ttu-id="ace94-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ace94-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ace94-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ace94-161">isFeatured</span></span>|<span data-ttu-id="ace94-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ace94-162">Boolean</span></span>|<span data-ttu-id="ace94-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ace94-164">privacyInformationUrl</span></span>|<span data-ttu-id="ace94-165">String</span><span class="sxs-lookup"><span data-stu-id="ace94-165">String</span></span>|<span data-ttu-id="ace94-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ace94-166">The privacy statement Url.</span></span> <span data-ttu-id="ace94-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ace94-168">informationUrl</span></span>|<span data-ttu-id="ace94-169">String</span><span class="sxs-lookup"><span data-stu-id="ace94-169">String</span></span>|<span data-ttu-id="ace94-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ace94-170">The more information Url.</span></span> <span data-ttu-id="ace94-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-172">owner</span><span class="sxs-lookup"><span data-stu-id="ace94-172">owner</span></span>|<span data-ttu-id="ace94-173">String</span><span class="sxs-lookup"><span data-stu-id="ace94-173">String</span></span>|<span data-ttu-id="ace94-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ace94-174">The owner of the app.</span></span> <span data-ttu-id="ace94-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-176">developer</span><span class="sxs-lookup"><span data-stu-id="ace94-176">developer</span></span>|<span data-ttu-id="ace94-177">String</span><span class="sxs-lookup"><span data-stu-id="ace94-177">String</span></span>|<span data-ttu-id="ace94-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ace94-178">The developer of the app.</span></span> <span data-ttu-id="ace94-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-180">notes</span><span class="sxs-lookup"><span data-stu-id="ace94-180">notes</span></span>|<span data-ttu-id="ace94-181">String</span><span class="sxs-lookup"><span data-stu-id="ace94-181">String</span></span>|<span data-ttu-id="ace94-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ace94-182">Notes for the app.</span></span> <span data-ttu-id="ace94-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ace94-184">uploadState</span></span>|<span data-ttu-id="ace94-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ace94-185">Int32</span></span>|<span data-ttu-id="ace94-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="ace94-186">The upload state.</span></span> <span data-ttu-id="ace94-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="ace94-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ace94-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ace94-189">publishingState</span></span>|[<span data-ttu-id="ace94-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="ace94-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ace94-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ace94-191">The publishing state for the app.</span></span> <span data-ttu-id="ace94-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ace94-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ace94-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ace94-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ace94-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ace94-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ace94-195">isAssigned</span></span>|<span data-ttu-id="ace94-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ace94-196">Boolean</span></span>|<span data-ttu-id="ace94-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="ace94-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ace94-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ace94-199">roleScopeTagIds</span></span>|<span data-ttu-id="ace94-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ace94-200">String collection</span></span>|<span data-ttu-id="ace94-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ace94-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ace94-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="ace94-203">dependentAppCount</span></span>|<span data-ttu-id="ace94-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ace94-204">Int32</span></span>|<span data-ttu-id="ace94-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="ace94-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ace94-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="ace94-207">supersedingAppCount</span></span>|<span data-ttu-id="ace94-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ace94-208">Int32</span></span>|<span data-ttu-id="ace94-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="ace94-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="ace94-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="ace94-211">supersededAppCount</span></span>|<span data-ttu-id="ace94-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ace94-212">Int32</span></span>|<span data-ttu-id="ace94-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="ace94-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="ace94-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ace94-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ace94-215">committedContentVersion</span></span>|<span data-ttu-id="ace94-216">String</span><span class="sxs-lookup"><span data-stu-id="ace94-216">String</span></span>|<span data-ttu-id="ace94-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="ace94-217">The internal committed content version.</span></span> <span data-ttu-id="ace94-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ace94-219">fileName</span><span class="sxs-lookup"><span data-stu-id="ace94-219">fileName</span></span>|<span data-ttu-id="ace94-220">String</span><span class="sxs-lookup"><span data-stu-id="ace94-220">String</span></span>|<span data-ttu-id="ace94-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ace94-221">The name of the main Lob application file.</span></span> <span data-ttu-id="ace94-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ace94-223">size</span><span class="sxs-lookup"><span data-stu-id="ace94-223">size</span></span>|<span data-ttu-id="ace94-224">Int64</span><span class="sxs-lookup"><span data-stu-id="ace94-224">Int64</span></span>|<span data-ttu-id="ace94-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="ace94-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="ace94-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ace94-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ace94-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="ace94-227">applicableArchitectures</span></span>|[<span data-ttu-id="ace94-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="ace94-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="ace94-229">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ace94-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="ace94-230">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="ace94-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="ace94-231">identityName</span><span class="sxs-lookup"><span data-stu-id="ace94-231">identityName</span></span>|<span data-ttu-id="ace94-232">String</span><span class="sxs-lookup"><span data-stu-id="ace94-232">String</span></span>|<span data-ttu-id="ace94-233">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ace94-233">The Identity Name.</span></span>|
|<span data-ttu-id="ace94-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="ace94-234">identityPublisherHash</span></span>|<span data-ttu-id="ace94-235">String</span><span class="sxs-lookup"><span data-stu-id="ace94-235">String</span></span>|<span data-ttu-id="ace94-236">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ace94-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="ace94-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ace94-237">identityResourceIdentifier</span></span>|<span data-ttu-id="ace94-238">String</span><span class="sxs-lookup"><span data-stu-id="ace94-238">String</span></span>|<span data-ttu-id="ace94-239">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="ace94-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="ace94-240">isBundle</span><span class="sxs-lookup"><span data-stu-id="ace94-240">isBundle</span></span>|<span data-ttu-id="ace94-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="ace94-241">Boolean</span></span>|<span data-ttu-id="ace94-242">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="ace94-242">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="ace94-243">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ace94-243">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ace94-244">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ace94-244">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="ace94-245">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ace94-245">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ace94-246">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ace94-246">identityVersion</span></span>|<span data-ttu-id="ace94-247">String</span><span class="sxs-lookup"><span data-stu-id="ace94-247">String</span></span>|<span data-ttu-id="ace94-248">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ace94-248">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ace94-249">Ответ</span><span class="sxs-lookup"><span data-stu-id="ace94-249">Response</span></span>
<span data-ttu-id="ace94-250">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsAppX](../resources/intune-apps-windowsappx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ace94-250">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ace94-251">Пример</span><span class="sxs-lookup"><span data-stu-id="ace94-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="ace94-252">Запрос</span><span class="sxs-lookup"><span data-stu-id="ace94-252">Request</span></span>
<span data-ttu-id="ace94-253">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ace94-253">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1470

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="ace94-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="ace94-254">Response</span></span>
<span data-ttu-id="ace94-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ace94-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1642

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```






