---
title: Создание win32LobApp
description: Создание нового объекта win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ffcb993889ff84bb2d2d388a7e7eebd2d9f493df
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247435"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="9f644-103">Создание win32LobApp</span><span class="sxs-lookup"><span data-stu-id="9f644-103">Create win32LobApp</span></span>

<span data-ttu-id="9f644-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f644-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f644-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f644-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f644-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f644-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f644-107">Создание нового объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9f644-107">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f644-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f644-108">Prerequisites</span></span>
<span data-ttu-id="9f644-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f644-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f644-111">Permission type</span></span>|<span data-ttu-id="9f644-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f644-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f644-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f644-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f644-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f644-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9f644-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f644-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f644-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f644-116">Not supported.</span></span>|
|<span data-ttu-id="9f644-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f644-117">Application</span></span>|<span data-ttu-id="9f644-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f644-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f644-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f644-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9f644-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f644-120">Request headers</span></span>
|<span data-ttu-id="9f644-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f644-121">Header</span></span>|<span data-ttu-id="9f644-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9f644-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f644-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f644-123">Authorization</span></span>|<span data-ttu-id="9f644-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f644-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f644-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f644-125">Accept</span></span>|<span data-ttu-id="9f644-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f644-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f644-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f644-127">Request body</span></span>
<span data-ttu-id="9f644-128">В тексте запроса добавьте представление объекта win32LobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f644-128">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="9f644-129">В следующей таблице приведены свойства, необходимые при создании win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="9f644-129">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="9f644-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f644-130">Property</span></span>|<span data-ttu-id="9f644-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f644-131">Type</span></span>|<span data-ttu-id="9f644-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f644-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f644-133">id</span><span class="sxs-lookup"><span data-stu-id="9f644-133">id</span></span>|<span data-ttu-id="9f644-134">String</span><span class="sxs-lookup"><span data-stu-id="9f644-134">String</span></span>|<span data-ttu-id="9f644-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9f644-135">Key of the entity.</span></span> <span data-ttu-id="9f644-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9f644-137">displayName</span></span>|<span data-ttu-id="9f644-138">String</span><span class="sxs-lookup"><span data-stu-id="9f644-138">String</span></span>|<span data-ttu-id="9f644-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9f644-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9f644-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-141">description</span><span class="sxs-lookup"><span data-stu-id="9f644-141">description</span></span>|<span data-ttu-id="9f644-142">String</span><span class="sxs-lookup"><span data-stu-id="9f644-142">String</span></span>|<span data-ttu-id="9f644-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-143">The description of the app.</span></span> <span data-ttu-id="9f644-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-145">publisher</span><span class="sxs-lookup"><span data-stu-id="9f644-145">publisher</span></span>|<span data-ttu-id="9f644-146">String</span><span class="sxs-lookup"><span data-stu-id="9f644-146">String</span></span>|<span data-ttu-id="9f644-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-147">The publisher of the app.</span></span> <span data-ttu-id="9f644-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9f644-149">largeIcon</span></span>|[<span data-ttu-id="9f644-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9f644-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9f644-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9f644-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9f644-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f644-153">createdDateTime</span></span>|<span data-ttu-id="9f644-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f644-154">DateTimeOffset</span></span>|<span data-ttu-id="9f644-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-155">The date and time the app was created.</span></span> <span data-ttu-id="9f644-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f644-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9f644-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f644-158">DateTimeOffset</span></span>|<span data-ttu-id="9f644-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9f644-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9f644-161">isFeatured</span></span>|<span data-ttu-id="9f644-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f644-162">Boolean</span></span>|<span data-ttu-id="9f644-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9f644-164">privacyInformationUrl</span></span>|<span data-ttu-id="9f644-165">String</span><span class="sxs-lookup"><span data-stu-id="9f644-165">String</span></span>|<span data-ttu-id="9f644-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9f644-166">The privacy statement Url.</span></span> <span data-ttu-id="9f644-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9f644-168">informationUrl</span></span>|<span data-ttu-id="9f644-169">String</span><span class="sxs-lookup"><span data-stu-id="9f644-169">String</span></span>|<span data-ttu-id="9f644-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9f644-170">The more information Url.</span></span> <span data-ttu-id="9f644-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-172">owner</span><span class="sxs-lookup"><span data-stu-id="9f644-172">owner</span></span>|<span data-ttu-id="9f644-173">String</span><span class="sxs-lookup"><span data-stu-id="9f644-173">String</span></span>|<span data-ttu-id="9f644-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-174">The owner of the app.</span></span> <span data-ttu-id="9f644-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-176">developer</span><span class="sxs-lookup"><span data-stu-id="9f644-176">developer</span></span>|<span data-ttu-id="9f644-177">String</span><span class="sxs-lookup"><span data-stu-id="9f644-177">String</span></span>|<span data-ttu-id="9f644-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-178">The developer of the app.</span></span> <span data-ttu-id="9f644-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-180">notes</span><span class="sxs-lookup"><span data-stu-id="9f644-180">notes</span></span>|<span data-ttu-id="9f644-181">String</span><span class="sxs-lookup"><span data-stu-id="9f644-181">String</span></span>|<span data-ttu-id="9f644-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-182">Notes for the app.</span></span> <span data-ttu-id="9f644-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9f644-184">uploadState</span></span>|<span data-ttu-id="9f644-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9f644-185">Int32</span></span>|<span data-ttu-id="9f644-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="9f644-186">The upload state.</span></span> <span data-ttu-id="9f644-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="9f644-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="9f644-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="9f644-189">publishingState</span></span>|[<span data-ttu-id="9f644-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9f644-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9f644-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-191">The publishing state for the app.</span></span> <span data-ttu-id="9f644-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9f644-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9f644-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="9f644-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9f644-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9f644-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9f644-195">isAssigned</span></span>|<span data-ttu-id="9f644-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f644-196">Boolean</span></span>|<span data-ttu-id="9f644-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="9f644-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9f644-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f644-199">roleScopeTagIds</span></span>|<span data-ttu-id="9f644-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9f644-200">String collection</span></span>|<span data-ttu-id="9f644-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9f644-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="9f644-203">dependentAppCount</span></span>|<span data-ttu-id="9f644-204">Int32</span><span class="sxs-lookup"><span data-stu-id="9f644-204">Int32</span></span>|<span data-ttu-id="9f644-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9f644-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="9f644-207">supersedingAppCount</span></span>|<span data-ttu-id="9f644-208">Int32</span><span class="sxs-lookup"><span data-stu-id="9f644-208">Int32</span></span>|<span data-ttu-id="9f644-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="9f644-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="9f644-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="9f644-211">supersededAppCount</span></span>|<span data-ttu-id="9f644-212">Int32</span><span class="sxs-lookup"><span data-stu-id="9f644-212">Int32</span></span>|<span data-ttu-id="9f644-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="9f644-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="9f644-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f644-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9f644-215">committedContentVersion</span></span>|<span data-ttu-id="9f644-216">String</span><span class="sxs-lookup"><span data-stu-id="9f644-216">String</span></span>|<span data-ttu-id="9f644-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="9f644-217">The internal committed content version.</span></span> <span data-ttu-id="9f644-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9f644-219">fileName</span><span class="sxs-lookup"><span data-stu-id="9f644-219">fileName</span></span>|<span data-ttu-id="9f644-220">String</span><span class="sxs-lookup"><span data-stu-id="9f644-220">String</span></span>|<span data-ttu-id="9f644-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-221">The name of the main Lob application file.</span></span> <span data-ttu-id="9f644-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9f644-223">size</span><span class="sxs-lookup"><span data-stu-id="9f644-223">size</span></span>|<span data-ttu-id="9f644-224">Int64</span><span class="sxs-lookup"><span data-stu-id="9f644-224">Int64</span></span>|<span data-ttu-id="9f644-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="9f644-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="9f644-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f644-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9f644-227">инсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="9f644-227">installCommandLine</span></span>|<span data-ttu-id="9f644-228">String</span><span class="sxs-lookup"><span data-stu-id="9f644-228">String</span></span>|<span data-ttu-id="9f644-229">Командная строка для установки приложения</span><span class="sxs-lookup"><span data-stu-id="9f644-229">The command line to install this app</span></span>|
|<span data-ttu-id="9f644-230">унинсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="9f644-230">uninstallCommandLine</span></span>|<span data-ttu-id="9f644-231">String</span><span class="sxs-lookup"><span data-stu-id="9f644-231">String</span></span>|<span data-ttu-id="9f644-232">Командная строка для удаления приложения</span><span class="sxs-lookup"><span data-stu-id="9f644-232">The command line to uninstall this app</span></span>|
|<span data-ttu-id="9f644-233">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="9f644-233">applicableArchitectures</span></span>|[<span data-ttu-id="9f644-234">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="9f644-234">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="9f644-235">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="9f644-235">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="9f644-236">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="9f644-236">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="9f644-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9f644-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9f644-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9f644-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9f644-239">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="9f644-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9f644-240">минимумфридискспацеинмб</span><span class="sxs-lookup"><span data-stu-id="9f644-240">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="9f644-241">Int32</span><span class="sxs-lookup"><span data-stu-id="9f644-241">Int32</span></span>|<span data-ttu-id="9f644-242">Минимальное свободное место на диске, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-242">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="9f644-243">минимуммеморинмб</span><span class="sxs-lookup"><span data-stu-id="9f644-243">minimumMemoryInMB</span></span>|<span data-ttu-id="9f644-244">Int32</span><span class="sxs-lookup"><span data-stu-id="9f644-244">Int32</span></span>|<span data-ttu-id="9f644-245">Значение минимальной физической памяти, необходимой для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-245">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="9f644-246">минимумнумберофпроцессорс</span><span class="sxs-lookup"><span data-stu-id="9f644-246">minimumNumberOfProcessors</span></span>|<span data-ttu-id="9f644-247">Int32</span><span class="sxs-lookup"><span data-stu-id="9f644-247">Int32</span></span>|<span data-ttu-id="9f644-248">Значение минимального числа процессоров, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-248">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="9f644-249">минимумкпуспидинмхз</span><span class="sxs-lookup"><span data-stu-id="9f644-249">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="9f644-250">Int32</span><span class="sxs-lookup"><span data-stu-id="9f644-250">Int32</span></span>|<span data-ttu-id="9f644-251">Значение минимальной скорости ЦП, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-251">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="9f644-252">детектионрулес</span><span class="sxs-lookup"><span data-stu-id="9f644-252">detectionRules</span></span>|<span data-ttu-id="9f644-253">Коллекция [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="9f644-253">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="9f644-254">Правила обнаружения для определения бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="9f644-254">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9f644-255">рекуирементрулес</span><span class="sxs-lookup"><span data-stu-id="9f644-255">requirementRules</span></span>|<span data-ttu-id="9f644-256">Коллекция [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="9f644-256">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="9f644-257">Правила требований для обнаружения бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="9f644-257">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9f644-258">правила</span><span class="sxs-lookup"><span data-stu-id="9f644-258">rules</span></span>|<span data-ttu-id="9f644-259">Коллекция [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="9f644-259">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="9f644-260">Правила обнаружения и требований для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-260">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="9f644-261">инсталлекспериенце</span><span class="sxs-lookup"><span data-stu-id="9f644-261">installExperience</span></span>|[<span data-ttu-id="9f644-262">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="9f644-262">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="9f644-263">Установка приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-263">The install experience for this app.</span></span>|
|<span data-ttu-id="9f644-264">ретурнкодес</span><span class="sxs-lookup"><span data-stu-id="9f644-264">returnCodes</span></span>|<span data-ttu-id="9f644-265">Коллекция [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="9f644-265">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="9f644-266">Коды возврата для поведения после установки.</span><span class="sxs-lookup"><span data-stu-id="9f644-266">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="9f644-267">мсиинформатион</span><span class="sxs-lookup"><span data-stu-id="9f644-267">msiInformation</span></span>|[<span data-ttu-id="9f644-268">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="9f644-268">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="9f644-269">Сведения о MSI, если это приложение Win32 является приложением MSI.</span><span class="sxs-lookup"><span data-stu-id="9f644-269">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="9f644-270">сетупфилепас</span><span class="sxs-lookup"><span data-stu-id="9f644-270">setupFilePath</span></span>|<span data-ttu-id="9f644-271">String</span><span class="sxs-lookup"><span data-stu-id="9f644-271">String</span></span>|<span data-ttu-id="9f644-272">Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="9f644-272">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="9f644-273">минимумсуппортедвиндовсрелеасе</span><span class="sxs-lookup"><span data-stu-id="9f644-273">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="9f644-274">String</span><span class="sxs-lookup"><span data-stu-id="9f644-274">String</span></span>|<span data-ttu-id="9f644-275">Значение минимального поддерживаемого выпуска Windows.</span><span class="sxs-lookup"><span data-stu-id="9f644-275">The value for the minimum supported windows release.</span></span>|
|<span data-ttu-id="9f644-276">дисплайверсион</span><span class="sxs-lookup"><span data-stu-id="9f644-276">displayVersion</span></span>|<span data-ttu-id="9f644-277">String</span><span class="sxs-lookup"><span data-stu-id="9f644-277">String</span></span>|<span data-ttu-id="9f644-278">Версия, отображаемая в UX для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="9f644-278">The version displayed in the UX for this app.</span></span>|



## <a name="response"></a><span data-ttu-id="9f644-279">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f644-279">Response</span></span>
<span data-ttu-id="9f644-280">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f644-280">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f644-281">Пример</span><span class="sxs-lookup"><span data-stu-id="9f644-281">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f644-282">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f644-282">Request</span></span>
<span data-ttu-id="9f644-283">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f644-283">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 3359

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="9f644-284">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f644-284">Response</span></span>
<span data-ttu-id="9f644-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f644-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3531

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value",
  "displayVersion": "Display Version value"
}
```




