---
title: Создание Андроидфорворкапп
description: Создание нового объекта Андроидфорворкапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40745c2ad8177d5ce6caa417591e83aa23688a7e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49254133"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="8d5ca-103">Создание Андроидфорворкапп</span><span class="sxs-lookup"><span data-stu-id="8d5ca-103">Create androidForWorkApp</span></span>

<span data-ttu-id="8d5ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d5ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d5ca-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d5ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d5ca-107">Создание нового объекта [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8d5ca-107">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d5ca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d5ca-108">Prerequisites</span></span>
<span data-ttu-id="8d5ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d5ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d5ca-111">Permission type</span></span>|<span data-ttu-id="8d5ca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d5ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d5ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d5ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d5ca-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d5ca-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8d5ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d5ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d5ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-116">Not supported.</span></span>|
|<span data-ttu-id="8d5ca-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8d5ca-117">Application</span></span>|<span data-ttu-id="8d5ca-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d5ca-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d5ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d5ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8d5ca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8d5ca-120">Request headers</span></span>
|<span data-ttu-id="8d5ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d5ca-121">Header</span></span>|<span data-ttu-id="8d5ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8d5ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d5ca-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d5ca-123">Authorization</span></span>|<span data-ttu-id="8d5ca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d5ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d5ca-125">Accept</span></span>|<span data-ttu-id="8d5ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d5ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d5ca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d5ca-127">Request body</span></span>
<span data-ttu-id="8d5ca-128">В тексте запроса добавьте представление объекта Андроидфорворкапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-128">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="8d5ca-129">В следующей таблице приведены свойства, необходимые при создании Андроидфорворкапп.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-129">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="8d5ca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d5ca-130">Property</span></span>|<span data-ttu-id="8d5ca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8d5ca-131">Type</span></span>|<span data-ttu-id="8d5ca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8d5ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d5ca-133">id</span><span class="sxs-lookup"><span data-stu-id="8d5ca-133">id</span></span>|<span data-ttu-id="8d5ca-134">String</span><span class="sxs-lookup"><span data-stu-id="8d5ca-134">String</span></span>|<span data-ttu-id="8d5ca-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-135">Key of the entity.</span></span> <span data-ttu-id="8d5ca-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8d5ca-137">displayName</span></span>|<span data-ttu-id="8d5ca-138">String</span><span class="sxs-lookup"><span data-stu-id="8d5ca-138">String</span></span>|<span data-ttu-id="8d5ca-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8d5ca-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-141">description</span><span class="sxs-lookup"><span data-stu-id="8d5ca-141">description</span></span>|<span data-ttu-id="8d5ca-142">String</span><span class="sxs-lookup"><span data-stu-id="8d5ca-142">String</span></span>|<span data-ttu-id="8d5ca-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-143">The description of the app.</span></span> <span data-ttu-id="8d5ca-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8d5ca-145">publisher</span></span>|<span data-ttu-id="8d5ca-146">String</span><span class="sxs-lookup"><span data-stu-id="8d5ca-146">String</span></span>|<span data-ttu-id="8d5ca-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-147">The publisher of the app.</span></span> <span data-ttu-id="8d5ca-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8d5ca-149">largeIcon</span></span>|[<span data-ttu-id="8d5ca-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8d5ca-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8d5ca-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8d5ca-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d5ca-153">createdDateTime</span></span>|<span data-ttu-id="8d5ca-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d5ca-154">DateTimeOffset</span></span>|<span data-ttu-id="8d5ca-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-155">The date and time the app was created.</span></span> <span data-ttu-id="8d5ca-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d5ca-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8d5ca-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d5ca-158">DateTimeOffset</span></span>|<span data-ttu-id="8d5ca-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8d5ca-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8d5ca-161">isFeatured</span></span>|<span data-ttu-id="8d5ca-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d5ca-162">Boolean</span></span>|<span data-ttu-id="8d5ca-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8d5ca-164">privacyInformationUrl</span></span>|<span data-ttu-id="8d5ca-165">String</span><span class="sxs-lookup"><span data-stu-id="8d5ca-165">String</span></span>|<span data-ttu-id="8d5ca-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-166">The privacy statement Url.</span></span> <span data-ttu-id="8d5ca-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8d5ca-168">informationUrl</span></span>|<span data-ttu-id="8d5ca-169">String</span><span class="sxs-lookup"><span data-stu-id="8d5ca-169">String</span></span>|<span data-ttu-id="8d5ca-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-170">The more information Url.</span></span> <span data-ttu-id="8d5ca-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-172">owner</span><span class="sxs-lookup"><span data-stu-id="8d5ca-172">owner</span></span>|<span data-ttu-id="8d5ca-173">String</span><span class="sxs-lookup"><span data-stu-id="8d5ca-173">String</span></span>|<span data-ttu-id="8d5ca-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-174">The owner of the app.</span></span> <span data-ttu-id="8d5ca-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-176">developer</span><span class="sxs-lookup"><span data-stu-id="8d5ca-176">developer</span></span>|<span data-ttu-id="8d5ca-177">String</span><span class="sxs-lookup"><span data-stu-id="8d5ca-177">String</span></span>|<span data-ttu-id="8d5ca-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-178">The developer of the app.</span></span> <span data-ttu-id="8d5ca-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-180">notes</span><span class="sxs-lookup"><span data-stu-id="8d5ca-180">notes</span></span>|<span data-ttu-id="8d5ca-181">String</span><span class="sxs-lookup"><span data-stu-id="8d5ca-181">String</span></span>|<span data-ttu-id="8d5ca-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-182">Notes for the app.</span></span> <span data-ttu-id="8d5ca-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8d5ca-184">uploadState</span></span>|<span data-ttu-id="8d5ca-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8d5ca-185">Int32</span></span>|<span data-ttu-id="8d5ca-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-186">The upload state.</span></span> <span data-ttu-id="8d5ca-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="8d5ca-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="8d5ca-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="8d5ca-189">publishingState</span></span>|[<span data-ttu-id="8d5ca-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="8d5ca-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8d5ca-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-191">The publishing state for the app.</span></span> <span data-ttu-id="8d5ca-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8d5ca-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8d5ca-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8d5ca-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8d5ca-195">isAssigned</span></span>|<span data-ttu-id="8d5ca-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d5ca-196">Boolean</span></span>|<span data-ttu-id="8d5ca-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8d5ca-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8d5ca-199">roleScopeTagIds</span></span>|<span data-ttu-id="8d5ca-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8d5ca-200">String collection</span></span>|<span data-ttu-id="8d5ca-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8d5ca-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="8d5ca-203">dependentAppCount</span></span>|<span data-ttu-id="8d5ca-204">Int32</span><span class="sxs-lookup"><span data-stu-id="8d5ca-204">Int32</span></span>|<span data-ttu-id="8d5ca-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8d5ca-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="8d5ca-207">supersedingAppCount</span></span>|<span data-ttu-id="8d5ca-208">Int32</span><span class="sxs-lookup"><span data-stu-id="8d5ca-208">Int32</span></span>|<span data-ttu-id="8d5ca-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="8d5ca-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="8d5ca-211">supersededAppCount</span></span>|<span data-ttu-id="8d5ca-212">Int32</span><span class="sxs-lookup"><span data-stu-id="8d5ca-212">Int32</span></span>|<span data-ttu-id="8d5ca-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="8d5ca-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8d5ca-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8d5ca-215">packageId</span><span class="sxs-lookup"><span data-stu-id="8d5ca-215">packageId</span></span>|<span data-ttu-id="8d5ca-216">String</span><span class="sxs-lookup"><span data-stu-id="8d5ca-216">String</span></span>|<span data-ttu-id="8d5ca-217">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-217">The package identifier.</span></span>|
|<span data-ttu-id="8d5ca-218">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="8d5ca-218">appIdentifier</span></span>|<span data-ttu-id="8d5ca-219">String</span><span class="sxs-lookup"><span data-stu-id="8d5ca-219">String</span></span>|<span data-ttu-id="8d5ca-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-220">The Identity Name.</span></span>|
|<span data-ttu-id="8d5ca-221">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8d5ca-221">usedLicenseCount</span></span>|<span data-ttu-id="8d5ca-222">Int32</span><span class="sxs-lookup"><span data-stu-id="8d5ca-222">Int32</span></span>|<span data-ttu-id="8d5ca-223">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-223">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="8d5ca-224">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8d5ca-224">totalLicenseCount</span></span>|<span data-ttu-id="8d5ca-225">Int32</span><span class="sxs-lookup"><span data-stu-id="8d5ca-225">Int32</span></span>|<span data-ttu-id="8d5ca-226">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-226">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="8d5ca-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8d5ca-227">appStoreUrl</span></span>|<span data-ttu-id="8d5ca-228">String</span><span class="sxs-lookup"><span data-stu-id="8d5ca-228">String</span></span>|<span data-ttu-id="8d5ca-229">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-229">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="8d5ca-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d5ca-230">Response</span></span>
<span data-ttu-id="8d5ca-231">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидфорворкапп](../resources/intune-apps-androidforworkapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-231">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d5ca-232">Пример</span><span class="sxs-lookup"><span data-stu-id="8d5ca-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d5ca-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d5ca-233">Request</span></span>
<span data-ttu-id="8d5ca-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8d5ca-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d5ca-235">Response</span></span>
<span data-ttu-id="8d5ca-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d5ca-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




