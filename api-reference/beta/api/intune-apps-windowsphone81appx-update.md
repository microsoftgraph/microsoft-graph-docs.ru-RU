---
title: Обновление windowsPhone81AppX
description: Обновление свойств объекта windowsPhone81AppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc367988329a65d0f71e8bc894ed45bab3c11de0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39933281"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="32a3f-103">Обновление windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="32a3f-103">Update windowsPhone81AppX</span></span>

> <span data-ttu-id="32a3f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32a3f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32a3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32a3f-106">Обновление свойств объекта [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="32a3f-106">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32a3f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="32a3f-107">Prerequisites</span></span>
<span data-ttu-id="32a3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32a3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32a3f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32a3f-110">Permission type</span></span>|<span data-ttu-id="32a3f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32a3f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32a3f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32a3f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32a3f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32a3f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32a3f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32a3f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32a3f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32a3f-115">Not supported.</span></span>|
|<span data-ttu-id="32a3f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32a3f-116">Application</span></span>|<span data-ttu-id="32a3f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32a3f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32a3f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32a3f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="32a3f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="32a3f-119">Request headers</span></span>
|<span data-ttu-id="32a3f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32a3f-120">Header</span></span>|<span data-ttu-id="32a3f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="32a3f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32a3f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32a3f-122">Authorization</span></span>|<span data-ttu-id="32a3f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32a3f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32a3f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="32a3f-124">Accept</span></span>|<span data-ttu-id="32a3f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32a3f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32a3f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32a3f-126">Request body</span></span>
<span data-ttu-id="32a3f-127">В тексте запроса добавьте представление объекта [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32a3f-127">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="32a3f-128">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-128">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="32a3f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="32a3f-129">Property</span></span>|<span data-ttu-id="32a3f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="32a3f-130">Type</span></span>|<span data-ttu-id="32a3f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="32a3f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32a3f-132">id</span><span class="sxs-lookup"><span data-stu-id="32a3f-132">id</span></span>|<span data-ttu-id="32a3f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-133">String</span></span>|<span data-ttu-id="32a3f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="32a3f-134">Key of the entity.</span></span> <span data-ttu-id="32a3f-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="32a3f-136">displayName</span></span>|<span data-ttu-id="32a3f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-137">String</span></span>|<span data-ttu-id="32a3f-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="32a3f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="32a3f-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-140">description</span><span class="sxs-lookup"><span data-stu-id="32a3f-140">description</span></span>|<span data-ttu-id="32a3f-141">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-141">String</span></span>|<span data-ttu-id="32a3f-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-142">The description of the app.</span></span> <span data-ttu-id="32a3f-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-144">publisher</span><span class="sxs-lookup"><span data-stu-id="32a3f-144">publisher</span></span>|<span data-ttu-id="32a3f-145">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-145">String</span></span>|<span data-ttu-id="32a3f-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-146">The publisher of the app.</span></span> <span data-ttu-id="32a3f-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="32a3f-148">largeIcon</span></span>|[<span data-ttu-id="32a3f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="32a3f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="32a3f-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="32a3f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="32a3f-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32a3f-152">createdDateTime</span></span>|<span data-ttu-id="32a3f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32a3f-153">DateTimeOffset</span></span>|<span data-ttu-id="32a3f-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-154">The date and time the app was created.</span></span> <span data-ttu-id="32a3f-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32a3f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="32a3f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32a3f-157">DateTimeOffset</span></span>|<span data-ttu-id="32a3f-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="32a3f-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="32a3f-160">isFeatured</span></span>|<span data-ttu-id="32a3f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="32a3f-161">Boolean</span></span>|<span data-ttu-id="32a3f-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="32a3f-163">privacyInformationUrl</span></span>|<span data-ttu-id="32a3f-164">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-164">String</span></span>|<span data-ttu-id="32a3f-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="32a3f-165">The privacy statement Url.</span></span> <span data-ttu-id="32a3f-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="32a3f-167">informationUrl</span></span>|<span data-ttu-id="32a3f-168">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-168">String</span></span>|<span data-ttu-id="32a3f-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="32a3f-169">The more information Url.</span></span> <span data-ttu-id="32a3f-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-171">owner</span><span class="sxs-lookup"><span data-stu-id="32a3f-171">owner</span></span>|<span data-ttu-id="32a3f-172">String</span><span class="sxs-lookup"><span data-stu-id="32a3f-172">String</span></span>|<span data-ttu-id="32a3f-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-173">The owner of the app.</span></span> <span data-ttu-id="32a3f-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-175">developer</span><span class="sxs-lookup"><span data-stu-id="32a3f-175">developer</span></span>|<span data-ttu-id="32a3f-176">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-176">String</span></span>|<span data-ttu-id="32a3f-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-177">The developer of the app.</span></span> <span data-ttu-id="32a3f-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-179">notes</span><span class="sxs-lookup"><span data-stu-id="32a3f-179">notes</span></span>|<span data-ttu-id="32a3f-180">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-180">String</span></span>|<span data-ttu-id="32a3f-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-181">Notes for the app.</span></span> <span data-ttu-id="32a3f-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="32a3f-183">uploadState</span></span>|<span data-ttu-id="32a3f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="32a3f-184">Int32</span></span>|<span data-ttu-id="32a3f-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="32a3f-185">The upload state.</span></span> <span data-ttu-id="32a3f-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="32a3f-187">publishingState</span></span>|[<span data-ttu-id="32a3f-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="32a3f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="32a3f-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-189">The publishing state for the app.</span></span> <span data-ttu-id="32a3f-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="32a3f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="32a3f-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="32a3f-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="32a3f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="32a3f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="32a3f-193">isAssigned</span></span>|<span data-ttu-id="32a3f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="32a3f-194">Boolean</span></span>|<span data-ttu-id="32a3f-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="32a3f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="32a3f-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="32a3f-197">roleScopeTagIds</span></span>|<span data-ttu-id="32a3f-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="32a3f-198">String collection</span></span>|<span data-ttu-id="32a3f-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="32a3f-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="32a3f-201">dependentAppCount</span></span>|<span data-ttu-id="32a3f-202">Int32</span><span class="sxs-lookup"><span data-stu-id="32a3f-202">Int32</span></span>|<span data-ttu-id="32a3f-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="32a3f-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32a3f-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="32a3f-205">committedContentVersion</span></span>|<span data-ttu-id="32a3f-206">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-206">String</span></span>|<span data-ttu-id="32a3f-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="32a3f-207">The internal committed content version.</span></span> <span data-ttu-id="32a3f-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="32a3f-209">fileName</span><span class="sxs-lookup"><span data-stu-id="32a3f-209">fileName</span></span>|<span data-ttu-id="32a3f-210">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-210">String</span></span>|<span data-ttu-id="32a3f-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-211">The name of the main Lob application file.</span></span> <span data-ttu-id="32a3f-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="32a3f-213">size</span><span class="sxs-lookup"><span data-stu-id="32a3f-213">size</span></span>|<span data-ttu-id="32a3f-214">Int64</span><span class="sxs-lookup"><span data-stu-id="32a3f-214">Int64</span></span>|<span data-ttu-id="32a3f-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="32a3f-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="32a3f-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="32a3f-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="32a3f-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="32a3f-217">applicableArchitectures</span></span>|[<span data-ttu-id="32a3f-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="32a3f-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="32a3f-219">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="32a3f-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="32a3f-220">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="32a3f-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="32a3f-221">identityName</span><span class="sxs-lookup"><span data-stu-id="32a3f-221">identityName</span></span>|<span data-ttu-id="32a3f-222">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-222">String</span></span>|<span data-ttu-id="32a3f-223">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-223">The Identity Name.</span></span>|
|<span data-ttu-id="32a3f-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="32a3f-224">identityPublisherHash</span></span>|<span data-ttu-id="32a3f-225">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-225">String</span></span>|<span data-ttu-id="32a3f-226">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="32a3f-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="32a3f-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="32a3f-227">identityResourceIdentifier</span></span>|<span data-ttu-id="32a3f-228">String</span><span class="sxs-lookup"><span data-stu-id="32a3f-228">String</span></span>|<span data-ttu-id="32a3f-229">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="32a3f-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="32a3f-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="32a3f-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="32a3f-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="32a3f-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="32a3f-232">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="32a3f-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="32a3f-233">фонепродуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="32a3f-233">phoneProductIdentifier</span></span>|<span data-ttu-id="32a3f-234">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-234">String</span></span>|<span data-ttu-id="32a3f-235">Идентификатор телефонного продукта.</span><span class="sxs-lookup"><span data-stu-id="32a3f-235">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="32a3f-236">фонепублишерид</span><span class="sxs-lookup"><span data-stu-id="32a3f-236">phonePublisherId</span></span>|<span data-ttu-id="32a3f-237">Строка</span><span class="sxs-lookup"><span data-stu-id="32a3f-237">String</span></span>|<span data-ttu-id="32a3f-238">Идентификатор издателя телефона.</span><span class="sxs-lookup"><span data-stu-id="32a3f-238">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="32a3f-239">identityVersion</span><span class="sxs-lookup"><span data-stu-id="32a3f-239">identityVersion</span></span>|<span data-ttu-id="32a3f-240">String</span><span class="sxs-lookup"><span data-stu-id="32a3f-240">String</span></span>|<span data-ttu-id="32a3f-241">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="32a3f-241">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="32a3f-242">Ответ</span><span class="sxs-lookup"><span data-stu-id="32a3f-242">Response</span></span>
<span data-ttu-id="32a3f-243">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32a3f-243">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32a3f-244">Пример</span><span class="sxs-lookup"><span data-stu-id="32a3f-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="32a3f-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="32a3f-245">Request</span></span>
<span data-ttu-id="32a3f-246">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32a3f-246">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="32a3f-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="32a3f-247">Response</span></span>
<span data-ttu-id="32a3f-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32a3f-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





