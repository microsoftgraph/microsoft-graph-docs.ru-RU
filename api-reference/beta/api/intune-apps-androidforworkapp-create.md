---
title: Создание Андроидфорворкапп
description: Создание нового объекта Андроидфорворкапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2fd15207306b07cb175bc1e8c97257a87be4b518
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012483"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="c575a-103">Создание Андроидфорворкапп</span><span class="sxs-lookup"><span data-stu-id="c575a-103">Create androidForWorkApp</span></span>

<span data-ttu-id="c575a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c575a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c575a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c575a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c575a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c575a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c575a-107">Создание нового объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="c575a-107">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c575a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c575a-108">Prerequisites</span></span>
<span data-ttu-id="c575a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c575a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c575a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c575a-111">Permission type</span></span>|<span data-ttu-id="c575a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c575a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c575a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c575a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c575a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c575a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c575a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c575a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c575a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c575a-116">Not supported.</span></span>|
|<span data-ttu-id="c575a-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c575a-117">Application</span></span>|<span data-ttu-id="c575a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c575a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c575a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c575a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c575a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c575a-120">Request headers</span></span>
|<span data-ttu-id="c575a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c575a-121">Header</span></span>|<span data-ttu-id="c575a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c575a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c575a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c575a-123">Authorization</span></span>|<span data-ttu-id="c575a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c575a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c575a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c575a-125">Accept</span></span>|<span data-ttu-id="c575a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c575a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c575a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c575a-127">Request body</span></span>
<span data-ttu-id="c575a-128">В тексте запроса добавьте представление объекта Андроидфорворкапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c575a-128">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="c575a-129">В следующей таблице приведены свойства, необходимые при создании Андроидфорворкапп.</span><span class="sxs-lookup"><span data-stu-id="c575a-129">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="c575a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c575a-130">Property</span></span>|<span data-ttu-id="c575a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c575a-131">Type</span></span>|<span data-ttu-id="c575a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c575a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c575a-133">id</span><span class="sxs-lookup"><span data-stu-id="c575a-133">id</span></span>|<span data-ttu-id="c575a-134">String</span><span class="sxs-lookup"><span data-stu-id="c575a-134">String</span></span>|<span data-ttu-id="c575a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c575a-135">Key of the entity.</span></span> <span data-ttu-id="c575a-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c575a-137">displayName</span></span>|<span data-ttu-id="c575a-138">String</span><span class="sxs-lookup"><span data-stu-id="c575a-138">String</span></span>|<span data-ttu-id="c575a-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c575a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c575a-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-141">description</span><span class="sxs-lookup"><span data-stu-id="c575a-141">description</span></span>|<span data-ttu-id="c575a-142">String</span><span class="sxs-lookup"><span data-stu-id="c575a-142">String</span></span>|<span data-ttu-id="c575a-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c575a-143">The description of the app.</span></span> <span data-ttu-id="c575a-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c575a-145">publisher</span></span>|<span data-ttu-id="c575a-146">String</span><span class="sxs-lookup"><span data-stu-id="c575a-146">String</span></span>|<span data-ttu-id="c575a-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c575a-147">The publisher of the app.</span></span> <span data-ttu-id="c575a-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c575a-149">largeIcon</span></span>|[<span data-ttu-id="c575a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c575a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c575a-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="c575a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c575a-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c575a-153">createdDateTime</span></span>|<span data-ttu-id="c575a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c575a-154">DateTimeOffset</span></span>|<span data-ttu-id="c575a-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="c575a-155">The date and time the app was created.</span></span> <span data-ttu-id="c575a-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c575a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c575a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c575a-158">DateTimeOffset</span></span>|<span data-ttu-id="c575a-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="c575a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c575a-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c575a-161">isFeatured</span></span>|<span data-ttu-id="c575a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c575a-162">Boolean</span></span>|<span data-ttu-id="c575a-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c575a-164">privacyInformationUrl</span></span>|<span data-ttu-id="c575a-165">String</span><span class="sxs-lookup"><span data-stu-id="c575a-165">String</span></span>|<span data-ttu-id="c575a-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c575a-166">The privacy statement Url.</span></span> <span data-ttu-id="c575a-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c575a-168">informationUrl</span></span>|<span data-ttu-id="c575a-169">String</span><span class="sxs-lookup"><span data-stu-id="c575a-169">String</span></span>|<span data-ttu-id="c575a-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="c575a-170">The more information Url.</span></span> <span data-ttu-id="c575a-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-172">owner</span><span class="sxs-lookup"><span data-stu-id="c575a-172">owner</span></span>|<span data-ttu-id="c575a-173">String</span><span class="sxs-lookup"><span data-stu-id="c575a-173">String</span></span>|<span data-ttu-id="c575a-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="c575a-174">The owner of the app.</span></span> <span data-ttu-id="c575a-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-176">developer</span><span class="sxs-lookup"><span data-stu-id="c575a-176">developer</span></span>|<span data-ttu-id="c575a-177">String</span><span class="sxs-lookup"><span data-stu-id="c575a-177">String</span></span>|<span data-ttu-id="c575a-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="c575a-178">The developer of the app.</span></span> <span data-ttu-id="c575a-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-180">notes</span><span class="sxs-lookup"><span data-stu-id="c575a-180">notes</span></span>|<span data-ttu-id="c575a-181">String</span><span class="sxs-lookup"><span data-stu-id="c575a-181">String</span></span>|<span data-ttu-id="c575a-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="c575a-182">Notes for the app.</span></span> <span data-ttu-id="c575a-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c575a-184">uploadState</span></span>|<span data-ttu-id="c575a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c575a-185">Int32</span></span>|<span data-ttu-id="c575a-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="c575a-186">The upload state.</span></span> <span data-ttu-id="c575a-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="c575a-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="c575a-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="c575a-189">publishingState</span></span>|[<span data-ttu-id="c575a-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="c575a-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c575a-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="c575a-191">The publishing state for the app.</span></span> <span data-ttu-id="c575a-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="c575a-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c575a-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="c575a-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c575a-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c575a-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c575a-195">isAssigned</span></span>|<span data-ttu-id="c575a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="c575a-196">Boolean</span></span>|<span data-ttu-id="c575a-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="c575a-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c575a-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c575a-199">roleScopeTagIds</span></span>|<span data-ttu-id="c575a-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c575a-200">String collection</span></span>|<span data-ttu-id="c575a-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="c575a-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c575a-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="c575a-203">dependentAppCount</span></span>|<span data-ttu-id="c575a-204">Int32</span><span class="sxs-lookup"><span data-stu-id="c575a-204">Int32</span></span>|<span data-ttu-id="c575a-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="c575a-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="c575a-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="c575a-207">supersedingAppCount</span></span>|<span data-ttu-id="c575a-208">Int32</span><span class="sxs-lookup"><span data-stu-id="c575a-208">Int32</span></span>|<span data-ttu-id="c575a-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="c575a-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="c575a-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="c575a-211">supersededAppCount</span></span>|<span data-ttu-id="c575a-212">Int32</span><span class="sxs-lookup"><span data-stu-id="c575a-212">Int32</span></span>|<span data-ttu-id="c575a-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="c575a-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="c575a-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c575a-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c575a-215">packageId</span><span class="sxs-lookup"><span data-stu-id="c575a-215">packageId</span></span>|<span data-ttu-id="c575a-216">String</span><span class="sxs-lookup"><span data-stu-id="c575a-216">String</span></span>|<span data-ttu-id="c575a-217">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="c575a-217">The package identifier.</span></span>|
|<span data-ttu-id="c575a-218">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c575a-218">appIdentifier</span></span>|<span data-ttu-id="c575a-219">String</span><span class="sxs-lookup"><span data-stu-id="c575a-219">String</span></span>|<span data-ttu-id="c575a-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c575a-220">The Identity Name.</span></span>|
|<span data-ttu-id="c575a-221">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c575a-221">usedLicenseCount</span></span>|<span data-ttu-id="c575a-222">Int32</span><span class="sxs-lookup"><span data-stu-id="c575a-222">Int32</span></span>|<span data-ttu-id="c575a-223">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="c575a-223">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="c575a-224">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="c575a-224">totalLicenseCount</span></span>|<span data-ttu-id="c575a-225">Int32</span><span class="sxs-lookup"><span data-stu-id="c575a-225">Int32</span></span>|<span data-ttu-id="c575a-226">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="c575a-226">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="c575a-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c575a-227">appStoreUrl</span></span>|<span data-ttu-id="c575a-228">String</span><span class="sxs-lookup"><span data-stu-id="c575a-228">String</span></span>|<span data-ttu-id="c575a-229">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="c575a-229">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="c575a-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="c575a-230">Response</span></span>
<span data-ttu-id="c575a-231">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c575a-231">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c575a-232">Пример</span><span class="sxs-lookup"><span data-stu-id="c575a-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="c575a-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="c575a-233">Request</span></span>
<span data-ttu-id="c575a-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c575a-234">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 960

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="c575a-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="c575a-235">Response</span></span>
<span data-ttu-id="c575a-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c575a-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1132

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```






