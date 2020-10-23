---
title: Создание Виндовсфонексап
description: Создание нового объекта Виндовсфонексап.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e97eb6fba971e8bde1f437f0979f08d249a3a643
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727095"
---
# <a name="create-windowsphonexap"></a><span data-ttu-id="3ffbd-103">Создание Виндовсфонексап</span><span class="sxs-lookup"><span data-stu-id="3ffbd-103">Create windowsPhoneXAP</span></span>

<span data-ttu-id="3ffbd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ffbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ffbd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ffbd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ffbd-107">Создание нового объекта [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="3ffbd-107">Create a new [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ffbd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3ffbd-108">Prerequisites</span></span>
<span data-ttu-id="3ffbd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ffbd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ffbd-111">Permission type</span></span>|<span data-ttu-id="3ffbd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ffbd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ffbd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ffbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ffbd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ffbd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3ffbd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ffbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ffbd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-116">Not supported.</span></span>|
|<span data-ttu-id="3ffbd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ffbd-117">Application</span></span>|<span data-ttu-id="3ffbd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ffbd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ffbd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ffbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3ffbd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3ffbd-120">Request headers</span></span>
|<span data-ttu-id="3ffbd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ffbd-121">Header</span></span>|<span data-ttu-id="3ffbd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3ffbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ffbd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ffbd-123">Authorization</span></span>|<span data-ttu-id="3ffbd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ffbd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3ffbd-125">Accept</span></span>|<span data-ttu-id="3ffbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ffbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ffbd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ffbd-127">Request body</span></span>
<span data-ttu-id="3ffbd-128">В тексте запроса добавьте представление объекта Виндовсфонексап в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-128">In the request body, supply a JSON representation for the windowsPhoneXAP object.</span></span>

<span data-ttu-id="3ffbd-129">В следующей таблице приведены свойства, необходимые при создании Виндовсфонексап.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-129">The following table shows the properties that are required when you create the windowsPhoneXAP.</span></span>

|<span data-ttu-id="3ffbd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ffbd-130">Property</span></span>|<span data-ttu-id="3ffbd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3ffbd-131">Type</span></span>|<span data-ttu-id="3ffbd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3ffbd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ffbd-133">id</span><span class="sxs-lookup"><span data-stu-id="3ffbd-133">id</span></span>|<span data-ttu-id="3ffbd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3ffbd-134">String</span></span>|<span data-ttu-id="3ffbd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-135">Key of the entity.</span></span> <span data-ttu-id="3ffbd-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3ffbd-137">displayName</span></span>|<span data-ttu-id="3ffbd-138">Строка</span><span class="sxs-lookup"><span data-stu-id="3ffbd-138">String</span></span>|<span data-ttu-id="3ffbd-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3ffbd-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-141">description</span><span class="sxs-lookup"><span data-stu-id="3ffbd-141">description</span></span>|<span data-ttu-id="3ffbd-142">Строка</span><span class="sxs-lookup"><span data-stu-id="3ffbd-142">String</span></span>|<span data-ttu-id="3ffbd-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-143">The description of the app.</span></span> <span data-ttu-id="3ffbd-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3ffbd-145">publisher</span></span>|<span data-ttu-id="3ffbd-146">String</span><span class="sxs-lookup"><span data-stu-id="3ffbd-146">String</span></span>|<span data-ttu-id="3ffbd-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-147">The publisher of the app.</span></span> <span data-ttu-id="3ffbd-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3ffbd-149">largeIcon</span></span>|[<span data-ttu-id="3ffbd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3ffbd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3ffbd-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3ffbd-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ffbd-153">createdDateTime</span></span>|<span data-ttu-id="3ffbd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ffbd-154">DateTimeOffset</span></span>|<span data-ttu-id="3ffbd-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-155">The date and time the app was created.</span></span> <span data-ttu-id="3ffbd-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ffbd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3ffbd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ffbd-158">DateTimeOffset</span></span>|<span data-ttu-id="3ffbd-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="3ffbd-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3ffbd-161">isFeatured</span></span>|<span data-ttu-id="3ffbd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ffbd-162">Boolean</span></span>|<span data-ttu-id="3ffbd-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3ffbd-164">privacyInformationUrl</span></span>|<span data-ttu-id="3ffbd-165">String</span><span class="sxs-lookup"><span data-stu-id="3ffbd-165">String</span></span>|<span data-ttu-id="3ffbd-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-166">The privacy statement Url.</span></span> <span data-ttu-id="3ffbd-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3ffbd-168">informationUrl</span></span>|<span data-ttu-id="3ffbd-169">String</span><span class="sxs-lookup"><span data-stu-id="3ffbd-169">String</span></span>|<span data-ttu-id="3ffbd-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-170">The more information Url.</span></span> <span data-ttu-id="3ffbd-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-172">owner</span><span class="sxs-lookup"><span data-stu-id="3ffbd-172">owner</span></span>|<span data-ttu-id="3ffbd-173">String</span><span class="sxs-lookup"><span data-stu-id="3ffbd-173">String</span></span>|<span data-ttu-id="3ffbd-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-174">The owner of the app.</span></span> <span data-ttu-id="3ffbd-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-176">developer</span><span class="sxs-lookup"><span data-stu-id="3ffbd-176">developer</span></span>|<span data-ttu-id="3ffbd-177">String</span><span class="sxs-lookup"><span data-stu-id="3ffbd-177">String</span></span>|<span data-ttu-id="3ffbd-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-178">The developer of the app.</span></span> <span data-ttu-id="3ffbd-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-180">notes</span><span class="sxs-lookup"><span data-stu-id="3ffbd-180">notes</span></span>|<span data-ttu-id="3ffbd-181">String</span><span class="sxs-lookup"><span data-stu-id="3ffbd-181">String</span></span>|<span data-ttu-id="3ffbd-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-182">Notes for the app.</span></span> <span data-ttu-id="3ffbd-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="3ffbd-184">uploadState</span></span>|<span data-ttu-id="3ffbd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3ffbd-185">Int32</span></span>|<span data-ttu-id="3ffbd-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-186">The upload state.</span></span> <span data-ttu-id="3ffbd-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="3ffbd-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="3ffbd-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="3ffbd-189">publishingState</span></span>|[<span data-ttu-id="3ffbd-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="3ffbd-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3ffbd-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-191">The publishing state for the app.</span></span> <span data-ttu-id="3ffbd-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3ffbd-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="3ffbd-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3ffbd-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3ffbd-195">isAssigned</span></span>|<span data-ttu-id="3ffbd-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ffbd-196">Boolean</span></span>|<span data-ttu-id="3ffbd-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3ffbd-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3ffbd-199">roleScopeTagIds</span></span>|<span data-ttu-id="3ffbd-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3ffbd-200">String collection</span></span>|<span data-ttu-id="3ffbd-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3ffbd-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="3ffbd-203">dependentAppCount</span></span>|<span data-ttu-id="3ffbd-204">Int32</span><span class="sxs-lookup"><span data-stu-id="3ffbd-204">Int32</span></span>|<span data-ttu-id="3ffbd-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="3ffbd-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="3ffbd-207">supersedingAppCount</span></span>|<span data-ttu-id="3ffbd-208">Int32</span><span class="sxs-lookup"><span data-stu-id="3ffbd-208">Int32</span></span>|<span data-ttu-id="3ffbd-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="3ffbd-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="3ffbd-211">supersededAppCount</span></span>|<span data-ttu-id="3ffbd-212">Int32</span><span class="sxs-lookup"><span data-stu-id="3ffbd-212">Int32</span></span>|<span data-ttu-id="3ffbd-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="3ffbd-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3ffbd-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3ffbd-215">committedContentVersion</span></span>|<span data-ttu-id="3ffbd-216">String</span><span class="sxs-lookup"><span data-stu-id="3ffbd-216">String</span></span>|<span data-ttu-id="3ffbd-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-217">The internal committed content version.</span></span> <span data-ttu-id="3ffbd-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3ffbd-219">fileName</span><span class="sxs-lookup"><span data-stu-id="3ffbd-219">fileName</span></span>|<span data-ttu-id="3ffbd-220">String</span><span class="sxs-lookup"><span data-stu-id="3ffbd-220">String</span></span>|<span data-ttu-id="3ffbd-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-221">The name of the main Lob application file.</span></span> <span data-ttu-id="3ffbd-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3ffbd-223">size</span><span class="sxs-lookup"><span data-stu-id="3ffbd-223">size</span></span>|<span data-ttu-id="3ffbd-224">Int64</span><span class="sxs-lookup"><span data-stu-id="3ffbd-224">Int64</span></span>|<span data-ttu-id="3ffbd-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="3ffbd-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3ffbd-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3ffbd-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3ffbd-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3ffbd-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3ffbd-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="3ffbd-229">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3ffbd-230">продуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="3ffbd-230">productIdentifier</span></span>|<span data-ttu-id="3ffbd-231">Строка</span><span class="sxs-lookup"><span data-stu-id="3ffbd-231">String</span></span>|<span data-ttu-id="3ffbd-232">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-232">The Product Identifier.</span></span>|
|<span data-ttu-id="3ffbd-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="3ffbd-233">identityVersion</span></span>|<span data-ttu-id="3ffbd-234">String</span><span class="sxs-lookup"><span data-stu-id="3ffbd-234">String</span></span>|<span data-ttu-id="3ffbd-235">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="3ffbd-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ffbd-236">Response</span></span>
<span data-ttu-id="3ffbd-237">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-237">If successful, this method returns a `201 Created` response code and a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ffbd-238">Пример</span><span class="sxs-lookup"><span data-stu-id="3ffbd-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ffbd-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ffbd-239">Request</span></span>
<span data-ttu-id="3ffbd-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1294

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="3ffbd-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ffbd-241">Response</span></span>
<span data-ttu-id="3ffbd-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ffbd-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1466

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```





