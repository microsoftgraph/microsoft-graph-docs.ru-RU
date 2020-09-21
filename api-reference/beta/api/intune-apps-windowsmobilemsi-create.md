---
title: Create windowsMobileMSI
description: Создание объекта windowsMobileMSI.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3bd2770e7fd94324c966d79fba3b57c36e9a9285
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976517"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="1cd60-103">Create windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="1cd60-103">Create windowsMobileMSI</span></span>

<span data-ttu-id="1cd60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cd60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1cd60-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cd60-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1cd60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cd60-107">Создание объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-107">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cd60-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1cd60-108">Prerequisites</span></span>
<span data-ttu-id="1cd60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cd60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cd60-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cd60-111">Permission type</span></span>|<span data-ttu-id="1cd60-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cd60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cd60-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cd60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1cd60-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cd60-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1cd60-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cd60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cd60-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd60-116">Not supported.</span></span>|
|<span data-ttu-id="1cd60-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cd60-117">Application</span></span>|<span data-ttu-id="1cd60-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cd60-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cd60-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cd60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1cd60-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1cd60-120">Request headers</span></span>
|<span data-ttu-id="1cd60-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cd60-121">Header</span></span>|<span data-ttu-id="1cd60-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1cd60-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cd60-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cd60-123">Authorization</span></span>|<span data-ttu-id="1cd60-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cd60-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cd60-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1cd60-125">Accept</span></span>|<span data-ttu-id="1cd60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1cd60-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cd60-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1cd60-127">Request body</span></span>
<span data-ttu-id="1cd60-128">В тексте запроса добавьте представление объекта windowsMobileMSI в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cd60-128">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="1cd60-129">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="1cd60-129">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="1cd60-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cd60-130">Property</span></span>|<span data-ttu-id="1cd60-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1cd60-131">Type</span></span>|<span data-ttu-id="1cd60-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1cd60-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd60-133">id</span><span class="sxs-lookup"><span data-stu-id="1cd60-133">id</span></span>|<span data-ttu-id="1cd60-134">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-134">String</span></span>|<span data-ttu-id="1cd60-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1cd60-135">Key of the entity.</span></span> <span data-ttu-id="1cd60-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1cd60-137">displayName</span></span>|<span data-ttu-id="1cd60-138">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-138">String</span></span>|<span data-ttu-id="1cd60-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="1cd60-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1cd60-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-141">description</span><span class="sxs-lookup"><span data-stu-id="1cd60-141">description</span></span>|<span data-ttu-id="1cd60-142">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-142">String</span></span>|<span data-ttu-id="1cd60-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd60-143">The description of the app.</span></span> <span data-ttu-id="1cd60-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-145">publisher</span><span class="sxs-lookup"><span data-stu-id="1cd60-145">publisher</span></span>|<span data-ttu-id="1cd60-146">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-146">String</span></span>|<span data-ttu-id="1cd60-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd60-147">The publisher of the app.</span></span> <span data-ttu-id="1cd60-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1cd60-149">largeIcon</span></span>|[<span data-ttu-id="1cd60-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1cd60-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1cd60-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="1cd60-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1cd60-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd60-153">createdDateTime</span></span>|<span data-ttu-id="1cd60-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd60-154">DateTimeOffset</span></span>|<span data-ttu-id="1cd60-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd60-155">The date and time the app was created.</span></span> <span data-ttu-id="1cd60-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd60-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1cd60-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd60-158">DateTimeOffset</span></span>|<span data-ttu-id="1cd60-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd60-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1cd60-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1cd60-161">isFeatured</span></span>|<span data-ttu-id="1cd60-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cd60-162">Boolean</span></span>|<span data-ttu-id="1cd60-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1cd60-164">privacyInformationUrl</span></span>|<span data-ttu-id="1cd60-165">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-165">String</span></span>|<span data-ttu-id="1cd60-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="1cd60-166">The privacy statement Url.</span></span> <span data-ttu-id="1cd60-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1cd60-168">informationUrl</span></span>|<span data-ttu-id="1cd60-169">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-169">String</span></span>|<span data-ttu-id="1cd60-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="1cd60-170">The more information Url.</span></span> <span data-ttu-id="1cd60-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-172">owner</span><span class="sxs-lookup"><span data-stu-id="1cd60-172">owner</span></span>|<span data-ttu-id="1cd60-173">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-173">String</span></span>|<span data-ttu-id="1cd60-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd60-174">The owner of the app.</span></span> <span data-ttu-id="1cd60-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-176">developer</span><span class="sxs-lookup"><span data-stu-id="1cd60-176">developer</span></span>|<span data-ttu-id="1cd60-177">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-177">String</span></span>|<span data-ttu-id="1cd60-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd60-178">The developer of the app.</span></span> <span data-ttu-id="1cd60-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-180">notes</span><span class="sxs-lookup"><span data-stu-id="1cd60-180">notes</span></span>|<span data-ttu-id="1cd60-181">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-181">String</span></span>|<span data-ttu-id="1cd60-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd60-182">Notes for the app.</span></span> <span data-ttu-id="1cd60-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1cd60-184">uploadState</span></span>|<span data-ttu-id="1cd60-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1cd60-185">Int32</span></span>|<span data-ttu-id="1cd60-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="1cd60-186">The upload state.</span></span> <span data-ttu-id="1cd60-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="1cd60-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="1cd60-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="1cd60-189">publishingState</span></span>|[<span data-ttu-id="1cd60-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="1cd60-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1cd60-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd60-191">The publishing state for the app.</span></span> <span data-ttu-id="1cd60-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="1cd60-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1cd60-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="1cd60-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1cd60-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1cd60-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1cd60-195">isAssigned</span></span>|<span data-ttu-id="1cd60-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cd60-196">Boolean</span></span>|<span data-ttu-id="1cd60-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="1cd60-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1cd60-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1cd60-199">roleScopeTagIds</span></span>|<span data-ttu-id="1cd60-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1cd60-200">String collection</span></span>|<span data-ttu-id="1cd60-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd60-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1cd60-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="1cd60-203">dependentAppCount</span></span>|<span data-ttu-id="1cd60-204">Int32</span><span class="sxs-lookup"><span data-stu-id="1cd60-204">Int32</span></span>|<span data-ttu-id="1cd60-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd60-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="1cd60-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="1cd60-207">supersedingAppCount</span></span>|<span data-ttu-id="1cd60-208">Int32</span><span class="sxs-lookup"><span data-stu-id="1cd60-208">Int32</span></span>|<span data-ttu-id="1cd60-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="1cd60-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="1cd60-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="1cd60-211">supersededAppCount</span></span>|<span data-ttu-id="1cd60-212">Int32</span><span class="sxs-lookup"><span data-stu-id="1cd60-212">Int32</span></span>|<span data-ttu-id="1cd60-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="1cd60-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="1cd60-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1cd60-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1cd60-215">committedContentVersion</span></span>|<span data-ttu-id="1cd60-216">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-216">String</span></span>|<span data-ttu-id="1cd60-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="1cd60-217">The internal committed content version.</span></span> <span data-ttu-id="1cd60-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1cd60-219">fileName</span><span class="sxs-lookup"><span data-stu-id="1cd60-219">fileName</span></span>|<span data-ttu-id="1cd60-220">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-220">String</span></span>|<span data-ttu-id="1cd60-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="1cd60-221">The name of the main Lob application file.</span></span> <span data-ttu-id="1cd60-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1cd60-223">size</span><span class="sxs-lookup"><span data-stu-id="1cd60-223">size</span></span>|<span data-ttu-id="1cd60-224">Int64</span><span class="sxs-lookup"><span data-stu-id="1cd60-224">Int64</span></span>|<span data-ttu-id="1cd60-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="1cd60-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="1cd60-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1cd60-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1cd60-227">commandLine</span><span class="sxs-lookup"><span data-stu-id="1cd60-227">commandLine</span></span>|<span data-ttu-id="1cd60-228">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-228">String</span></span>|<span data-ttu-id="1cd60-229">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="1cd60-229">The command line.</span></span>|
|<span data-ttu-id="1cd60-230">productCode</span><span class="sxs-lookup"><span data-stu-id="1cd60-230">productCode</span></span>|<span data-ttu-id="1cd60-231">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-231">String</span></span>|<span data-ttu-id="1cd60-232">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="1cd60-232">The product code.</span></span>|
|<span data-ttu-id="1cd60-233">productVersion</span><span class="sxs-lookup"><span data-stu-id="1cd60-233">productVersion</span></span>|<span data-ttu-id="1cd60-234">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-234">String</span></span>|<span data-ttu-id="1cd60-235">Версия бизнес-приложения, к которому применяется MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="1cd60-235">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1cd60-236">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="1cd60-236">ignoreVersionDetection</span></span>|<span data-ttu-id="1cd60-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cd60-237">Boolean</span></span>|<span data-ttu-id="1cd60-238">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="1cd60-238">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="1cd60-239">Задайте значение true для бизнес-приложений MSI для Windows Mobile с функцией самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="1cd60-239">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="1cd60-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1cd60-240">identityVersion</span></span>|<span data-ttu-id="1cd60-241">String</span><span class="sxs-lookup"><span data-stu-id="1cd60-241">String</span></span>|<span data-ttu-id="1cd60-242">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="1cd60-242">The identity version.</span></span>|
|<span data-ttu-id="1cd60-243">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="1cd60-243">useDeviceContext</span></span>|<span data-ttu-id="1cd60-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cd60-244">Boolean</span></span>|<span data-ttu-id="1cd60-245">Указывает, следует ли установить MSI с двойным режимом в контексте устройства.</span><span class="sxs-lookup"><span data-stu-id="1cd60-245">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="1cd60-246">Если задано значение true, приложение будет установлено для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="1cd60-246">If true, app will be installed for all users.</span></span> <span data-ttu-id="1cd60-247">Если задано значение false, приложение будет установлено для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="1cd60-247">If false, app will be installed per-user.</span></span> <span data-ttu-id="1cd60-248">Если значение равно null, служба будет использовать стандартный контекст установки пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="1cd60-248">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="1cd60-249">В случае с двойным режимом MSI это значение по умолчанию будет иметь значение "на пользователя".</span><span class="sxs-lookup"><span data-stu-id="1cd60-249">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="1cd60-250">Не может быть задано для приложений с несдвоенным режимом.</span><span class="sxs-lookup"><span data-stu-id="1cd60-250">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="1cd60-251">После первоначального создания приложения его невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="1cd60-251">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="1cd60-252">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cd60-252">Response</span></span>
<span data-ttu-id="1cd60-253">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1cd60-253">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cd60-254">Пример</span><span class="sxs-lookup"><span data-stu-id="1cd60-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cd60-255">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cd60-255">Request</span></span>
<span data-ttu-id="1cd60-256">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cd60-256">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1123

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="1cd60-257">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cd60-257">Response</span></span>
<span data-ttu-id="1cd60-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1cd60-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1295

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```






