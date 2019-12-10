---
title: Обновление Макосмикрософтеджеапп
description: Обновление свойств объекта Макосмикрософтеджеапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b842106313d62bd2bf187cbc2f417524733a25af
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39925034"
---
# <a name="update-macosmicrosoftedgeapp"></a><span data-ttu-id="9f4d6-103">Обновление Макосмикрософтеджеапп</span><span class="sxs-lookup"><span data-stu-id="9f4d6-103">Update macOSMicrosoftEdgeApp</span></span>

> <span data-ttu-id="9f4d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f4d6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f4d6-106">Обновление свойств объекта [макосмикрософтеджеапп](../resources/intune-apps-macosmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9f4d6-106">Update the properties of a [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f4d6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f4d6-107">Prerequisites</span></span>
<span data-ttu-id="9f4d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f4d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f4d6-110">Permission type</span></span>|<span data-ttu-id="9f4d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f4d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f4d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f4d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f4d6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f4d6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9f4d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f4d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f4d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-115">Not supported.</span></span>|
|<span data-ttu-id="9f4d6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f4d6-116">Application</span></span>|<span data-ttu-id="9f4d6-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f4d6-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f4d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f4d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9f4d6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f4d6-119">Request headers</span></span>
|<span data-ttu-id="9f4d6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f4d6-120">Header</span></span>|<span data-ttu-id="9f4d6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9f4d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f4d6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f4d6-122">Authorization</span></span>|<span data-ttu-id="9f4d6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f4d6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9f4d6-124">Accept</span></span>|<span data-ttu-id="9f4d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f4d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f4d6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f4d6-126">Request body</span></span>
<span data-ttu-id="9f4d6-127">В тексте запроса добавьте представление объекта [макосмикрософтеджеапп](../resources/intune-apps-macosmicrosoftedgeapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-127">In the request body, supply a JSON representation for the [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object.</span></span>

<span data-ttu-id="9f4d6-128">В следующей таблице приведены свойства, необходимые при создании [макосмикрософтеджеапп](../resources/intune-apps-macosmicrosoftedgeapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-128">The following table shows the properties that are required when you create the [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md).</span></span>

|<span data-ttu-id="9f4d6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f4d6-129">Property</span></span>|<span data-ttu-id="9f4d6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9f4d6-130">Type</span></span>|<span data-ttu-id="9f4d6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9f4d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f4d6-132">id</span><span class="sxs-lookup"><span data-stu-id="9f4d6-132">id</span></span>|<span data-ttu-id="9f4d6-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9f4d6-133">String</span></span>|<span data-ttu-id="9f4d6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-134">Key of the entity.</span></span> <span data-ttu-id="9f4d6-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9f4d6-136">displayName</span></span>|<span data-ttu-id="9f4d6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9f4d6-137">String</span></span>|<span data-ttu-id="9f4d6-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9f4d6-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-140">description</span><span class="sxs-lookup"><span data-stu-id="9f4d6-140">description</span></span>|<span data-ttu-id="9f4d6-141">Строка</span><span class="sxs-lookup"><span data-stu-id="9f4d6-141">String</span></span>|<span data-ttu-id="9f4d6-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-142">The description of the app.</span></span> <span data-ttu-id="9f4d6-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9f4d6-144">publisher</span></span>|<span data-ttu-id="9f4d6-145">Строка</span><span class="sxs-lookup"><span data-stu-id="9f4d6-145">String</span></span>|<span data-ttu-id="9f4d6-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-146">The publisher of the app.</span></span> <span data-ttu-id="9f4d6-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9f4d6-148">largeIcon</span></span>|[<span data-ttu-id="9f4d6-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9f4d6-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9f4d6-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9f4d6-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f4d6-152">createdDateTime</span></span>|<span data-ttu-id="9f4d6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f4d6-153">DateTimeOffset</span></span>|<span data-ttu-id="9f4d6-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-154">The date and time the app was created.</span></span> <span data-ttu-id="9f4d6-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f4d6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9f4d6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f4d6-157">DateTimeOffset</span></span>|<span data-ttu-id="9f4d6-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9f4d6-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9f4d6-160">isFeatured</span></span>|<span data-ttu-id="9f4d6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f4d6-161">Boolean</span></span>|<span data-ttu-id="9f4d6-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9f4d6-163">privacyInformationUrl</span></span>|<span data-ttu-id="9f4d6-164">Строка</span><span class="sxs-lookup"><span data-stu-id="9f4d6-164">String</span></span>|<span data-ttu-id="9f4d6-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-165">The privacy statement Url.</span></span> <span data-ttu-id="9f4d6-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9f4d6-167">informationUrl</span></span>|<span data-ttu-id="9f4d6-168">Строка</span><span class="sxs-lookup"><span data-stu-id="9f4d6-168">String</span></span>|<span data-ttu-id="9f4d6-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-169">The more information Url.</span></span> <span data-ttu-id="9f4d6-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-171">owner</span><span class="sxs-lookup"><span data-stu-id="9f4d6-171">owner</span></span>|<span data-ttu-id="9f4d6-172">String</span><span class="sxs-lookup"><span data-stu-id="9f4d6-172">String</span></span>|<span data-ttu-id="9f4d6-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-173">The owner of the app.</span></span> <span data-ttu-id="9f4d6-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-175">developer</span><span class="sxs-lookup"><span data-stu-id="9f4d6-175">developer</span></span>|<span data-ttu-id="9f4d6-176">Строка</span><span class="sxs-lookup"><span data-stu-id="9f4d6-176">String</span></span>|<span data-ttu-id="9f4d6-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-177">The developer of the app.</span></span> <span data-ttu-id="9f4d6-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-179">notes</span><span class="sxs-lookup"><span data-stu-id="9f4d6-179">notes</span></span>|<span data-ttu-id="9f4d6-180">String</span><span class="sxs-lookup"><span data-stu-id="9f4d6-180">String</span></span>|<span data-ttu-id="9f4d6-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-181">Notes for the app.</span></span> <span data-ttu-id="9f4d6-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9f4d6-183">uploadState</span></span>|<span data-ttu-id="9f4d6-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9f4d6-184">Int32</span></span>|<span data-ttu-id="9f4d6-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-185">The upload state.</span></span> <span data-ttu-id="9f4d6-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9f4d6-187">publishingState</span></span>|[<span data-ttu-id="9f4d6-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9f4d6-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9f4d6-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-189">The publishing state for the app.</span></span> <span data-ttu-id="9f4d6-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9f4d6-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="9f4d6-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9f4d6-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9f4d6-193">isAssigned</span></span>|<span data-ttu-id="9f4d6-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f4d6-194">Boolean</span></span>|<span data-ttu-id="9f4d6-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9f4d6-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f4d6-197">roleScopeTagIds</span></span>|<span data-ttu-id="9f4d6-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9f4d6-198">String collection</span></span>|<span data-ttu-id="9f4d6-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9f4d6-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="9f4d6-201">dependentAppCount</span></span>|<span data-ttu-id="9f4d6-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9f4d6-202">Int32</span></span>|<span data-ttu-id="9f4d6-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9f4d6-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f4d6-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f4d6-205">оптоволокон</span><span class="sxs-lookup"><span data-stu-id="9f4d6-205">channel</span></span>|[<span data-ttu-id="9f4d6-206">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="9f4d6-206">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="9f4d6-207">Канал, который необходимо установить на целевые устройства.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-207">The channel to install on target devices.</span></span> <span data-ttu-id="9f4d6-208">Возможные значения: `dev`, `beta`, `stable`.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-208">Possible values are: `dev`, `beta`, `stable`.</span></span>|



## <a name="response"></a><span data-ttu-id="9f4d6-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f4d6-209">Response</span></span>
<span data-ttu-id="9f4d6-210">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосмикрософтеджеапп](../resources/intune-apps-macosmicrosoftedgeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-210">If successful, this method returns a `200 OK` response code and an updated [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f4d6-211">Пример</span><span class="sxs-lookup"><span data-stu-id="9f4d6-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f4d6-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f4d6-212">Request</span></span>
<span data-ttu-id="9f4d6-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 742

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
  "channel": "beta"
}
```

### <a name="response"></a><span data-ttu-id="9f4d6-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f4d6-214">Response</span></span>
<span data-ttu-id="9f4d6-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f4d6-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

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
  "channel": "beta"
}
```





