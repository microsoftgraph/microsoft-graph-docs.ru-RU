---
title: Создание Виндовсмикрософтеджеапп
description: Создание нового объекта Виндовсмикрософтеджеапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 524a89f2477ad0070f7836789a8cf1ab721417c1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247141"
---
# <a name="create-windowsmicrosoftedgeapp"></a><span data-ttu-id="8535e-103">Создание Виндовсмикрософтеджеапп</span><span class="sxs-lookup"><span data-stu-id="8535e-103">Create windowsMicrosoftEdgeApp</span></span>

<span data-ttu-id="8535e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8535e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8535e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8535e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8535e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8535e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8535e-107">Создание нового объекта [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8535e-107">Create a new [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8535e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8535e-108">Prerequisites</span></span>
<span data-ttu-id="8535e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8535e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8535e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8535e-111">Permission type</span></span>|<span data-ttu-id="8535e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8535e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8535e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8535e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8535e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8535e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8535e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8535e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8535e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8535e-116">Not supported.</span></span>|
|<span data-ttu-id="8535e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8535e-117">Application</span></span>|<span data-ttu-id="8535e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8535e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8535e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8535e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8535e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8535e-120">Request headers</span></span>
|<span data-ttu-id="8535e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8535e-121">Header</span></span>|<span data-ttu-id="8535e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8535e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8535e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8535e-123">Authorization</span></span>|<span data-ttu-id="8535e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8535e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8535e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8535e-125">Accept</span></span>|<span data-ttu-id="8535e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8535e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8535e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8535e-127">Request body</span></span>
<span data-ttu-id="8535e-128">В тексте запроса добавьте представление объекта Виндовсмикрософтеджеапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8535e-128">In the request body, supply a JSON representation for the windowsMicrosoftEdgeApp object.</span></span>

<span data-ttu-id="8535e-129">В следующей таблице приведены свойства, необходимые при создании Виндовсмикрософтеджеапп.</span><span class="sxs-lookup"><span data-stu-id="8535e-129">The following table shows the properties that are required when you create the windowsMicrosoftEdgeApp.</span></span>

|<span data-ttu-id="8535e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8535e-130">Property</span></span>|<span data-ttu-id="8535e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8535e-131">Type</span></span>|<span data-ttu-id="8535e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8535e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8535e-133">id</span><span class="sxs-lookup"><span data-stu-id="8535e-133">id</span></span>|<span data-ttu-id="8535e-134">String</span><span class="sxs-lookup"><span data-stu-id="8535e-134">String</span></span>|<span data-ttu-id="8535e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8535e-135">Key of the entity.</span></span> <span data-ttu-id="8535e-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8535e-137">displayName</span></span>|<span data-ttu-id="8535e-138">String</span><span class="sxs-lookup"><span data-stu-id="8535e-138">String</span></span>|<span data-ttu-id="8535e-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="8535e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8535e-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-141">description</span><span class="sxs-lookup"><span data-stu-id="8535e-141">description</span></span>|<span data-ttu-id="8535e-142">String</span><span class="sxs-lookup"><span data-stu-id="8535e-142">String</span></span>|<span data-ttu-id="8535e-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="8535e-143">The description of the app.</span></span> <span data-ttu-id="8535e-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8535e-145">publisher</span></span>|<span data-ttu-id="8535e-146">String</span><span class="sxs-lookup"><span data-stu-id="8535e-146">String</span></span>|<span data-ttu-id="8535e-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="8535e-147">The publisher of the app.</span></span> <span data-ttu-id="8535e-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8535e-149">largeIcon</span></span>|[<span data-ttu-id="8535e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8535e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8535e-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="8535e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8535e-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8535e-153">createdDateTime</span></span>|<span data-ttu-id="8535e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8535e-154">DateTimeOffset</span></span>|<span data-ttu-id="8535e-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="8535e-155">The date and time the app was created.</span></span> <span data-ttu-id="8535e-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8535e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8535e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8535e-158">DateTimeOffset</span></span>|<span data-ttu-id="8535e-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="8535e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8535e-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8535e-161">isFeatured</span></span>|<span data-ttu-id="8535e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8535e-162">Boolean</span></span>|<span data-ttu-id="8535e-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8535e-164">privacyInformationUrl</span></span>|<span data-ttu-id="8535e-165">String</span><span class="sxs-lookup"><span data-stu-id="8535e-165">String</span></span>|<span data-ttu-id="8535e-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8535e-166">The privacy statement Url.</span></span> <span data-ttu-id="8535e-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8535e-168">informationUrl</span></span>|<span data-ttu-id="8535e-169">String</span><span class="sxs-lookup"><span data-stu-id="8535e-169">String</span></span>|<span data-ttu-id="8535e-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="8535e-170">The more information Url.</span></span> <span data-ttu-id="8535e-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-172">owner</span><span class="sxs-lookup"><span data-stu-id="8535e-172">owner</span></span>|<span data-ttu-id="8535e-173">String</span><span class="sxs-lookup"><span data-stu-id="8535e-173">String</span></span>|<span data-ttu-id="8535e-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="8535e-174">The owner of the app.</span></span> <span data-ttu-id="8535e-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-176">developer</span><span class="sxs-lookup"><span data-stu-id="8535e-176">developer</span></span>|<span data-ttu-id="8535e-177">String</span><span class="sxs-lookup"><span data-stu-id="8535e-177">String</span></span>|<span data-ttu-id="8535e-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="8535e-178">The developer of the app.</span></span> <span data-ttu-id="8535e-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-180">notes</span><span class="sxs-lookup"><span data-stu-id="8535e-180">notes</span></span>|<span data-ttu-id="8535e-181">String</span><span class="sxs-lookup"><span data-stu-id="8535e-181">String</span></span>|<span data-ttu-id="8535e-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="8535e-182">Notes for the app.</span></span> <span data-ttu-id="8535e-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8535e-184">uploadState</span></span>|<span data-ttu-id="8535e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8535e-185">Int32</span></span>|<span data-ttu-id="8535e-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="8535e-186">The upload state.</span></span> <span data-ttu-id="8535e-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="8535e-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="8535e-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="8535e-189">publishingState</span></span>|[<span data-ttu-id="8535e-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="8535e-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8535e-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="8535e-191">The publishing state for the app.</span></span> <span data-ttu-id="8535e-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="8535e-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8535e-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8535e-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8535e-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8535e-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8535e-195">isAssigned</span></span>|<span data-ttu-id="8535e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="8535e-196">Boolean</span></span>|<span data-ttu-id="8535e-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="8535e-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8535e-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8535e-199">roleScopeTagIds</span></span>|<span data-ttu-id="8535e-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8535e-200">String collection</span></span>|<span data-ttu-id="8535e-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="8535e-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8535e-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="8535e-203">dependentAppCount</span></span>|<span data-ttu-id="8535e-204">Int32</span><span class="sxs-lookup"><span data-stu-id="8535e-204">Int32</span></span>|<span data-ttu-id="8535e-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="8535e-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8535e-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="8535e-207">supersedingAppCount</span></span>|<span data-ttu-id="8535e-208">Int32</span><span class="sxs-lookup"><span data-stu-id="8535e-208">Int32</span></span>|<span data-ttu-id="8535e-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="8535e-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="8535e-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="8535e-211">supersededAppCount</span></span>|<span data-ttu-id="8535e-212">Int32</span><span class="sxs-lookup"><span data-stu-id="8535e-212">Int32</span></span>|<span data-ttu-id="8535e-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="8535e-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="8535e-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8535e-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8535e-215">оптоволокон</span><span class="sxs-lookup"><span data-stu-id="8535e-215">channel</span></span>|[<span data-ttu-id="8535e-216">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="8535e-216">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="8535e-217">Канал, который необходимо установить на целевые устройства.</span><span class="sxs-lookup"><span data-stu-id="8535e-217">The channel to install on target devices.</span></span> <span data-ttu-id="8535e-218">Возможные значения: `dev`, `beta`, `stable`.</span><span class="sxs-lookup"><span data-stu-id="8535e-218">Possible values are: `dev`, `beta`, `stable`.</span></span>|
|<span data-ttu-id="8535e-219">дисплайлангуажелокале</span><span class="sxs-lookup"><span data-stu-id="8535e-219">displayLanguageLocale</span></span>|<span data-ttu-id="8535e-220">String</span><span class="sxs-lookup"><span data-stu-id="8535e-220">String</span></span>|<span data-ttu-id="8535e-221">Языковой стандарт, используемый при отображении текста для пользователя в пограничной приложении.</span><span class="sxs-lookup"><span data-stu-id="8535e-221">The language locale to use when the Edge app displays text to the user.</span></span>|



## <a name="response"></a><span data-ttu-id="8535e-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="8535e-222">Response</span></span>
<span data-ttu-id="8535e-223">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсмикрософтеджеапп](../resources/intune-apps-windowsmicrosoftedgeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8535e-223">If successful, this method returns a `201 Created` response code and a [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8535e-224">Пример</span><span class="sxs-lookup"><span data-stu-id="8535e-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="8535e-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="8535e-225">Request</span></span>
<span data-ttu-id="8535e-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8535e-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 862

{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
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
  "channel": "beta",
  "displayLanguageLocale": "Display Language Locale value"
}
```

### <a name="response"></a><span data-ttu-id="8535e-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="8535e-227">Response</span></span>
<span data-ttu-id="8535e-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8535e-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1034

{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
  "id": "a4d4a316-a316-a4d4-16a3-d4a416a3d4a4",
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
  "channel": "beta",
  "displayLanguageLocale": "Display Language Locale value"
}
```




