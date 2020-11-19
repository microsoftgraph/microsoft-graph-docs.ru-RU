---
title: Создание Макосмикрософтеджеапп
description: Создание нового объекта Макосмикрософтеджеапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 95fabb65882a9838a5918b95af7e4ab6ec6d02af
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49251502"
---
# <a name="create-macosmicrosoftedgeapp"></a><span data-ttu-id="529f0-103">Создание Макосмикрософтеджеапп</span><span class="sxs-lookup"><span data-stu-id="529f0-103">Create macOSMicrosoftEdgeApp</span></span>

<span data-ttu-id="529f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="529f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="529f0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="529f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="529f0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="529f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="529f0-107">Создание нового объекта [макосмикрософтеджеапп](../resources/intune-apps-macosmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="529f0-107">Create a new [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="529f0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="529f0-108">Prerequisites</span></span>
<span data-ttu-id="529f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="529f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="529f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="529f0-111">Permission type</span></span>|<span data-ttu-id="529f0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="529f0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="529f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="529f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="529f0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="529f0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="529f0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="529f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="529f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="529f0-116">Not supported.</span></span>|
|<span data-ttu-id="529f0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="529f0-117">Application</span></span>|<span data-ttu-id="529f0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="529f0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="529f0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="529f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="529f0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="529f0-120">Request headers</span></span>
|<span data-ttu-id="529f0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="529f0-121">Header</span></span>|<span data-ttu-id="529f0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="529f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="529f0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="529f0-123">Authorization</span></span>|<span data-ttu-id="529f0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="529f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="529f0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="529f0-125">Accept</span></span>|<span data-ttu-id="529f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="529f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="529f0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="529f0-127">Request body</span></span>
<span data-ttu-id="529f0-128">В тексте запроса добавьте представление объекта Макосмикрософтеджеапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="529f0-128">In the request body, supply a JSON representation for the macOSMicrosoftEdgeApp object.</span></span>

<span data-ttu-id="529f0-129">В следующей таблице приведены свойства, необходимые при создании Макосмикрософтеджеапп.</span><span class="sxs-lookup"><span data-stu-id="529f0-129">The following table shows the properties that are required when you create the macOSMicrosoftEdgeApp.</span></span>

|<span data-ttu-id="529f0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="529f0-130">Property</span></span>|<span data-ttu-id="529f0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="529f0-131">Type</span></span>|<span data-ttu-id="529f0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="529f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="529f0-133">id</span><span class="sxs-lookup"><span data-stu-id="529f0-133">id</span></span>|<span data-ttu-id="529f0-134">String</span><span class="sxs-lookup"><span data-stu-id="529f0-134">String</span></span>|<span data-ttu-id="529f0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="529f0-135">Key of the entity.</span></span> <span data-ttu-id="529f0-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="529f0-137">displayName</span></span>|<span data-ttu-id="529f0-138">String</span><span class="sxs-lookup"><span data-stu-id="529f0-138">String</span></span>|<span data-ttu-id="529f0-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="529f0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="529f0-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-141">description</span><span class="sxs-lookup"><span data-stu-id="529f0-141">description</span></span>|<span data-ttu-id="529f0-142">String</span><span class="sxs-lookup"><span data-stu-id="529f0-142">String</span></span>|<span data-ttu-id="529f0-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="529f0-143">The description of the app.</span></span> <span data-ttu-id="529f0-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-145">publisher</span><span class="sxs-lookup"><span data-stu-id="529f0-145">publisher</span></span>|<span data-ttu-id="529f0-146">String</span><span class="sxs-lookup"><span data-stu-id="529f0-146">String</span></span>|<span data-ttu-id="529f0-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="529f0-147">The publisher of the app.</span></span> <span data-ttu-id="529f0-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="529f0-149">largeIcon</span></span>|[<span data-ttu-id="529f0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="529f0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="529f0-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="529f0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="529f0-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="529f0-153">createdDateTime</span></span>|<span data-ttu-id="529f0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="529f0-154">DateTimeOffset</span></span>|<span data-ttu-id="529f0-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="529f0-155">The date and time the app was created.</span></span> <span data-ttu-id="529f0-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="529f0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="529f0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="529f0-158">DateTimeOffset</span></span>|<span data-ttu-id="529f0-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="529f0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="529f0-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="529f0-161">isFeatured</span></span>|<span data-ttu-id="529f0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="529f0-162">Boolean</span></span>|<span data-ttu-id="529f0-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="529f0-164">privacyInformationUrl</span></span>|<span data-ttu-id="529f0-165">String</span><span class="sxs-lookup"><span data-stu-id="529f0-165">String</span></span>|<span data-ttu-id="529f0-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="529f0-166">The privacy statement Url.</span></span> <span data-ttu-id="529f0-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="529f0-168">informationUrl</span></span>|<span data-ttu-id="529f0-169">String</span><span class="sxs-lookup"><span data-stu-id="529f0-169">String</span></span>|<span data-ttu-id="529f0-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="529f0-170">The more information Url.</span></span> <span data-ttu-id="529f0-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-172">owner</span><span class="sxs-lookup"><span data-stu-id="529f0-172">owner</span></span>|<span data-ttu-id="529f0-173">String</span><span class="sxs-lookup"><span data-stu-id="529f0-173">String</span></span>|<span data-ttu-id="529f0-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="529f0-174">The owner of the app.</span></span> <span data-ttu-id="529f0-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-176">developer</span><span class="sxs-lookup"><span data-stu-id="529f0-176">developer</span></span>|<span data-ttu-id="529f0-177">String</span><span class="sxs-lookup"><span data-stu-id="529f0-177">String</span></span>|<span data-ttu-id="529f0-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="529f0-178">The developer of the app.</span></span> <span data-ttu-id="529f0-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-180">notes</span><span class="sxs-lookup"><span data-stu-id="529f0-180">notes</span></span>|<span data-ttu-id="529f0-181">String</span><span class="sxs-lookup"><span data-stu-id="529f0-181">String</span></span>|<span data-ttu-id="529f0-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="529f0-182">Notes for the app.</span></span> <span data-ttu-id="529f0-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="529f0-184">uploadState</span></span>|<span data-ttu-id="529f0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="529f0-185">Int32</span></span>|<span data-ttu-id="529f0-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="529f0-186">The upload state.</span></span> <span data-ttu-id="529f0-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="529f0-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="529f0-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="529f0-189">publishingState</span></span>|[<span data-ttu-id="529f0-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="529f0-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="529f0-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="529f0-191">The publishing state for the app.</span></span> <span data-ttu-id="529f0-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="529f0-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="529f0-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="529f0-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="529f0-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="529f0-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="529f0-195">isAssigned</span></span>|<span data-ttu-id="529f0-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="529f0-196">Boolean</span></span>|<span data-ttu-id="529f0-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="529f0-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="529f0-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="529f0-199">roleScopeTagIds</span></span>|<span data-ttu-id="529f0-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="529f0-200">String collection</span></span>|<span data-ttu-id="529f0-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="529f0-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="529f0-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="529f0-203">dependentAppCount</span></span>|<span data-ttu-id="529f0-204">Int32</span><span class="sxs-lookup"><span data-stu-id="529f0-204">Int32</span></span>|<span data-ttu-id="529f0-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="529f0-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="529f0-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="529f0-207">supersedingAppCount</span></span>|<span data-ttu-id="529f0-208">Int32</span><span class="sxs-lookup"><span data-stu-id="529f0-208">Int32</span></span>|<span data-ttu-id="529f0-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="529f0-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="529f0-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="529f0-211">supersededAppCount</span></span>|<span data-ttu-id="529f0-212">Int32</span><span class="sxs-lookup"><span data-stu-id="529f0-212">Int32</span></span>|<span data-ttu-id="529f0-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="529f0-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="529f0-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="529f0-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="529f0-215">оптоволокон</span><span class="sxs-lookup"><span data-stu-id="529f0-215">channel</span></span>|[<span data-ttu-id="529f0-216">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="529f0-216">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="529f0-217">Канал, который необходимо установить на целевые устройства.</span><span class="sxs-lookup"><span data-stu-id="529f0-217">The channel to install on target devices.</span></span> <span data-ttu-id="529f0-218">Возможные значения: `dev`, `beta`, `stable`.</span><span class="sxs-lookup"><span data-stu-id="529f0-218">Possible values are: `dev`, `beta`, `stable`.</span></span>|



## <a name="response"></a><span data-ttu-id="529f0-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="529f0-219">Response</span></span>
<span data-ttu-id="529f0-220">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосмикрософтеджеапп](../resources/intune-apps-macosmicrosoftedgeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="529f0-220">If successful, this method returns a `201 Created` response code and a [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="529f0-221">Пример</span><span class="sxs-lookup"><span data-stu-id="529f0-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="529f0-222">Запрос</span><span class="sxs-lookup"><span data-stu-id="529f0-222">Request</span></span>
<span data-ttu-id="529f0-223">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="529f0-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 799

{
  "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
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
  "channel": "beta"
}
```

### <a name="response"></a><span data-ttu-id="529f0-224">Отклик</span><span class="sxs-lookup"><span data-stu-id="529f0-224">Response</span></span>
<span data-ttu-id="529f0-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="529f0-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 971

{
  "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
  "id": "c964092a-092a-c964-2a09-64c92a0964c9",
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
  "channel": "beta"
}
```




