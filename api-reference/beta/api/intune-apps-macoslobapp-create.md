---
title: Создание Макослобапп
description: Создание нового объекта Макослобапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc3ad5256ca281944d197b68cd29fd0d99c8c054
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986940"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="e0545-103">Создание Макослобапп</span><span class="sxs-lookup"><span data-stu-id="e0545-103">Create macOSLobApp</span></span>

<span data-ttu-id="e0545-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0545-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0545-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0545-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0545-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0545-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0545-107">Создание нового объекта [макослобапп](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e0545-107">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0545-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e0545-108">Prerequisites</span></span>
<span data-ttu-id="e0545-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0545-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0545-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0545-111">Permission type</span></span>|<span data-ttu-id="e0545-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0545-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0545-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0545-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0545-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0545-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0545-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0545-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0545-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0545-116">Not supported.</span></span>|
|<span data-ttu-id="e0545-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0545-117">Application</span></span>|<span data-ttu-id="e0545-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0545-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0545-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0545-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e0545-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e0545-120">Request headers</span></span>
|<span data-ttu-id="e0545-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0545-121">Header</span></span>|<span data-ttu-id="e0545-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e0545-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0545-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0545-123">Authorization</span></span>|<span data-ttu-id="e0545-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0545-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0545-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e0545-125">Accept</span></span>|<span data-ttu-id="e0545-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0545-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0545-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0545-127">Request body</span></span>
<span data-ttu-id="e0545-128">В тексте запроса добавьте представление объекта Макослобапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0545-128">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="e0545-129">В следующей таблице приведены свойства, необходимые при создании Макослобапп.</span><span class="sxs-lookup"><span data-stu-id="e0545-129">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="e0545-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0545-130">Property</span></span>|<span data-ttu-id="e0545-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e0545-131">Type</span></span>|<span data-ttu-id="e0545-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e0545-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0545-133">id</span><span class="sxs-lookup"><span data-stu-id="e0545-133">id</span></span>|<span data-ttu-id="e0545-134">String</span><span class="sxs-lookup"><span data-stu-id="e0545-134">String</span></span>|<span data-ttu-id="e0545-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e0545-135">Key of the entity.</span></span> <span data-ttu-id="e0545-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e0545-137">displayName</span></span>|<span data-ttu-id="e0545-138">String</span><span class="sxs-lookup"><span data-stu-id="e0545-138">String</span></span>|<span data-ttu-id="e0545-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e0545-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e0545-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-141">description</span><span class="sxs-lookup"><span data-stu-id="e0545-141">description</span></span>|<span data-ttu-id="e0545-142">String</span><span class="sxs-lookup"><span data-stu-id="e0545-142">String</span></span>|<span data-ttu-id="e0545-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e0545-143">The description of the app.</span></span> <span data-ttu-id="e0545-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e0545-145">publisher</span></span>|<span data-ttu-id="e0545-146">String</span><span class="sxs-lookup"><span data-stu-id="e0545-146">String</span></span>|<span data-ttu-id="e0545-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e0545-147">The publisher of the app.</span></span> <span data-ttu-id="e0545-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e0545-149">largeIcon</span></span>|[<span data-ttu-id="e0545-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e0545-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e0545-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e0545-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e0545-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0545-153">createdDateTime</span></span>|<span data-ttu-id="e0545-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0545-154">DateTimeOffset</span></span>|<span data-ttu-id="e0545-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e0545-155">The date and time the app was created.</span></span> <span data-ttu-id="e0545-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0545-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e0545-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0545-158">DateTimeOffset</span></span>|<span data-ttu-id="e0545-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e0545-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e0545-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e0545-161">isFeatured</span></span>|<span data-ttu-id="e0545-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0545-162">Boolean</span></span>|<span data-ttu-id="e0545-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e0545-164">privacyInformationUrl</span></span>|<span data-ttu-id="e0545-165">String</span><span class="sxs-lookup"><span data-stu-id="e0545-165">String</span></span>|<span data-ttu-id="e0545-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e0545-166">The privacy statement Url.</span></span> <span data-ttu-id="e0545-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e0545-168">informationUrl</span></span>|<span data-ttu-id="e0545-169">String</span><span class="sxs-lookup"><span data-stu-id="e0545-169">String</span></span>|<span data-ttu-id="e0545-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e0545-170">The more information Url.</span></span> <span data-ttu-id="e0545-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-172">owner</span><span class="sxs-lookup"><span data-stu-id="e0545-172">owner</span></span>|<span data-ttu-id="e0545-173">String</span><span class="sxs-lookup"><span data-stu-id="e0545-173">String</span></span>|<span data-ttu-id="e0545-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e0545-174">The owner of the app.</span></span> <span data-ttu-id="e0545-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-176">developer</span><span class="sxs-lookup"><span data-stu-id="e0545-176">developer</span></span>|<span data-ttu-id="e0545-177">String</span><span class="sxs-lookup"><span data-stu-id="e0545-177">String</span></span>|<span data-ttu-id="e0545-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e0545-178">The developer of the app.</span></span> <span data-ttu-id="e0545-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-180">notes</span><span class="sxs-lookup"><span data-stu-id="e0545-180">notes</span></span>|<span data-ttu-id="e0545-181">String</span><span class="sxs-lookup"><span data-stu-id="e0545-181">String</span></span>|<span data-ttu-id="e0545-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="e0545-182">Notes for the app.</span></span> <span data-ttu-id="e0545-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e0545-184">uploadState</span></span>|<span data-ttu-id="e0545-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e0545-185">Int32</span></span>|<span data-ttu-id="e0545-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="e0545-186">The upload state.</span></span> <span data-ttu-id="e0545-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="e0545-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="e0545-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="e0545-189">publishingState</span></span>|[<span data-ttu-id="e0545-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="e0545-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e0545-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="e0545-191">The publishing state for the app.</span></span> <span data-ttu-id="e0545-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e0545-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e0545-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e0545-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e0545-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e0545-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e0545-195">isAssigned</span></span>|<span data-ttu-id="e0545-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0545-196">Boolean</span></span>|<span data-ttu-id="e0545-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="e0545-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e0545-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e0545-199">roleScopeTagIds</span></span>|<span data-ttu-id="e0545-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e0545-200">String collection</span></span>|<span data-ttu-id="e0545-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e0545-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e0545-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="e0545-203">dependentAppCount</span></span>|<span data-ttu-id="e0545-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e0545-204">Int32</span></span>|<span data-ttu-id="e0545-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="e0545-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e0545-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="e0545-207">supersedingAppCount</span></span>|<span data-ttu-id="e0545-208">Int32</span><span class="sxs-lookup"><span data-stu-id="e0545-208">Int32</span></span>|<span data-ttu-id="e0545-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="e0545-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="e0545-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="e0545-211">supersededAppCount</span></span>|<span data-ttu-id="e0545-212">Int32</span><span class="sxs-lookup"><span data-stu-id="e0545-212">Int32</span></span>|<span data-ttu-id="e0545-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="e0545-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="e0545-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e0545-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e0545-215">committedContentVersion</span></span>|<span data-ttu-id="e0545-216">String</span><span class="sxs-lookup"><span data-stu-id="e0545-216">String</span></span>|<span data-ttu-id="e0545-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="e0545-217">The internal committed content version.</span></span> <span data-ttu-id="e0545-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e0545-219">fileName</span><span class="sxs-lookup"><span data-stu-id="e0545-219">fileName</span></span>|<span data-ttu-id="e0545-220">String</span><span class="sxs-lookup"><span data-stu-id="e0545-220">String</span></span>|<span data-ttu-id="e0545-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="e0545-221">The name of the main Lob application file.</span></span> <span data-ttu-id="e0545-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e0545-223">size</span><span class="sxs-lookup"><span data-stu-id="e0545-223">size</span></span>|<span data-ttu-id="e0545-224">Int64</span><span class="sxs-lookup"><span data-stu-id="e0545-224">Int64</span></span>|<span data-ttu-id="e0545-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="e0545-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="e0545-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e0545-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e0545-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="e0545-227">bundleId</span></span>|<span data-ttu-id="e0545-228">String</span><span class="sxs-lookup"><span data-stu-id="e0545-228">String</span></span>|<span data-ttu-id="e0545-229">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="e0545-229">The bundle id.</span></span>|
|<span data-ttu-id="e0545-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e0545-230">minimumSupportedOperatingSystem</span></span>|<span data-ttu-id="e0545-231">[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md);</span><span class="sxs-lookup"><span data-stu-id="e0545-231">[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md)</span></span>|<span data-ttu-id="e0545-232">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e0545-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e0545-233">buildNumber</span><span class="sxs-lookup"><span data-stu-id="e0545-233">buildNumber</span></span>|<span data-ttu-id="e0545-234">String</span><span class="sxs-lookup"><span data-stu-id="e0545-234">String</span></span>|<span data-ttu-id="e0545-235">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="e0545-235">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e0545-236">versionNumber</span><span class="sxs-lookup"><span data-stu-id="e0545-236">versionNumber</span></span>|<span data-ttu-id="e0545-237">String</span><span class="sxs-lookup"><span data-stu-id="e0545-237">String</span></span>|<span data-ttu-id="e0545-238">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="e0545-238">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e0545-239">чилдаппс</span><span class="sxs-lookup"><span data-stu-id="e0545-239">childApps</span></span>|<span data-ttu-id="e0545-240">Коллекция [макослобчилдапп](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="e0545-240">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="e0545-241">Список приложений в этом пакете набора</span><span class="sxs-lookup"><span data-stu-id="e0545-241">The app list in this bundle package</span></span>|
|<span data-ttu-id="e0545-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e0545-242">identityVersion</span></span>|<span data-ttu-id="e0545-243">String</span><span class="sxs-lookup"><span data-stu-id="e0545-243">String</span></span>|<span data-ttu-id="e0545-244">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e0545-244">The identity version.</span></span>|
|<span data-ttu-id="e0545-245">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="e0545-245">md5HashChunkSize</span></span>|<span data-ttu-id="e0545-246">Int32</span><span class="sxs-lookup"><span data-stu-id="e0545-246">Int32</span></span>|<span data-ttu-id="e0545-247">Размер фрагмента для хеша MD5</span><span class="sxs-lookup"><span data-stu-id="e0545-247">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="e0545-248">md5Hash</span><span class="sxs-lookup"><span data-stu-id="e0545-248">md5Hash</span></span>|<span data-ttu-id="e0545-249">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e0545-249">String collection</span></span>|<span data-ttu-id="e0545-250">Хэш-коды MD5</span><span class="sxs-lookup"><span data-stu-id="e0545-250">The MD5 hash codes</span></span>|
|<span data-ttu-id="e0545-251">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="e0545-251">ignoreVersionDetection</span></span>|<span data-ttu-id="e0545-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0545-252">Boolean</span></span>|<span data-ttu-id="e0545-253">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="e0545-253">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="e0545-254">Установите для этого параметра значение true для бизнес-приложений macOS (LoB), использующих функцию самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="e0545-254">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="e0545-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0545-255">Response</span></span>
<span data-ttu-id="e0545-256">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макослобапп](../resources/intune-apps-macoslobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0545-256">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0545-257">Пример</span><span class="sxs-lookup"><span data-stu-id="e0545-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0545-258">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0545-258">Request</span></span>
<span data-ttu-id="e0545-259">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0545-259">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1673

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="e0545-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0545-260">Response</span></span>
<span data-ttu-id="e0545-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0545-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1845

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```






