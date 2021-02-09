---
title: Создание windowsPhoneXAP
description: Создание объекта windowsPhoneXAP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae1418eacccdfeb9fedef34d28b1a8fb1c89e65a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157066"
---
# <a name="create-windowsphonexap"></a><span data-ttu-id="87de0-103">Создание windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="87de0-103">Create windowsPhoneXAP</span></span>

<span data-ttu-id="87de0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87de0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87de0-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87de0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87de0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87de0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87de0-107">Создание объекта [windowsPhoneXAP.](../resources/intune-apps-windowsphonexap.md)</span><span class="sxs-lookup"><span data-stu-id="87de0-107">Create a new [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87de0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="87de0-108">Prerequisites</span></span>
<span data-ttu-id="87de0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87de0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87de0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87de0-111">Permission type</span></span>|<span data-ttu-id="87de0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87de0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87de0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87de0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87de0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87de0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="87de0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87de0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87de0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87de0-116">Not supported.</span></span>|
|<span data-ttu-id="87de0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87de0-117">Application</span></span>|<span data-ttu-id="87de0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87de0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87de0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87de0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="87de0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87de0-120">Request headers</span></span>
|<span data-ttu-id="87de0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87de0-121">Header</span></span>|<span data-ttu-id="87de0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87de0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87de0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87de0-123">Authorization</span></span>|<span data-ttu-id="87de0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87de0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87de0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87de0-125">Accept</span></span>|<span data-ttu-id="87de0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87de0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87de0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87de0-127">Request body</span></span>
<span data-ttu-id="87de0-128">В теле запроса укажу представление объекта windowsPhoneXAP в JSON.</span><span class="sxs-lookup"><span data-stu-id="87de0-128">In the request body, supply a JSON representation for the windowsPhoneXAP object.</span></span>

<span data-ttu-id="87de0-129">В следующей таблице показаны свойства, необходимые при создании объекта windowsPhoneXAP.</span><span class="sxs-lookup"><span data-stu-id="87de0-129">The following table shows the properties that are required when you create the windowsPhoneXAP.</span></span>

|<span data-ttu-id="87de0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="87de0-130">Property</span></span>|<span data-ttu-id="87de0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="87de0-131">Type</span></span>|<span data-ttu-id="87de0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="87de0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87de0-133">id</span><span class="sxs-lookup"><span data-stu-id="87de0-133">id</span></span>|<span data-ttu-id="87de0-134">String</span><span class="sxs-lookup"><span data-stu-id="87de0-134">String</span></span>|<span data-ttu-id="87de0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="87de0-135">Key of the entity.</span></span> <span data-ttu-id="87de0-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="87de0-137">displayName</span></span>|<span data-ttu-id="87de0-138">String</span><span class="sxs-lookup"><span data-stu-id="87de0-138">String</span></span>|<span data-ttu-id="87de0-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="87de0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="87de0-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-141">description</span><span class="sxs-lookup"><span data-stu-id="87de0-141">description</span></span>|<span data-ttu-id="87de0-142">String</span><span class="sxs-lookup"><span data-stu-id="87de0-142">String</span></span>|<span data-ttu-id="87de0-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="87de0-143">The description of the app.</span></span> <span data-ttu-id="87de0-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-145">publisher</span><span class="sxs-lookup"><span data-stu-id="87de0-145">publisher</span></span>|<span data-ttu-id="87de0-146">String</span><span class="sxs-lookup"><span data-stu-id="87de0-146">String</span></span>|<span data-ttu-id="87de0-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="87de0-147">The publisher of the app.</span></span> <span data-ttu-id="87de0-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="87de0-149">largeIcon</span></span>|[<span data-ttu-id="87de0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="87de0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="87de0-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="87de0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="87de0-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87de0-153">createdDateTime</span></span>|<span data-ttu-id="87de0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87de0-154">DateTimeOffset</span></span>|<span data-ttu-id="87de0-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="87de0-155">The date and time the app was created.</span></span> <span data-ttu-id="87de0-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87de0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="87de0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87de0-158">DateTimeOffset</span></span>|<span data-ttu-id="87de0-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="87de0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="87de0-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="87de0-161">isFeatured</span></span>|<span data-ttu-id="87de0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="87de0-162">Boolean</span></span>|<span data-ttu-id="87de0-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="87de0-164">privacyInformationUrl</span></span>|<span data-ttu-id="87de0-165">String</span><span class="sxs-lookup"><span data-stu-id="87de0-165">String</span></span>|<span data-ttu-id="87de0-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="87de0-166">The privacy statement Url.</span></span> <span data-ttu-id="87de0-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="87de0-168">informationUrl</span></span>|<span data-ttu-id="87de0-169">String</span><span class="sxs-lookup"><span data-stu-id="87de0-169">String</span></span>|<span data-ttu-id="87de0-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="87de0-170">The more information Url.</span></span> <span data-ttu-id="87de0-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-172">owner</span><span class="sxs-lookup"><span data-stu-id="87de0-172">owner</span></span>|<span data-ttu-id="87de0-173">String</span><span class="sxs-lookup"><span data-stu-id="87de0-173">String</span></span>|<span data-ttu-id="87de0-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="87de0-174">The owner of the app.</span></span> <span data-ttu-id="87de0-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-176">developer</span><span class="sxs-lookup"><span data-stu-id="87de0-176">developer</span></span>|<span data-ttu-id="87de0-177">String</span><span class="sxs-lookup"><span data-stu-id="87de0-177">String</span></span>|<span data-ttu-id="87de0-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="87de0-178">The developer of the app.</span></span> <span data-ttu-id="87de0-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-180">notes</span><span class="sxs-lookup"><span data-stu-id="87de0-180">notes</span></span>|<span data-ttu-id="87de0-181">String</span><span class="sxs-lookup"><span data-stu-id="87de0-181">String</span></span>|<span data-ttu-id="87de0-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="87de0-182">Notes for the app.</span></span> <span data-ttu-id="87de0-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="87de0-184">uploadState</span></span>|<span data-ttu-id="87de0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="87de0-185">Int32</span></span>|<span data-ttu-id="87de0-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="87de0-186">The upload state.</span></span> <span data-ttu-id="87de0-187">Возможные значения: 0- `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="87de0-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="87de0-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="87de0-189">publishingState</span></span>|[<span data-ttu-id="87de0-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="87de0-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="87de0-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="87de0-191">The publishing state for the app.</span></span> <span data-ttu-id="87de0-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="87de0-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="87de0-193">Наследуется от [mobileApp.](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="87de0-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="87de0-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="87de0-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="87de0-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="87de0-195">isAssigned</span></span>|<span data-ttu-id="87de0-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="87de0-196">Boolean</span></span>|<span data-ttu-id="87de0-197">Значение, указывающее, назначено ли приложению хотя бы одна группа.</span><span class="sxs-lookup"><span data-stu-id="87de0-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="87de0-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="87de0-199">roleScopeTagIds</span></span>|<span data-ttu-id="87de0-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="87de0-200">String collection</span></span>|<span data-ttu-id="87de0-201">Список ид тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="87de0-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="87de0-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="87de0-203">dependentAppCount</span></span>|<span data-ttu-id="87de0-204">Int32</span><span class="sxs-lookup"><span data-stu-id="87de0-204">Int32</span></span>|<span data-ttu-id="87de0-205">Общее количество зависимостей, которые есть у этого приложения.</span><span class="sxs-lookup"><span data-stu-id="87de0-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="87de0-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="87de0-207">supersedingAppCount</span></span>|<span data-ttu-id="87de0-208">Int32</span><span class="sxs-lookup"><span data-stu-id="87de0-208">Int32</span></span>|<span data-ttu-id="87de0-209">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="87de0-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="87de0-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="87de0-211">supersededAppCount</span></span>|<span data-ttu-id="87de0-212">Int32</span><span class="sxs-lookup"><span data-stu-id="87de0-212">Int32</span></span>|<span data-ttu-id="87de0-213">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="87de0-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="87de0-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="87de0-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="87de0-215">committedContentVersion</span></span>|<span data-ttu-id="87de0-216">String</span><span class="sxs-lookup"><span data-stu-id="87de0-216">String</span></span>|<span data-ttu-id="87de0-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="87de0-217">The internal committed content version.</span></span> <span data-ttu-id="87de0-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="87de0-219">fileName</span><span class="sxs-lookup"><span data-stu-id="87de0-219">fileName</span></span>|<span data-ttu-id="87de0-220">String</span><span class="sxs-lookup"><span data-stu-id="87de0-220">String</span></span>|<span data-ttu-id="87de0-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="87de0-221">The name of the main Lob application file.</span></span> <span data-ttu-id="87de0-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="87de0-223">size</span><span class="sxs-lookup"><span data-stu-id="87de0-223">size</span></span>|<span data-ttu-id="87de0-224">Int64</span><span class="sxs-lookup"><span data-stu-id="87de0-224">Int64</span></span>|<span data-ttu-id="87de0-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="87de0-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="87de0-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="87de0-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="87de0-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="87de0-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="87de0-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="87de0-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="87de0-229">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="87de0-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="87de0-230">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="87de0-230">productIdentifier</span></span>|<span data-ttu-id="87de0-231">String</span><span class="sxs-lookup"><span data-stu-id="87de0-231">String</span></span>|<span data-ttu-id="87de0-232">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="87de0-232">The Product Identifier.</span></span>|
|<span data-ttu-id="87de0-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="87de0-233">identityVersion</span></span>|<span data-ttu-id="87de0-234">String</span><span class="sxs-lookup"><span data-stu-id="87de0-234">String</span></span>|<span data-ttu-id="87de0-235">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="87de0-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="87de0-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="87de0-236">Response</span></span>
<span data-ttu-id="87de0-237">В случае успеха этот метод возвращает код отклика и объект `201 Created` [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87de0-237">If successful, this method returns a `201 Created` response code and a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87de0-238">Пример</span><span class="sxs-lookup"><span data-stu-id="87de0-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="87de0-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="87de0-239">Request</span></span>
<span data-ttu-id="87de0-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87de0-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1340

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
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="87de0-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="87de0-241">Response</span></span>
<span data-ttu-id="87de0-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87de0-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1512

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
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```




