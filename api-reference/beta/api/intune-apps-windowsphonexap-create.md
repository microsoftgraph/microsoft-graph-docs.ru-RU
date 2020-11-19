---
title: Создание Виндовсфонексап
description: Создание нового объекта Виндовсфонексап.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 387f53cc1fe7e598e731c01fff85a7eb06eb5544
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49246420"
---
# <a name="create-windowsphonexap"></a><span data-ttu-id="ad75e-103">Создание Виндовсфонексап</span><span class="sxs-lookup"><span data-stu-id="ad75e-103">Create windowsPhoneXAP</span></span>

<span data-ttu-id="ad75e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad75e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad75e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad75e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad75e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad75e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad75e-107">Создание нового объекта [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="ad75e-107">Create a new [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad75e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ad75e-108">Prerequisites</span></span>
<span data-ttu-id="ad75e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad75e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad75e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad75e-111">Permission type</span></span>|<span data-ttu-id="ad75e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad75e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad75e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad75e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad75e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad75e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad75e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad75e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad75e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad75e-116">Not supported.</span></span>|
|<span data-ttu-id="ad75e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ad75e-117">Application</span></span>|<span data-ttu-id="ad75e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad75e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad75e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad75e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ad75e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ad75e-120">Request headers</span></span>
|<span data-ttu-id="ad75e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad75e-121">Header</span></span>|<span data-ttu-id="ad75e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad75e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad75e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad75e-123">Authorization</span></span>|<span data-ttu-id="ad75e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad75e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad75e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad75e-125">Accept</span></span>|<span data-ttu-id="ad75e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad75e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad75e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad75e-127">Request body</span></span>
<span data-ttu-id="ad75e-128">В тексте запроса добавьте представление объекта Виндовсфонексап в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad75e-128">In the request body, supply a JSON representation for the windowsPhoneXAP object.</span></span>

<span data-ttu-id="ad75e-129">В следующей таблице приведены свойства, необходимые при создании Виндовсфонексап.</span><span class="sxs-lookup"><span data-stu-id="ad75e-129">The following table shows the properties that are required when you create the windowsPhoneXAP.</span></span>

|<span data-ttu-id="ad75e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad75e-130">Property</span></span>|<span data-ttu-id="ad75e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ad75e-131">Type</span></span>|<span data-ttu-id="ad75e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ad75e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad75e-133">id</span><span class="sxs-lookup"><span data-stu-id="ad75e-133">id</span></span>|<span data-ttu-id="ad75e-134">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-134">String</span></span>|<span data-ttu-id="ad75e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ad75e-135">Key of the entity.</span></span> <span data-ttu-id="ad75e-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ad75e-137">displayName</span></span>|<span data-ttu-id="ad75e-138">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-138">String</span></span>|<span data-ttu-id="ad75e-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ad75e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ad75e-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-141">description</span><span class="sxs-lookup"><span data-stu-id="ad75e-141">description</span></span>|<span data-ttu-id="ad75e-142">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-142">String</span></span>|<span data-ttu-id="ad75e-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ad75e-143">The description of the app.</span></span> <span data-ttu-id="ad75e-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ad75e-145">publisher</span></span>|<span data-ttu-id="ad75e-146">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-146">String</span></span>|<span data-ttu-id="ad75e-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ad75e-147">The publisher of the app.</span></span> <span data-ttu-id="ad75e-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ad75e-149">largeIcon</span></span>|[<span data-ttu-id="ad75e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ad75e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ad75e-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ad75e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ad75e-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad75e-153">createdDateTime</span></span>|<span data-ttu-id="ad75e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad75e-154">DateTimeOffset</span></span>|<span data-ttu-id="ad75e-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ad75e-155">The date and time the app was created.</span></span> <span data-ttu-id="ad75e-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad75e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ad75e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad75e-158">DateTimeOffset</span></span>|<span data-ttu-id="ad75e-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ad75e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ad75e-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ad75e-161">isFeatured</span></span>|<span data-ttu-id="ad75e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad75e-162">Boolean</span></span>|<span data-ttu-id="ad75e-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ad75e-164">privacyInformationUrl</span></span>|<span data-ttu-id="ad75e-165">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-165">String</span></span>|<span data-ttu-id="ad75e-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ad75e-166">The privacy statement Url.</span></span> <span data-ttu-id="ad75e-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ad75e-168">informationUrl</span></span>|<span data-ttu-id="ad75e-169">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-169">String</span></span>|<span data-ttu-id="ad75e-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ad75e-170">The more information Url.</span></span> <span data-ttu-id="ad75e-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-172">owner</span><span class="sxs-lookup"><span data-stu-id="ad75e-172">owner</span></span>|<span data-ttu-id="ad75e-173">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-173">String</span></span>|<span data-ttu-id="ad75e-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ad75e-174">The owner of the app.</span></span> <span data-ttu-id="ad75e-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-176">developer</span><span class="sxs-lookup"><span data-stu-id="ad75e-176">developer</span></span>|<span data-ttu-id="ad75e-177">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-177">String</span></span>|<span data-ttu-id="ad75e-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ad75e-178">The developer of the app.</span></span> <span data-ttu-id="ad75e-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-180">notes</span><span class="sxs-lookup"><span data-stu-id="ad75e-180">notes</span></span>|<span data-ttu-id="ad75e-181">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-181">String</span></span>|<span data-ttu-id="ad75e-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ad75e-182">Notes for the app.</span></span> <span data-ttu-id="ad75e-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ad75e-184">uploadState</span></span>|<span data-ttu-id="ad75e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ad75e-185">Int32</span></span>|<span data-ttu-id="ad75e-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="ad75e-186">The upload state.</span></span> <span data-ttu-id="ad75e-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="ad75e-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ad75e-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ad75e-189">publishingState</span></span>|[<span data-ttu-id="ad75e-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="ad75e-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ad75e-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ad75e-191">The publishing state for the app.</span></span> <span data-ttu-id="ad75e-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ad75e-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ad75e-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ad75e-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ad75e-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ad75e-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ad75e-195">isAssigned</span></span>|<span data-ttu-id="ad75e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad75e-196">Boolean</span></span>|<span data-ttu-id="ad75e-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="ad75e-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ad75e-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ad75e-199">roleScopeTagIds</span></span>|<span data-ttu-id="ad75e-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ad75e-200">String collection</span></span>|<span data-ttu-id="ad75e-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ad75e-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ad75e-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="ad75e-203">dependentAppCount</span></span>|<span data-ttu-id="ad75e-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ad75e-204">Int32</span></span>|<span data-ttu-id="ad75e-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="ad75e-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ad75e-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="ad75e-207">supersedingAppCount</span></span>|<span data-ttu-id="ad75e-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ad75e-208">Int32</span></span>|<span data-ttu-id="ad75e-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="ad75e-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="ad75e-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="ad75e-211">supersededAppCount</span></span>|<span data-ttu-id="ad75e-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ad75e-212">Int32</span></span>|<span data-ttu-id="ad75e-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="ad75e-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="ad75e-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ad75e-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ad75e-215">committedContentVersion</span></span>|<span data-ttu-id="ad75e-216">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-216">String</span></span>|<span data-ttu-id="ad75e-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="ad75e-217">The internal committed content version.</span></span> <span data-ttu-id="ad75e-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ad75e-219">fileName</span><span class="sxs-lookup"><span data-stu-id="ad75e-219">fileName</span></span>|<span data-ttu-id="ad75e-220">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-220">String</span></span>|<span data-ttu-id="ad75e-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ad75e-221">The name of the main Lob application file.</span></span> <span data-ttu-id="ad75e-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ad75e-223">size</span><span class="sxs-lookup"><span data-stu-id="ad75e-223">size</span></span>|<span data-ttu-id="ad75e-224">Int64</span><span class="sxs-lookup"><span data-stu-id="ad75e-224">Int64</span></span>|<span data-ttu-id="ad75e-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="ad75e-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="ad75e-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad75e-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ad75e-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ad75e-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ad75e-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ad75e-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="ad75e-229">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ad75e-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ad75e-230">продуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="ad75e-230">productIdentifier</span></span>|<span data-ttu-id="ad75e-231">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-231">String</span></span>|<span data-ttu-id="ad75e-232">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="ad75e-232">The Product Identifier.</span></span>|
|<span data-ttu-id="ad75e-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ad75e-233">identityVersion</span></span>|<span data-ttu-id="ad75e-234">String</span><span class="sxs-lookup"><span data-stu-id="ad75e-234">String</span></span>|<span data-ttu-id="ad75e-235">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ad75e-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ad75e-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad75e-236">Response</span></span>
<span data-ttu-id="ad75e-237">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad75e-237">If successful, this method returns a `201 Created` response code and a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad75e-238">Пример</span><span class="sxs-lookup"><span data-stu-id="ad75e-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad75e-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad75e-239">Request</span></span>
<span data-ttu-id="ad75e-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad75e-240">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ad75e-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad75e-241">Response</span></span>
<span data-ttu-id="ad75e-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad75e-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




