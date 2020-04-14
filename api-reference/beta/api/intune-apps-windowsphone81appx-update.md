---
title: Обновление windowsPhone81AppX
description: Обновление свойств объекта windowsPhone81AppX.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 562df1bb46ad7ea0a82a43de5b21c65aade0ae50
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43409282"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="2ad7d-103">Обновление windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="2ad7d-103">Update windowsPhone81AppX</span></span>

<span data-ttu-id="2ad7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ad7d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ad7d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ad7d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ad7d-107">Обновление свойств объекта [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="2ad7d-107">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ad7d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2ad7d-108">Prerequisites</span></span>
<span data-ttu-id="2ad7d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ad7d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ad7d-111">Permission type</span></span>|<span data-ttu-id="2ad7d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ad7d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ad7d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ad7d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ad7d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ad7d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2ad7d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ad7d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ad7d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-116">Not supported.</span></span>|
|<span data-ttu-id="2ad7d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2ad7d-117">Application</span></span>|<span data-ttu-id="2ad7d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ad7d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ad7d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ad7d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="2ad7d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2ad7d-120">Request headers</span></span>
|<span data-ttu-id="2ad7d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ad7d-121">Header</span></span>|<span data-ttu-id="2ad7d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2ad7d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ad7d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ad7d-123">Authorization</span></span>|<span data-ttu-id="2ad7d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ad7d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2ad7d-125">Accept</span></span>|<span data-ttu-id="2ad7d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ad7d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ad7d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ad7d-127">Request body</span></span>
<span data-ttu-id="2ad7d-128">В тексте запроса добавьте представление объекта [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-128">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="2ad7d-129">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-129">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="2ad7d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ad7d-130">Property</span></span>|<span data-ttu-id="2ad7d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2ad7d-131">Type</span></span>|<span data-ttu-id="2ad7d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2ad7d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ad7d-133">id</span><span class="sxs-lookup"><span data-stu-id="2ad7d-133">id</span></span>|<span data-ttu-id="2ad7d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2ad7d-134">String</span></span>|<span data-ttu-id="2ad7d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-135">Key of the entity.</span></span> <span data-ttu-id="2ad7d-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2ad7d-137">displayName</span></span>|<span data-ttu-id="2ad7d-138">Строка</span><span class="sxs-lookup"><span data-stu-id="2ad7d-138">String</span></span>|<span data-ttu-id="2ad7d-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2ad7d-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-141">description</span><span class="sxs-lookup"><span data-stu-id="2ad7d-141">description</span></span>|<span data-ttu-id="2ad7d-142">Строка</span><span class="sxs-lookup"><span data-stu-id="2ad7d-142">String</span></span>|<span data-ttu-id="2ad7d-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-143">The description of the app.</span></span> <span data-ttu-id="2ad7d-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-145">publisher</span><span class="sxs-lookup"><span data-stu-id="2ad7d-145">publisher</span></span>|<span data-ttu-id="2ad7d-146">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-146">String</span></span>|<span data-ttu-id="2ad7d-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-147">The publisher of the app.</span></span> <span data-ttu-id="2ad7d-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2ad7d-149">largeIcon</span></span>|[<span data-ttu-id="2ad7d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2ad7d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2ad7d-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2ad7d-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad7d-153">createdDateTime</span></span>|<span data-ttu-id="2ad7d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad7d-154">DateTimeOffset</span></span>|<span data-ttu-id="2ad7d-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-155">The date and time the app was created.</span></span> <span data-ttu-id="2ad7d-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad7d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="2ad7d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad7d-158">DateTimeOffset</span></span>|<span data-ttu-id="2ad7d-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="2ad7d-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2ad7d-161">isFeatured</span></span>|<span data-ttu-id="2ad7d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad7d-162">Boolean</span></span>|<span data-ttu-id="2ad7d-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2ad7d-164">privacyInformationUrl</span></span>|<span data-ttu-id="2ad7d-165">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-165">String</span></span>|<span data-ttu-id="2ad7d-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-166">The privacy statement Url.</span></span> <span data-ttu-id="2ad7d-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2ad7d-168">informationUrl</span></span>|<span data-ttu-id="2ad7d-169">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-169">String</span></span>|<span data-ttu-id="2ad7d-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-170">The more information Url.</span></span> <span data-ttu-id="2ad7d-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-172">owner</span><span class="sxs-lookup"><span data-stu-id="2ad7d-172">owner</span></span>|<span data-ttu-id="2ad7d-173">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-173">String</span></span>|<span data-ttu-id="2ad7d-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-174">The owner of the app.</span></span> <span data-ttu-id="2ad7d-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-176">developer</span><span class="sxs-lookup"><span data-stu-id="2ad7d-176">developer</span></span>|<span data-ttu-id="2ad7d-177">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-177">String</span></span>|<span data-ttu-id="2ad7d-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-178">The developer of the app.</span></span> <span data-ttu-id="2ad7d-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-180">notes</span><span class="sxs-lookup"><span data-stu-id="2ad7d-180">notes</span></span>|<span data-ttu-id="2ad7d-181">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-181">String</span></span>|<span data-ttu-id="2ad7d-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-182">Notes for the app.</span></span> <span data-ttu-id="2ad7d-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="2ad7d-184">uploadState</span></span>|<span data-ttu-id="2ad7d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad7d-185">Int32</span></span>|<span data-ttu-id="2ad7d-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-186">The upload state.</span></span> <span data-ttu-id="2ad7d-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="2ad7d-188">publishingState</span></span>|[<span data-ttu-id="2ad7d-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="2ad7d-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2ad7d-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-190">The publishing state for the app.</span></span> <span data-ttu-id="2ad7d-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2ad7d-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="2ad7d-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2ad7d-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2ad7d-194">isAssigned</span></span>|<span data-ttu-id="2ad7d-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ad7d-195">Boolean</span></span>|<span data-ttu-id="2ad7d-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2ad7d-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2ad7d-198">roleScopeTagIds</span></span>|<span data-ttu-id="2ad7d-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-199">String collection</span></span>|<span data-ttu-id="2ad7d-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2ad7d-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="2ad7d-202">dependentAppCount</span></span>|<span data-ttu-id="2ad7d-203">Int32</span><span class="sxs-lookup"><span data-stu-id="2ad7d-203">Int32</span></span>|<span data-ttu-id="2ad7d-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="2ad7d-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2ad7d-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2ad7d-206">committedContentVersion</span></span>|<span data-ttu-id="2ad7d-207">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-207">String</span></span>|<span data-ttu-id="2ad7d-208">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-208">The internal committed content version.</span></span> <span data-ttu-id="2ad7d-209">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2ad7d-210">fileName</span><span class="sxs-lookup"><span data-stu-id="2ad7d-210">fileName</span></span>|<span data-ttu-id="2ad7d-211">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-211">String</span></span>|<span data-ttu-id="2ad7d-212">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-212">The name of the main Lob application file.</span></span> <span data-ttu-id="2ad7d-213">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2ad7d-214">size</span><span class="sxs-lookup"><span data-stu-id="2ad7d-214">size</span></span>|<span data-ttu-id="2ad7d-215">Int64</span><span class="sxs-lookup"><span data-stu-id="2ad7d-215">Int64</span></span>|<span data-ttu-id="2ad7d-216">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="2ad7d-217">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ad7d-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2ad7d-218">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="2ad7d-218">applicableArchitectures</span></span>|[<span data-ttu-id="2ad7d-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="2ad7d-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="2ad7d-220">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-220">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="2ad7d-221">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="2ad7d-222">identityName</span><span class="sxs-lookup"><span data-stu-id="2ad7d-222">identityName</span></span>|<span data-ttu-id="2ad7d-223">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-223">String</span></span>|<span data-ttu-id="2ad7d-224">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-224">The Identity Name.</span></span>|
|<span data-ttu-id="2ad7d-225">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="2ad7d-225">identityPublisherHash</span></span>|<span data-ttu-id="2ad7d-226">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-226">String</span></span>|<span data-ttu-id="2ad7d-227">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-227">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="2ad7d-228">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2ad7d-228">identityResourceIdentifier</span></span>|<span data-ttu-id="2ad7d-229">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-229">String</span></span>|<span data-ttu-id="2ad7d-230">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-230">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="2ad7d-231">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2ad7d-231">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2ad7d-232">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2ad7d-232">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="2ad7d-233">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-233">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2ad7d-234">фонепродуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="2ad7d-234">phoneProductIdentifier</span></span>|<span data-ttu-id="2ad7d-235">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-235">String</span></span>|<span data-ttu-id="2ad7d-236">Идентификатор телефонного продукта.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-236">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="2ad7d-237">фонепублишерид</span><span class="sxs-lookup"><span data-stu-id="2ad7d-237">phonePublisherId</span></span>|<span data-ttu-id="2ad7d-238">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-238">String</span></span>|<span data-ttu-id="2ad7d-239">Идентификатор издателя телефона.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-239">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="2ad7d-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="2ad7d-240">identityVersion</span></span>|<span data-ttu-id="2ad7d-241">String</span><span class="sxs-lookup"><span data-stu-id="2ad7d-241">String</span></span>|<span data-ttu-id="2ad7d-242">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="2ad7d-243">Ответ</span><span class="sxs-lookup"><span data-stu-id="2ad7d-243">Response</span></span>
<span data-ttu-id="2ad7d-244">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-244">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ad7d-245">Пример</span><span class="sxs-lookup"><span data-stu-id="2ad7d-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ad7d-246">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ad7d-246">Request</span></span>
<span data-ttu-id="2ad7d-247">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1513

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="2ad7d-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ad7d-248">Response</span></span>
<span data-ttu-id="2ad7d-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ad7d-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1685

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
  "identityVersion": "Identity Version value"
}
```



