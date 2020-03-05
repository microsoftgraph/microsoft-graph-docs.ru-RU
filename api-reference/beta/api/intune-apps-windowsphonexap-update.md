---
title: Обновление Виндовсфонексап
description: Обновление свойств объекта Виндовсфонексап.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3128660e45d2dfc055e8545298256f5b2201e121
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444709"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="7dd7f-103">Обновление Виндовсфонексап</span><span class="sxs-lookup"><span data-stu-id="7dd7f-103">Update windowsPhoneXAP</span></span>

<span data-ttu-id="7dd7f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7dd7f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7dd7f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dd7f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dd7f-107">Обновление свойств объекта [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="7dd7f-107">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dd7f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7dd7f-108">Prerequisites</span></span>
<span data-ttu-id="7dd7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dd7f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dd7f-111">Permission type</span></span>|<span data-ttu-id="7dd7f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dd7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dd7f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dd7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7dd7f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dd7f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7dd7f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dd7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dd7f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-116">Not supported.</span></span>|
|<span data-ttu-id="7dd7f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dd7f-117">Application</span></span>|<span data-ttu-id="7dd7f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dd7f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dd7f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7dd7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="7dd7f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7dd7f-120">Request headers</span></span>
|<span data-ttu-id="7dd7f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7dd7f-121">Header</span></span>|<span data-ttu-id="7dd7f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7dd7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dd7f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dd7f-123">Authorization</span></span>|<span data-ttu-id="7dd7f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dd7f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7dd7f-125">Accept</span></span>|<span data-ttu-id="7dd7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7dd7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dd7f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7dd7f-127">Request body</span></span>
<span data-ttu-id="7dd7f-128">В тексте запроса добавьте представление объекта [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-128">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="7dd7f-129">В следующей таблице приведены свойства, необходимые при создании [виндовсфонексап](../resources/intune-apps-windowsphonexap.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-129">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="7dd7f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7dd7f-130">Property</span></span>|<span data-ttu-id="7dd7f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7dd7f-131">Type</span></span>|<span data-ttu-id="7dd7f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7dd7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dd7f-133">id</span><span class="sxs-lookup"><span data-stu-id="7dd7f-133">id</span></span>|<span data-ttu-id="7dd7f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7dd7f-134">String</span></span>|<span data-ttu-id="7dd7f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-135">Key of the entity.</span></span> <span data-ttu-id="7dd7f-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7dd7f-137">displayName</span></span>|<span data-ttu-id="7dd7f-138">Строка</span><span class="sxs-lookup"><span data-stu-id="7dd7f-138">String</span></span>|<span data-ttu-id="7dd7f-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7dd7f-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-141">description</span><span class="sxs-lookup"><span data-stu-id="7dd7f-141">description</span></span>|<span data-ttu-id="7dd7f-142">Строка</span><span class="sxs-lookup"><span data-stu-id="7dd7f-142">String</span></span>|<span data-ttu-id="7dd7f-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-143">The description of the app.</span></span> <span data-ttu-id="7dd7f-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="7dd7f-145">publisher</span></span>|<span data-ttu-id="7dd7f-146">String</span><span class="sxs-lookup"><span data-stu-id="7dd7f-146">String</span></span>|<span data-ttu-id="7dd7f-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-147">The publisher of the app.</span></span> <span data-ttu-id="7dd7f-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7dd7f-149">largeIcon</span></span>|[<span data-ttu-id="7dd7f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7dd7f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7dd7f-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7dd7f-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dd7f-153">createdDateTime</span></span>|<span data-ttu-id="7dd7f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dd7f-154">DateTimeOffset</span></span>|<span data-ttu-id="7dd7f-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-155">The date and time the app was created.</span></span> <span data-ttu-id="7dd7f-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7dd7f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7dd7f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dd7f-158">DateTimeOffset</span></span>|<span data-ttu-id="7dd7f-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="7dd7f-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7dd7f-161">isFeatured</span></span>|<span data-ttu-id="7dd7f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dd7f-162">Boolean</span></span>|<span data-ttu-id="7dd7f-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7dd7f-164">privacyInformationUrl</span></span>|<span data-ttu-id="7dd7f-165">String</span><span class="sxs-lookup"><span data-stu-id="7dd7f-165">String</span></span>|<span data-ttu-id="7dd7f-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-166">The privacy statement Url.</span></span> <span data-ttu-id="7dd7f-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7dd7f-168">informationUrl</span></span>|<span data-ttu-id="7dd7f-169">String</span><span class="sxs-lookup"><span data-stu-id="7dd7f-169">String</span></span>|<span data-ttu-id="7dd7f-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-170">The more information Url.</span></span> <span data-ttu-id="7dd7f-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-172">owner</span><span class="sxs-lookup"><span data-stu-id="7dd7f-172">owner</span></span>|<span data-ttu-id="7dd7f-173">String</span><span class="sxs-lookup"><span data-stu-id="7dd7f-173">String</span></span>|<span data-ttu-id="7dd7f-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-174">The owner of the app.</span></span> <span data-ttu-id="7dd7f-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-176">developer</span><span class="sxs-lookup"><span data-stu-id="7dd7f-176">developer</span></span>|<span data-ttu-id="7dd7f-177">String</span><span class="sxs-lookup"><span data-stu-id="7dd7f-177">String</span></span>|<span data-ttu-id="7dd7f-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-178">The developer of the app.</span></span> <span data-ttu-id="7dd7f-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-180">notes</span><span class="sxs-lookup"><span data-stu-id="7dd7f-180">notes</span></span>|<span data-ttu-id="7dd7f-181">String</span><span class="sxs-lookup"><span data-stu-id="7dd7f-181">String</span></span>|<span data-ttu-id="7dd7f-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-182">Notes for the app.</span></span> <span data-ttu-id="7dd7f-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="7dd7f-184">uploadState</span></span>|<span data-ttu-id="7dd7f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7dd7f-185">Int32</span></span>|<span data-ttu-id="7dd7f-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-186">The upload state.</span></span> <span data-ttu-id="7dd7f-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="7dd7f-188">publishingState</span></span>|[<span data-ttu-id="7dd7f-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="7dd7f-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7dd7f-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-190">The publishing state for the app.</span></span> <span data-ttu-id="7dd7f-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7dd7f-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="7dd7f-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7dd7f-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7dd7f-194">isAssigned</span></span>|<span data-ttu-id="7dd7f-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dd7f-195">Boolean</span></span>|<span data-ttu-id="7dd7f-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7dd7f-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7dd7f-198">roleScopeTagIds</span></span>|<span data-ttu-id="7dd7f-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7dd7f-199">String collection</span></span>|<span data-ttu-id="7dd7f-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7dd7f-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="7dd7f-202">dependentAppCount</span></span>|<span data-ttu-id="7dd7f-203">Int32</span><span class="sxs-lookup"><span data-stu-id="7dd7f-203">Int32</span></span>|<span data-ttu-id="7dd7f-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7dd7f-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7dd7f-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7dd7f-206">committedContentVersion</span></span>|<span data-ttu-id="7dd7f-207">String</span><span class="sxs-lookup"><span data-stu-id="7dd7f-207">String</span></span>|<span data-ttu-id="7dd7f-208">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-208">The internal committed content version.</span></span> <span data-ttu-id="7dd7f-209">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7dd7f-210">fileName</span><span class="sxs-lookup"><span data-stu-id="7dd7f-210">fileName</span></span>|<span data-ttu-id="7dd7f-211">String</span><span class="sxs-lookup"><span data-stu-id="7dd7f-211">String</span></span>|<span data-ttu-id="7dd7f-212">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-212">The name of the main Lob application file.</span></span> <span data-ttu-id="7dd7f-213">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7dd7f-214">size</span><span class="sxs-lookup"><span data-stu-id="7dd7f-214">size</span></span>|<span data-ttu-id="7dd7f-215">Int64</span><span class="sxs-lookup"><span data-stu-id="7dd7f-215">Int64</span></span>|<span data-ttu-id="7dd7f-216">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="7dd7f-217">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7dd7f-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7dd7f-218">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7dd7f-218">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7dd7f-219">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7dd7f-219">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="7dd7f-220">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-220">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="7dd7f-221">продуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="7dd7f-221">productIdentifier</span></span>|<span data-ttu-id="7dd7f-222">String</span><span class="sxs-lookup"><span data-stu-id="7dd7f-222">String</span></span>|<span data-ttu-id="7dd7f-223">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-223">The Product Identifier.</span></span>|
|<span data-ttu-id="7dd7f-224">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7dd7f-224">identityVersion</span></span>|<span data-ttu-id="7dd7f-225">String</span><span class="sxs-lookup"><span data-stu-id="7dd7f-225">String</span></span>|<span data-ttu-id="7dd7f-226">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-226">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="7dd7f-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="7dd7f-227">Response</span></span>
<span data-ttu-id="7dd7f-228">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-228">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dd7f-229">Пример</span><span class="sxs-lookup"><span data-stu-id="7dd7f-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dd7f-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dd7f-230">Request</span></span>
<span data-ttu-id="7dd7f-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1237

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

### <a name="response"></a><span data-ttu-id="7dd7f-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dd7f-232">Response</span></span>
<span data-ttu-id="7dd7f-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7dd7f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1409

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





