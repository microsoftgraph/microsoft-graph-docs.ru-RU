---
title: Создание windowsAppX
description: Создание нового объекта windowsAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0227c5a7ce9d25d2167401c1f3cf8afcc47a3083
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694762"
---
# <a name="create-windowsappx"></a><span data-ttu-id="7052d-103">Создание windowsAppX</span><span class="sxs-lookup"><span data-stu-id="7052d-103">Create windowsAppX</span></span>

<span data-ttu-id="7052d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7052d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7052d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7052d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7052d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7052d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7052d-107">Создание нового объекта [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="7052d-107">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7052d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7052d-108">Prerequisites</span></span>
<span data-ttu-id="7052d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7052d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7052d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7052d-111">Permission type</span></span>|<span data-ttu-id="7052d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7052d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7052d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7052d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7052d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7052d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7052d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7052d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7052d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7052d-116">Not supported.</span></span>|
|<span data-ttu-id="7052d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7052d-117">Application</span></span>|<span data-ttu-id="7052d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7052d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7052d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7052d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7052d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7052d-120">Request headers</span></span>
|<span data-ttu-id="7052d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7052d-121">Header</span></span>|<span data-ttu-id="7052d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7052d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7052d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7052d-123">Authorization</span></span>|<span data-ttu-id="7052d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7052d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7052d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7052d-125">Accept</span></span>|<span data-ttu-id="7052d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7052d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7052d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7052d-127">Request body</span></span>
<span data-ttu-id="7052d-128">В тексте запроса добавьте представление объекта windowsAppX в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7052d-128">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="7052d-129">В следующей таблице приведены свойства, необходимые при создании windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="7052d-129">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="7052d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7052d-130">Property</span></span>|<span data-ttu-id="7052d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7052d-131">Type</span></span>|<span data-ttu-id="7052d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7052d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7052d-133">id</span><span class="sxs-lookup"><span data-stu-id="7052d-133">id</span></span>|<span data-ttu-id="7052d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7052d-134">String</span></span>|<span data-ttu-id="7052d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7052d-135">Key of the entity.</span></span> <span data-ttu-id="7052d-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7052d-137">displayName</span></span>|<span data-ttu-id="7052d-138">Строка</span><span class="sxs-lookup"><span data-stu-id="7052d-138">String</span></span>|<span data-ttu-id="7052d-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="7052d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7052d-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-141">description</span><span class="sxs-lookup"><span data-stu-id="7052d-141">description</span></span>|<span data-ttu-id="7052d-142">Строка</span><span class="sxs-lookup"><span data-stu-id="7052d-142">String</span></span>|<span data-ttu-id="7052d-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7052d-143">The description of the app.</span></span> <span data-ttu-id="7052d-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-145">publisher</span><span class="sxs-lookup"><span data-stu-id="7052d-145">publisher</span></span>|<span data-ttu-id="7052d-146">String</span><span class="sxs-lookup"><span data-stu-id="7052d-146">String</span></span>|<span data-ttu-id="7052d-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="7052d-147">The publisher of the app.</span></span> <span data-ttu-id="7052d-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7052d-149">largeIcon</span></span>|[<span data-ttu-id="7052d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7052d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7052d-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="7052d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7052d-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7052d-153">createdDateTime</span></span>|<span data-ttu-id="7052d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7052d-154">DateTimeOffset</span></span>|<span data-ttu-id="7052d-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="7052d-155">The date and time the app was created.</span></span> <span data-ttu-id="7052d-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7052d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7052d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7052d-158">DateTimeOffset</span></span>|<span data-ttu-id="7052d-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="7052d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="7052d-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7052d-161">isFeatured</span></span>|<span data-ttu-id="7052d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7052d-162">Boolean</span></span>|<span data-ttu-id="7052d-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7052d-164">privacyInformationUrl</span></span>|<span data-ttu-id="7052d-165">String</span><span class="sxs-lookup"><span data-stu-id="7052d-165">String</span></span>|<span data-ttu-id="7052d-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="7052d-166">The privacy statement Url.</span></span> <span data-ttu-id="7052d-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7052d-168">informationUrl</span></span>|<span data-ttu-id="7052d-169">String</span><span class="sxs-lookup"><span data-stu-id="7052d-169">String</span></span>|<span data-ttu-id="7052d-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="7052d-170">The more information Url.</span></span> <span data-ttu-id="7052d-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-172">owner</span><span class="sxs-lookup"><span data-stu-id="7052d-172">owner</span></span>|<span data-ttu-id="7052d-173">String</span><span class="sxs-lookup"><span data-stu-id="7052d-173">String</span></span>|<span data-ttu-id="7052d-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="7052d-174">The owner of the app.</span></span> <span data-ttu-id="7052d-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-176">developer</span><span class="sxs-lookup"><span data-stu-id="7052d-176">developer</span></span>|<span data-ttu-id="7052d-177">String</span><span class="sxs-lookup"><span data-stu-id="7052d-177">String</span></span>|<span data-ttu-id="7052d-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="7052d-178">The developer of the app.</span></span> <span data-ttu-id="7052d-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-180">notes</span><span class="sxs-lookup"><span data-stu-id="7052d-180">notes</span></span>|<span data-ttu-id="7052d-181">String</span><span class="sxs-lookup"><span data-stu-id="7052d-181">String</span></span>|<span data-ttu-id="7052d-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="7052d-182">Notes for the app.</span></span> <span data-ttu-id="7052d-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="7052d-184">uploadState</span></span>|<span data-ttu-id="7052d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7052d-185">Int32</span></span>|<span data-ttu-id="7052d-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="7052d-186">The upload state.</span></span> <span data-ttu-id="7052d-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="7052d-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="7052d-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="7052d-189">publishingState</span></span>|[<span data-ttu-id="7052d-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="7052d-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7052d-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="7052d-191">The publishing state for the app.</span></span> <span data-ttu-id="7052d-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="7052d-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7052d-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="7052d-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7052d-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7052d-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7052d-195">isAssigned</span></span>|<span data-ttu-id="7052d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="7052d-196">Boolean</span></span>|<span data-ttu-id="7052d-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="7052d-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7052d-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7052d-199">roleScopeTagIds</span></span>|<span data-ttu-id="7052d-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7052d-200">String collection</span></span>|<span data-ttu-id="7052d-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="7052d-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7052d-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="7052d-203">dependentAppCount</span></span>|<span data-ttu-id="7052d-204">Int32</span><span class="sxs-lookup"><span data-stu-id="7052d-204">Int32</span></span>|<span data-ttu-id="7052d-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="7052d-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7052d-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="7052d-207">supersedingAppCount</span></span>|<span data-ttu-id="7052d-208">Int32</span><span class="sxs-lookup"><span data-stu-id="7052d-208">Int32</span></span>|<span data-ttu-id="7052d-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="7052d-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="7052d-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="7052d-211">supersededAppCount</span></span>|<span data-ttu-id="7052d-212">Int32</span><span class="sxs-lookup"><span data-stu-id="7052d-212">Int32</span></span>|<span data-ttu-id="7052d-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="7052d-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="7052d-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7052d-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7052d-215">committedContentVersion</span></span>|<span data-ttu-id="7052d-216">String</span><span class="sxs-lookup"><span data-stu-id="7052d-216">String</span></span>|<span data-ttu-id="7052d-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="7052d-217">The internal committed content version.</span></span> <span data-ttu-id="7052d-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7052d-219">fileName</span><span class="sxs-lookup"><span data-stu-id="7052d-219">fileName</span></span>|<span data-ttu-id="7052d-220">String</span><span class="sxs-lookup"><span data-stu-id="7052d-220">String</span></span>|<span data-ttu-id="7052d-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="7052d-221">The name of the main Lob application file.</span></span> <span data-ttu-id="7052d-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7052d-223">size</span><span class="sxs-lookup"><span data-stu-id="7052d-223">size</span></span>|<span data-ttu-id="7052d-224">Int64</span><span class="sxs-lookup"><span data-stu-id="7052d-224">Int64</span></span>|<span data-ttu-id="7052d-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="7052d-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="7052d-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7052d-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7052d-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="7052d-227">applicableArchitectures</span></span>|[<span data-ttu-id="7052d-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="7052d-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="7052d-229">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="7052d-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="7052d-230">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="7052d-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="7052d-231">identityName</span><span class="sxs-lookup"><span data-stu-id="7052d-231">identityName</span></span>|<span data-ttu-id="7052d-232">String</span><span class="sxs-lookup"><span data-stu-id="7052d-232">String</span></span>|<span data-ttu-id="7052d-233">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="7052d-233">The Identity Name.</span></span>|
|<span data-ttu-id="7052d-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="7052d-234">identityPublisherHash</span></span>|<span data-ttu-id="7052d-235">String</span><span class="sxs-lookup"><span data-stu-id="7052d-235">String</span></span>|<span data-ttu-id="7052d-236">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="7052d-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="7052d-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7052d-237">identityResourceIdentifier</span></span>|<span data-ttu-id="7052d-238">String</span><span class="sxs-lookup"><span data-stu-id="7052d-238">String</span></span>|<span data-ttu-id="7052d-239">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="7052d-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="7052d-240">isBundle</span><span class="sxs-lookup"><span data-stu-id="7052d-240">isBundle</span></span>|<span data-ttu-id="7052d-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="7052d-241">Boolean</span></span>|<span data-ttu-id="7052d-242">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="7052d-242">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="7052d-243">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7052d-243">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7052d-244">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7052d-244">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="7052d-245">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="7052d-245">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="7052d-246">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7052d-246">identityVersion</span></span>|<span data-ttu-id="7052d-247">String</span><span class="sxs-lookup"><span data-stu-id="7052d-247">String</span></span>|<span data-ttu-id="7052d-248">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="7052d-248">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="7052d-249">Ответ</span><span class="sxs-lookup"><span data-stu-id="7052d-249">Response</span></span>
<span data-ttu-id="7052d-250">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsAppX](../resources/intune-apps-windowsappx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7052d-250">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7052d-251">Пример</span><span class="sxs-lookup"><span data-stu-id="7052d-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="7052d-252">Запрос</span><span class="sxs-lookup"><span data-stu-id="7052d-252">Request</span></span>
<span data-ttu-id="7052d-253">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7052d-253">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7052d-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="7052d-254">Response</span></span>
<span data-ttu-id="7052d-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7052d-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





