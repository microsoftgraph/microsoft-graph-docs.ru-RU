---
title: Обновление Виндовсфонексап
description: Обновление свойств объекта Виндовсфонексап.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f5dcecd676e12ab51c4a651b1393e51775a8090
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43409073"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="0e894-103">Обновление Виндовсфонексап</span><span class="sxs-lookup"><span data-stu-id="0e894-103">Update windowsPhoneXAP</span></span>

<span data-ttu-id="0e894-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e894-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e894-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e894-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e894-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e894-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e894-107">Обновление свойств объекта [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="0e894-107">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e894-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0e894-108">Prerequisites</span></span>
<span data-ttu-id="0e894-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e894-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e894-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e894-111">Permission type</span></span>|<span data-ttu-id="0e894-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e894-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e894-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e894-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e894-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e894-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0e894-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e894-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e894-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e894-116">Not supported.</span></span>|
|<span data-ttu-id="0e894-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0e894-117">Application</span></span>|<span data-ttu-id="0e894-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e894-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e894-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e894-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="0e894-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0e894-120">Request headers</span></span>
|<span data-ttu-id="0e894-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e894-121">Header</span></span>|<span data-ttu-id="0e894-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0e894-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e894-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e894-123">Authorization</span></span>|<span data-ttu-id="0e894-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e894-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e894-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e894-125">Accept</span></span>|<span data-ttu-id="0e894-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e894-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e894-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e894-127">Request body</span></span>
<span data-ttu-id="0e894-128">В тексте запроса добавьте представление объекта [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e894-128">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="0e894-129">В следующей таблице приведены свойства, необходимые при создании [виндовсфонексап](../resources/intune-apps-windowsphonexap.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-129">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="0e894-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e894-130">Property</span></span>|<span data-ttu-id="0e894-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0e894-131">Type</span></span>|<span data-ttu-id="0e894-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0e894-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e894-133">id</span><span class="sxs-lookup"><span data-stu-id="0e894-133">id</span></span>|<span data-ttu-id="0e894-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0e894-134">String</span></span>|<span data-ttu-id="0e894-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0e894-135">Key of the entity.</span></span> <span data-ttu-id="0e894-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0e894-137">displayName</span></span>|<span data-ttu-id="0e894-138">Строка</span><span class="sxs-lookup"><span data-stu-id="0e894-138">String</span></span>|<span data-ttu-id="0e894-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="0e894-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0e894-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-141">description</span><span class="sxs-lookup"><span data-stu-id="0e894-141">description</span></span>|<span data-ttu-id="0e894-142">Строка</span><span class="sxs-lookup"><span data-stu-id="0e894-142">String</span></span>|<span data-ttu-id="0e894-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="0e894-143">The description of the app.</span></span> <span data-ttu-id="0e894-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-145">publisher</span><span class="sxs-lookup"><span data-stu-id="0e894-145">publisher</span></span>|<span data-ttu-id="0e894-146">String</span><span class="sxs-lookup"><span data-stu-id="0e894-146">String</span></span>|<span data-ttu-id="0e894-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="0e894-147">The publisher of the app.</span></span> <span data-ttu-id="0e894-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0e894-149">largeIcon</span></span>|[<span data-ttu-id="0e894-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0e894-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0e894-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="0e894-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0e894-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e894-153">createdDateTime</span></span>|<span data-ttu-id="0e894-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e894-154">DateTimeOffset</span></span>|<span data-ttu-id="0e894-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="0e894-155">The date and time the app was created.</span></span> <span data-ttu-id="0e894-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e894-157">lastModifiedDateTime</span></span>|<span data-ttu-id="0e894-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e894-158">DateTimeOffset</span></span>|<span data-ttu-id="0e894-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="0e894-159">The date and time the app was last modified.</span></span> <span data-ttu-id="0e894-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0e894-161">isFeatured</span></span>|<span data-ttu-id="0e894-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e894-162">Boolean</span></span>|<span data-ttu-id="0e894-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0e894-164">privacyInformationUrl</span></span>|<span data-ttu-id="0e894-165">String</span><span class="sxs-lookup"><span data-stu-id="0e894-165">String</span></span>|<span data-ttu-id="0e894-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="0e894-166">The privacy statement Url.</span></span> <span data-ttu-id="0e894-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0e894-168">informationUrl</span></span>|<span data-ttu-id="0e894-169">String</span><span class="sxs-lookup"><span data-stu-id="0e894-169">String</span></span>|<span data-ttu-id="0e894-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="0e894-170">The more information Url.</span></span> <span data-ttu-id="0e894-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-172">owner</span><span class="sxs-lookup"><span data-stu-id="0e894-172">owner</span></span>|<span data-ttu-id="0e894-173">String</span><span class="sxs-lookup"><span data-stu-id="0e894-173">String</span></span>|<span data-ttu-id="0e894-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="0e894-174">The owner of the app.</span></span> <span data-ttu-id="0e894-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-176">developer</span><span class="sxs-lookup"><span data-stu-id="0e894-176">developer</span></span>|<span data-ttu-id="0e894-177">String</span><span class="sxs-lookup"><span data-stu-id="0e894-177">String</span></span>|<span data-ttu-id="0e894-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="0e894-178">The developer of the app.</span></span> <span data-ttu-id="0e894-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-180">notes</span><span class="sxs-lookup"><span data-stu-id="0e894-180">notes</span></span>|<span data-ttu-id="0e894-181">String</span><span class="sxs-lookup"><span data-stu-id="0e894-181">String</span></span>|<span data-ttu-id="0e894-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="0e894-182">Notes for the app.</span></span> <span data-ttu-id="0e894-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="0e894-184">uploadState</span></span>|<span data-ttu-id="0e894-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0e894-185">Int32</span></span>|<span data-ttu-id="0e894-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="0e894-186">The upload state.</span></span> <span data-ttu-id="0e894-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="0e894-188">publishingState</span></span>|[<span data-ttu-id="0e894-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="0e894-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0e894-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="0e894-190">The publishing state for the app.</span></span> <span data-ttu-id="0e894-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="0e894-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0e894-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="0e894-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0e894-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0e894-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0e894-194">isAssigned</span></span>|<span data-ttu-id="0e894-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e894-195">Boolean</span></span>|<span data-ttu-id="0e894-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="0e894-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0e894-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e894-198">roleScopeTagIds</span></span>|<span data-ttu-id="0e894-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0e894-199">String collection</span></span>|<span data-ttu-id="0e894-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="0e894-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0e894-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="0e894-202">dependentAppCount</span></span>|<span data-ttu-id="0e894-203">Int32</span><span class="sxs-lookup"><span data-stu-id="0e894-203">Int32</span></span>|<span data-ttu-id="0e894-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="0e894-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="0e894-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0e894-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0e894-206">committedContentVersion</span></span>|<span data-ttu-id="0e894-207">String</span><span class="sxs-lookup"><span data-stu-id="0e894-207">String</span></span>|<span data-ttu-id="0e894-208">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="0e894-208">The internal committed content version.</span></span> <span data-ttu-id="0e894-209">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0e894-210">fileName</span><span class="sxs-lookup"><span data-stu-id="0e894-210">fileName</span></span>|<span data-ttu-id="0e894-211">String</span><span class="sxs-lookup"><span data-stu-id="0e894-211">String</span></span>|<span data-ttu-id="0e894-212">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="0e894-212">The name of the main Lob application file.</span></span> <span data-ttu-id="0e894-213">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0e894-214">size</span><span class="sxs-lookup"><span data-stu-id="0e894-214">size</span></span>|<span data-ttu-id="0e894-215">Int64</span><span class="sxs-lookup"><span data-stu-id="0e894-215">Int64</span></span>|<span data-ttu-id="0e894-216">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="0e894-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="0e894-217">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e894-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0e894-218">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0e894-218">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0e894-219">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0e894-219">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="0e894-220">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="0e894-220">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="0e894-221">продуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="0e894-221">productIdentifier</span></span>|<span data-ttu-id="0e894-222">String</span><span class="sxs-lookup"><span data-stu-id="0e894-222">String</span></span>|<span data-ttu-id="0e894-223">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="0e894-223">The Product Identifier.</span></span>|
|<span data-ttu-id="0e894-224">identityVersion</span><span class="sxs-lookup"><span data-stu-id="0e894-224">identityVersion</span></span>|<span data-ttu-id="0e894-225">String</span><span class="sxs-lookup"><span data-stu-id="0e894-225">String</span></span>|<span data-ttu-id="0e894-226">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="0e894-226">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="0e894-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e894-227">Response</span></span>
<span data-ttu-id="0e894-228">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e894-228">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e894-229">Пример</span><span class="sxs-lookup"><span data-stu-id="0e894-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e894-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e894-230">Request</span></span>
<span data-ttu-id="0e894-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e894-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e894-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e894-232">Response</span></span>
<span data-ttu-id="0e894-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e894-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



