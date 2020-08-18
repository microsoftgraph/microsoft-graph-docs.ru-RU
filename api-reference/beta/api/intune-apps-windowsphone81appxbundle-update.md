---
title: Обновление windowsPhone81AppXBundle
description: Обновление свойств объекта windowsPhone81AppXBundle.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: afa3e85f90720977efe71b67f28c09e4c6485855
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790961"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="0d265-103">Обновление windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="0d265-103">Update windowsPhone81AppXBundle</span></span>

<span data-ttu-id="0d265-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d265-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d265-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d265-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d265-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d265-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d265-107">Обновление свойств объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="0d265-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d265-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0d265-108">Prerequisites</span></span>
<span data-ttu-id="0d265-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d265-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d265-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d265-111">Permission type</span></span>|<span data-ttu-id="0d265-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d265-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d265-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d265-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0d265-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d265-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0d265-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d265-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d265-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d265-116">Not supported.</span></span>|
|<span data-ttu-id="0d265-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0d265-117">Application</span></span>|<span data-ttu-id="0d265-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d265-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d265-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d265-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="0d265-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0d265-120">Request headers</span></span>
|<span data-ttu-id="0d265-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d265-121">Header</span></span>|<span data-ttu-id="0d265-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0d265-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d265-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d265-123">Authorization</span></span>|<span data-ttu-id="0d265-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d265-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d265-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0d265-125">Accept</span></span>|<span data-ttu-id="0d265-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0d265-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d265-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d265-127">Request body</span></span>
<span data-ttu-id="0d265-128">В тексте запроса добавьте представление объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d265-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="0d265-129">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="0d265-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d265-130">Property</span></span>|<span data-ttu-id="0d265-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0d265-131">Type</span></span>|<span data-ttu-id="0d265-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0d265-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d265-133">id</span><span class="sxs-lookup"><span data-stu-id="0d265-133">id</span></span>|<span data-ttu-id="0d265-134">String</span><span class="sxs-lookup"><span data-stu-id="0d265-134">String</span></span>|<span data-ttu-id="0d265-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0d265-135">Key of the entity.</span></span> <span data-ttu-id="0d265-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0d265-137">displayName</span></span>|<span data-ttu-id="0d265-138">String</span><span class="sxs-lookup"><span data-stu-id="0d265-138">String</span></span>|<span data-ttu-id="0d265-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="0d265-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0d265-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-141">description</span><span class="sxs-lookup"><span data-stu-id="0d265-141">description</span></span>|<span data-ttu-id="0d265-142">String</span><span class="sxs-lookup"><span data-stu-id="0d265-142">String</span></span>|<span data-ttu-id="0d265-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="0d265-143">The description of the app.</span></span> <span data-ttu-id="0d265-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-145">publisher</span><span class="sxs-lookup"><span data-stu-id="0d265-145">publisher</span></span>|<span data-ttu-id="0d265-146">String</span><span class="sxs-lookup"><span data-stu-id="0d265-146">String</span></span>|<span data-ttu-id="0d265-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="0d265-147">The publisher of the app.</span></span> <span data-ttu-id="0d265-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0d265-149">largeIcon</span></span>|[<span data-ttu-id="0d265-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0d265-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0d265-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="0d265-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0d265-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d265-153">createdDateTime</span></span>|<span data-ttu-id="0d265-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d265-154">DateTimeOffset</span></span>|<span data-ttu-id="0d265-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="0d265-155">The date and time the app was created.</span></span> <span data-ttu-id="0d265-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d265-157">lastModifiedDateTime</span></span>|<span data-ttu-id="0d265-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d265-158">DateTimeOffset</span></span>|<span data-ttu-id="0d265-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="0d265-159">The date and time the app was last modified.</span></span> <span data-ttu-id="0d265-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0d265-161">isFeatured</span></span>|<span data-ttu-id="0d265-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d265-162">Boolean</span></span>|<span data-ttu-id="0d265-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0d265-164">privacyInformationUrl</span></span>|<span data-ttu-id="0d265-165">String</span><span class="sxs-lookup"><span data-stu-id="0d265-165">String</span></span>|<span data-ttu-id="0d265-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="0d265-166">The privacy statement Url.</span></span> <span data-ttu-id="0d265-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0d265-168">informationUrl</span></span>|<span data-ttu-id="0d265-169">String</span><span class="sxs-lookup"><span data-stu-id="0d265-169">String</span></span>|<span data-ttu-id="0d265-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="0d265-170">The more information Url.</span></span> <span data-ttu-id="0d265-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-172">owner</span><span class="sxs-lookup"><span data-stu-id="0d265-172">owner</span></span>|<span data-ttu-id="0d265-173">String</span><span class="sxs-lookup"><span data-stu-id="0d265-173">String</span></span>|<span data-ttu-id="0d265-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="0d265-174">The owner of the app.</span></span> <span data-ttu-id="0d265-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-176">developer</span><span class="sxs-lookup"><span data-stu-id="0d265-176">developer</span></span>|<span data-ttu-id="0d265-177">String</span><span class="sxs-lookup"><span data-stu-id="0d265-177">String</span></span>|<span data-ttu-id="0d265-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="0d265-178">The developer of the app.</span></span> <span data-ttu-id="0d265-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-180">notes</span><span class="sxs-lookup"><span data-stu-id="0d265-180">notes</span></span>|<span data-ttu-id="0d265-181">String</span><span class="sxs-lookup"><span data-stu-id="0d265-181">String</span></span>|<span data-ttu-id="0d265-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="0d265-182">Notes for the app.</span></span> <span data-ttu-id="0d265-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="0d265-184">uploadState</span></span>|<span data-ttu-id="0d265-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0d265-185">Int32</span></span>|<span data-ttu-id="0d265-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="0d265-186">The upload state.</span></span> <span data-ttu-id="0d265-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="0d265-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="0d265-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="0d265-189">publishingState</span></span>|[<span data-ttu-id="0d265-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="0d265-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0d265-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="0d265-191">The publishing state for the app.</span></span> <span data-ttu-id="0d265-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="0d265-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0d265-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="0d265-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0d265-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0d265-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0d265-195">isAssigned</span></span>|<span data-ttu-id="0d265-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d265-196">Boolean</span></span>|<span data-ttu-id="0d265-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="0d265-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0d265-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0d265-199">roleScopeTagIds</span></span>|<span data-ttu-id="0d265-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0d265-200">String collection</span></span>|<span data-ttu-id="0d265-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="0d265-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0d265-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="0d265-203">dependentAppCount</span></span>|<span data-ttu-id="0d265-204">Int32</span><span class="sxs-lookup"><span data-stu-id="0d265-204">Int32</span></span>|<span data-ttu-id="0d265-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="0d265-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="0d265-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0d265-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0d265-207">committedContentVersion</span></span>|<span data-ttu-id="0d265-208">String</span><span class="sxs-lookup"><span data-stu-id="0d265-208">String</span></span>|<span data-ttu-id="0d265-209">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="0d265-209">The internal committed content version.</span></span> <span data-ttu-id="0d265-210">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0d265-211">fileName</span><span class="sxs-lookup"><span data-stu-id="0d265-211">fileName</span></span>|<span data-ttu-id="0d265-212">String</span><span class="sxs-lookup"><span data-stu-id="0d265-212">String</span></span>|<span data-ttu-id="0d265-213">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="0d265-213">The name of the main Lob application file.</span></span> <span data-ttu-id="0d265-214">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0d265-215">size</span><span class="sxs-lookup"><span data-stu-id="0d265-215">size</span></span>|<span data-ttu-id="0d265-216">Int64</span><span class="sxs-lookup"><span data-stu-id="0d265-216">Int64</span></span>|<span data-ttu-id="0d265-217">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="0d265-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="0d265-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0d265-219">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="0d265-219">applicableArchitectures</span></span>|[<span data-ttu-id="0d265-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="0d265-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="0d265-221">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="0d265-221">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="0d265-222">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="0d265-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="0d265-223">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="0d265-223">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="0d265-224">identityName</span><span class="sxs-lookup"><span data-stu-id="0d265-224">identityName</span></span>|<span data-ttu-id="0d265-225">String</span><span class="sxs-lookup"><span data-stu-id="0d265-225">String</span></span>|<span data-ttu-id="0d265-226">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="0d265-226">The Identity Name.</span></span> <span data-ttu-id="0d265-227">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d265-227">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d265-228">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="0d265-228">identityPublisherHash</span></span>|<span data-ttu-id="0d265-229">String</span><span class="sxs-lookup"><span data-stu-id="0d265-229">String</span></span>|<span data-ttu-id="0d265-230">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="0d265-230">The Identity Publisher Hash.</span></span> <span data-ttu-id="0d265-231">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d265-231">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d265-232">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="0d265-232">identityResourceIdentifier</span></span>|<span data-ttu-id="0d265-233">String</span><span class="sxs-lookup"><span data-stu-id="0d265-233">String</span></span>|<span data-ttu-id="0d265-234">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="0d265-234">The Identity Resource Identifier.</span></span> <span data-ttu-id="0d265-235">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d265-235">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d265-236">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0d265-236">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0d265-237">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0d265-237">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="0d265-238">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="0d265-238">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="0d265-239">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d265-239">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d265-240">фонепродуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="0d265-240">phoneProductIdentifier</span></span>|<span data-ttu-id="0d265-241">String</span><span class="sxs-lookup"><span data-stu-id="0d265-241">String</span></span>|<span data-ttu-id="0d265-242">Идентификатор телефонного продукта.</span><span class="sxs-lookup"><span data-stu-id="0d265-242">The Phone Product Identifier.</span></span> <span data-ttu-id="0d265-243">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d265-243">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d265-244">фонепублишерид</span><span class="sxs-lookup"><span data-stu-id="0d265-244">phonePublisherId</span></span>|<span data-ttu-id="0d265-245">String</span><span class="sxs-lookup"><span data-stu-id="0d265-245">String</span></span>|<span data-ttu-id="0d265-246">Идентификатор издателя телефона. наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d265-246">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d265-247">identityVersion</span><span class="sxs-lookup"><span data-stu-id="0d265-247">identityVersion</span></span>|<span data-ttu-id="0d265-248">String</span><span class="sxs-lookup"><span data-stu-id="0d265-248">String</span></span>|<span data-ttu-id="0d265-249">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="0d265-249">The identity version.</span></span> <span data-ttu-id="0d265-250">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="0d265-250">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="0d265-251">аппкспаккажеинформатионлист</span><span class="sxs-lookup"><span data-stu-id="0d265-251">appXPackageInformationList</span></span>|<span data-ttu-id="0d265-252">Коллекция [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="0d265-252">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="0d265-253">Список сведений о пакете AppX.</span><span class="sxs-lookup"><span data-stu-id="0d265-253">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="0d265-254">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d265-254">Response</span></span>
<span data-ttu-id="0d265-255">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d265-255">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d265-256">Пример</span><span class="sxs-lookup"><span data-stu-id="0d265-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d265-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d265-257">Request</span></span>
<span data-ttu-id="0d265-258">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d265-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2311

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

### <a name="response"></a><span data-ttu-id="0d265-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d265-259">Response</span></span>
<span data-ttu-id="0d265-p129">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d265-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2483

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



