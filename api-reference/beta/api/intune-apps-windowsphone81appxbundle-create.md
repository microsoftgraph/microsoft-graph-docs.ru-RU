---
title: Создание windowsPhone81AppXBundle
description: Создание нового объекта windowsPhone81AppXBundle.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 519469de33158ae2199b3a31b64f09fbd046eed2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697142"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="30a06-103">Создание windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="30a06-103">Create windowsPhone81AppXBundle</span></span>

<span data-ttu-id="30a06-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30a06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30a06-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30a06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30a06-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30a06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30a06-107">Создание нового объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="30a06-107">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30a06-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="30a06-108">Prerequisites</span></span>
<span data-ttu-id="30a06-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30a06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30a06-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30a06-111">Permission type</span></span>|<span data-ttu-id="30a06-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30a06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30a06-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30a06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30a06-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30a06-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30a06-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30a06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30a06-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30a06-116">Not supported.</span></span>|
|<span data-ttu-id="30a06-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30a06-117">Application</span></span>|<span data-ttu-id="30a06-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30a06-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30a06-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30a06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="30a06-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="30a06-120">Request headers</span></span>
|<span data-ttu-id="30a06-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30a06-121">Header</span></span>|<span data-ttu-id="30a06-122">Значение</span><span class="sxs-lookup"><span data-stu-id="30a06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30a06-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30a06-123">Authorization</span></span>|<span data-ttu-id="30a06-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30a06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30a06-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30a06-125">Accept</span></span>|<span data-ttu-id="30a06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30a06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30a06-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30a06-127">Request body</span></span>
<span data-ttu-id="30a06-128">В тексте запроса добавьте представление объекта windowsPhone81AppXBundle в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30a06-128">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="30a06-129">В следующей таблице приведены свойства, необходимые при создании windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="30a06-129">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="30a06-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="30a06-130">Property</span></span>|<span data-ttu-id="30a06-131">Тип</span><span class="sxs-lookup"><span data-stu-id="30a06-131">Type</span></span>|<span data-ttu-id="30a06-132">Описание</span><span class="sxs-lookup"><span data-stu-id="30a06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30a06-133">id</span><span class="sxs-lookup"><span data-stu-id="30a06-133">id</span></span>|<span data-ttu-id="30a06-134">Строка</span><span class="sxs-lookup"><span data-stu-id="30a06-134">String</span></span>|<span data-ttu-id="30a06-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="30a06-135">Key of the entity.</span></span> <span data-ttu-id="30a06-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-137">displayName</span><span class="sxs-lookup"><span data-stu-id="30a06-137">displayName</span></span>|<span data-ttu-id="30a06-138">Строка</span><span class="sxs-lookup"><span data-stu-id="30a06-138">String</span></span>|<span data-ttu-id="30a06-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="30a06-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="30a06-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-141">description</span><span class="sxs-lookup"><span data-stu-id="30a06-141">description</span></span>|<span data-ttu-id="30a06-142">Строка</span><span class="sxs-lookup"><span data-stu-id="30a06-142">String</span></span>|<span data-ttu-id="30a06-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="30a06-143">The description of the app.</span></span> <span data-ttu-id="30a06-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-145">publisher</span><span class="sxs-lookup"><span data-stu-id="30a06-145">publisher</span></span>|<span data-ttu-id="30a06-146">String</span><span class="sxs-lookup"><span data-stu-id="30a06-146">String</span></span>|<span data-ttu-id="30a06-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="30a06-147">The publisher of the app.</span></span> <span data-ttu-id="30a06-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="30a06-149">largeIcon</span></span>|[<span data-ttu-id="30a06-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="30a06-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="30a06-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="30a06-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="30a06-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30a06-153">createdDateTime</span></span>|<span data-ttu-id="30a06-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30a06-154">DateTimeOffset</span></span>|<span data-ttu-id="30a06-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="30a06-155">The date and time the app was created.</span></span> <span data-ttu-id="30a06-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30a06-157">lastModifiedDateTime</span></span>|<span data-ttu-id="30a06-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30a06-158">DateTimeOffset</span></span>|<span data-ttu-id="30a06-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="30a06-159">The date and time the app was last modified.</span></span> <span data-ttu-id="30a06-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="30a06-161">isFeatured</span></span>|<span data-ttu-id="30a06-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="30a06-162">Boolean</span></span>|<span data-ttu-id="30a06-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="30a06-164">privacyInformationUrl</span></span>|<span data-ttu-id="30a06-165">String</span><span class="sxs-lookup"><span data-stu-id="30a06-165">String</span></span>|<span data-ttu-id="30a06-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="30a06-166">The privacy statement Url.</span></span> <span data-ttu-id="30a06-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="30a06-168">informationUrl</span></span>|<span data-ttu-id="30a06-169">String</span><span class="sxs-lookup"><span data-stu-id="30a06-169">String</span></span>|<span data-ttu-id="30a06-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="30a06-170">The more information Url.</span></span> <span data-ttu-id="30a06-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-172">owner</span><span class="sxs-lookup"><span data-stu-id="30a06-172">owner</span></span>|<span data-ttu-id="30a06-173">String</span><span class="sxs-lookup"><span data-stu-id="30a06-173">String</span></span>|<span data-ttu-id="30a06-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="30a06-174">The owner of the app.</span></span> <span data-ttu-id="30a06-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-176">developer</span><span class="sxs-lookup"><span data-stu-id="30a06-176">developer</span></span>|<span data-ttu-id="30a06-177">String</span><span class="sxs-lookup"><span data-stu-id="30a06-177">String</span></span>|<span data-ttu-id="30a06-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="30a06-178">The developer of the app.</span></span> <span data-ttu-id="30a06-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-180">notes</span><span class="sxs-lookup"><span data-stu-id="30a06-180">notes</span></span>|<span data-ttu-id="30a06-181">String</span><span class="sxs-lookup"><span data-stu-id="30a06-181">String</span></span>|<span data-ttu-id="30a06-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="30a06-182">Notes for the app.</span></span> <span data-ttu-id="30a06-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="30a06-184">uploadState</span></span>|<span data-ttu-id="30a06-185">Int32</span><span class="sxs-lookup"><span data-stu-id="30a06-185">Int32</span></span>|<span data-ttu-id="30a06-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="30a06-186">The upload state.</span></span> <span data-ttu-id="30a06-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="30a06-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="30a06-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="30a06-189">publishingState</span></span>|[<span data-ttu-id="30a06-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="30a06-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="30a06-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="30a06-191">The publishing state for the app.</span></span> <span data-ttu-id="30a06-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="30a06-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="30a06-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="30a06-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="30a06-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="30a06-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="30a06-195">isAssigned</span></span>|<span data-ttu-id="30a06-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="30a06-196">Boolean</span></span>|<span data-ttu-id="30a06-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="30a06-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="30a06-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="30a06-199">roleScopeTagIds</span></span>|<span data-ttu-id="30a06-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="30a06-200">String collection</span></span>|<span data-ttu-id="30a06-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="30a06-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="30a06-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="30a06-203">dependentAppCount</span></span>|<span data-ttu-id="30a06-204">Int32</span><span class="sxs-lookup"><span data-stu-id="30a06-204">Int32</span></span>|<span data-ttu-id="30a06-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="30a06-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="30a06-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="30a06-207">supersedingAppCount</span></span>|<span data-ttu-id="30a06-208">Int32</span><span class="sxs-lookup"><span data-stu-id="30a06-208">Int32</span></span>|<span data-ttu-id="30a06-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="30a06-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="30a06-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="30a06-211">supersededAppCount</span></span>|<span data-ttu-id="30a06-212">Int32</span><span class="sxs-lookup"><span data-stu-id="30a06-212">Int32</span></span>|<span data-ttu-id="30a06-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="30a06-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="30a06-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30a06-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="30a06-215">committedContentVersion</span></span>|<span data-ttu-id="30a06-216">String</span><span class="sxs-lookup"><span data-stu-id="30a06-216">String</span></span>|<span data-ttu-id="30a06-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="30a06-217">The internal committed content version.</span></span> <span data-ttu-id="30a06-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="30a06-219">fileName</span><span class="sxs-lookup"><span data-stu-id="30a06-219">fileName</span></span>|<span data-ttu-id="30a06-220">String</span><span class="sxs-lookup"><span data-stu-id="30a06-220">String</span></span>|<span data-ttu-id="30a06-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="30a06-221">The name of the main Lob application file.</span></span> <span data-ttu-id="30a06-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="30a06-223">size</span><span class="sxs-lookup"><span data-stu-id="30a06-223">size</span></span>|<span data-ttu-id="30a06-224">Int64</span><span class="sxs-lookup"><span data-stu-id="30a06-224">Int64</span></span>|<span data-ttu-id="30a06-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="30a06-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="30a06-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="30a06-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="30a06-227">applicableArchitectures</span></span>|[<span data-ttu-id="30a06-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="30a06-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="30a06-229">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="30a06-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="30a06-230">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="30a06-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="30a06-231">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="30a06-231">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="30a06-232">identityName</span><span class="sxs-lookup"><span data-stu-id="30a06-232">identityName</span></span>|<span data-ttu-id="30a06-233">String</span><span class="sxs-lookup"><span data-stu-id="30a06-233">String</span></span>|<span data-ttu-id="30a06-234">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="30a06-234">The Identity Name.</span></span> <span data-ttu-id="30a06-235">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="30a06-235">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="30a06-236">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="30a06-236">identityPublisherHash</span></span>|<span data-ttu-id="30a06-237">String</span><span class="sxs-lookup"><span data-stu-id="30a06-237">String</span></span>|<span data-ttu-id="30a06-238">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="30a06-238">The Identity Publisher Hash.</span></span> <span data-ttu-id="30a06-239">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="30a06-239">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="30a06-240">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="30a06-240">identityResourceIdentifier</span></span>|<span data-ttu-id="30a06-241">String</span><span class="sxs-lookup"><span data-stu-id="30a06-241">String</span></span>|<span data-ttu-id="30a06-242">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="30a06-242">The Identity Resource Identifier.</span></span> <span data-ttu-id="30a06-243">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="30a06-243">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="30a06-244">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="30a06-244">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="30a06-245">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="30a06-245">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="30a06-246">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="30a06-246">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="30a06-247">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="30a06-247">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="30a06-248">фонепродуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="30a06-248">phoneProductIdentifier</span></span>|<span data-ttu-id="30a06-249">Строка</span><span class="sxs-lookup"><span data-stu-id="30a06-249">String</span></span>|<span data-ttu-id="30a06-250">Идентификатор телефонного продукта.</span><span class="sxs-lookup"><span data-stu-id="30a06-250">The Phone Product Identifier.</span></span> <span data-ttu-id="30a06-251">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="30a06-251">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="30a06-252">фонепублишерид</span><span class="sxs-lookup"><span data-stu-id="30a06-252">phonePublisherId</span></span>|<span data-ttu-id="30a06-253">Строка</span><span class="sxs-lookup"><span data-stu-id="30a06-253">String</span></span>|<span data-ttu-id="30a06-254">Идентификатор издателя телефона. наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="30a06-254">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="30a06-255">identityVersion</span><span class="sxs-lookup"><span data-stu-id="30a06-255">identityVersion</span></span>|<span data-ttu-id="30a06-256">String</span><span class="sxs-lookup"><span data-stu-id="30a06-256">String</span></span>|<span data-ttu-id="30a06-257">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="30a06-257">The identity version.</span></span> <span data-ttu-id="30a06-258">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="30a06-258">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="30a06-259">аппкспаккажеинформатионлист</span><span class="sxs-lookup"><span data-stu-id="30a06-259">appXPackageInformationList</span></span>|<span data-ttu-id="30a06-260">Коллекция [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="30a06-260">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="30a06-261">Список сведений о пакете AppX.</span><span class="sxs-lookup"><span data-stu-id="30a06-261">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="30a06-262">Ответ</span><span class="sxs-lookup"><span data-stu-id="30a06-262">Response</span></span>
<span data-ttu-id="30a06-263">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30a06-263">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30a06-264">Пример</span><span class="sxs-lookup"><span data-stu-id="30a06-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="30a06-265">Запрос</span><span class="sxs-lookup"><span data-stu-id="30a06-265">Request</span></span>
<span data-ttu-id="30a06-266">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30a06-266">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2368

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="30a06-267">Отклик</span><span class="sxs-lookup"><span data-stu-id="30a06-267">Response</span></span>
<span data-ttu-id="30a06-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30a06-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2540

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
      }
    }
  ]
}
```





