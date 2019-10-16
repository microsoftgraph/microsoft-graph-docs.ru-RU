---
title: Обновление windowsPhone81AppXBundle
description: Обновление свойств объекта windowsPhone81AppXBundle.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04e4d87eb7e5170c26faa311c4e102e92a6a95e8
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535018"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="cc568-103">Обновление windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="cc568-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="cc568-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc568-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc568-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc568-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc568-106">Обновление свойств объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="cc568-106">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc568-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cc568-107">Prerequisites</span></span>
<span data-ttu-id="cc568-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc568-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc568-110">Permission type</span></span>|<span data-ttu-id="cc568-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc568-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc568-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc568-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc568-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc568-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cc568-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc568-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc568-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc568-115">Not supported.</span></span>|
|<span data-ttu-id="cc568-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="cc568-116">Application</span></span>|<span data-ttu-id="cc568-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc568-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc568-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc568-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="cc568-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc568-119">Request headers</span></span>
|<span data-ttu-id="cc568-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc568-120">Header</span></span>|<span data-ttu-id="cc568-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cc568-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc568-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc568-122">Authorization</span></span>|<span data-ttu-id="cc568-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc568-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc568-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cc568-124">Accept</span></span>|<span data-ttu-id="cc568-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc568-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc568-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc568-126">Request body</span></span>
<span data-ttu-id="cc568-127">В тексте запроса добавьте представление объекта [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc568-127">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="cc568-128">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-128">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="cc568-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc568-129">Property</span></span>|<span data-ttu-id="cc568-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cc568-130">Type</span></span>|<span data-ttu-id="cc568-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cc568-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc568-132">id</span><span class="sxs-lookup"><span data-stu-id="cc568-132">id</span></span>|<span data-ttu-id="cc568-133">Строка</span><span class="sxs-lookup"><span data-stu-id="cc568-133">String</span></span>|<span data-ttu-id="cc568-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cc568-134">Key of the entity.</span></span> <span data-ttu-id="cc568-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cc568-136">displayName</span></span>|<span data-ttu-id="cc568-137">Строка</span><span class="sxs-lookup"><span data-stu-id="cc568-137">String</span></span>|<span data-ttu-id="cc568-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="cc568-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cc568-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-140">description</span><span class="sxs-lookup"><span data-stu-id="cc568-140">description</span></span>|<span data-ttu-id="cc568-141">Строка</span><span class="sxs-lookup"><span data-stu-id="cc568-141">String</span></span>|<span data-ttu-id="cc568-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="cc568-142">The description of the app.</span></span> <span data-ttu-id="cc568-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-144">publisher</span><span class="sxs-lookup"><span data-stu-id="cc568-144">publisher</span></span>|<span data-ttu-id="cc568-145">String</span><span class="sxs-lookup"><span data-stu-id="cc568-145">String</span></span>|<span data-ttu-id="cc568-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="cc568-146">The publisher of the app.</span></span> <span data-ttu-id="cc568-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cc568-148">largeIcon</span></span>|[<span data-ttu-id="cc568-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cc568-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cc568-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="cc568-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cc568-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc568-152">createdDateTime</span></span>|<span data-ttu-id="cc568-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc568-153">DateTimeOffset</span></span>|<span data-ttu-id="cc568-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="cc568-154">The date and time the app was created.</span></span> <span data-ttu-id="cc568-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc568-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cc568-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc568-157">DateTimeOffset</span></span>|<span data-ttu-id="cc568-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="cc568-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cc568-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cc568-160">isFeatured</span></span>|<span data-ttu-id="cc568-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc568-161">Boolean</span></span>|<span data-ttu-id="cc568-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cc568-163">privacyInformationUrl</span></span>|<span data-ttu-id="cc568-164">String</span><span class="sxs-lookup"><span data-stu-id="cc568-164">String</span></span>|<span data-ttu-id="cc568-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cc568-165">The privacy statement Url.</span></span> <span data-ttu-id="cc568-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cc568-167">informationUrl</span></span>|<span data-ttu-id="cc568-168">String</span><span class="sxs-lookup"><span data-stu-id="cc568-168">String</span></span>|<span data-ttu-id="cc568-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="cc568-169">The more information Url.</span></span> <span data-ttu-id="cc568-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-171">owner</span><span class="sxs-lookup"><span data-stu-id="cc568-171">owner</span></span>|<span data-ttu-id="cc568-172">String</span><span class="sxs-lookup"><span data-stu-id="cc568-172">String</span></span>|<span data-ttu-id="cc568-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="cc568-173">The owner of the app.</span></span> <span data-ttu-id="cc568-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-175">developer</span><span class="sxs-lookup"><span data-stu-id="cc568-175">developer</span></span>|<span data-ttu-id="cc568-176">String</span><span class="sxs-lookup"><span data-stu-id="cc568-176">String</span></span>|<span data-ttu-id="cc568-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="cc568-177">The developer of the app.</span></span> <span data-ttu-id="cc568-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-179">notes</span><span class="sxs-lookup"><span data-stu-id="cc568-179">notes</span></span>|<span data-ttu-id="cc568-180">String</span><span class="sxs-lookup"><span data-stu-id="cc568-180">String</span></span>|<span data-ttu-id="cc568-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="cc568-181">Notes for the app.</span></span> <span data-ttu-id="cc568-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="cc568-183">uploadState</span></span>|<span data-ttu-id="cc568-184">Int32</span><span class="sxs-lookup"><span data-stu-id="cc568-184">Int32</span></span>|<span data-ttu-id="cc568-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="cc568-185">The upload state.</span></span> <span data-ttu-id="cc568-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="cc568-187">publishingState</span></span>|[<span data-ttu-id="cc568-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="cc568-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cc568-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="cc568-189">The publishing state for the app.</span></span> <span data-ttu-id="cc568-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="cc568-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cc568-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="cc568-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cc568-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cc568-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cc568-193">isAssigned</span></span>|<span data-ttu-id="cc568-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc568-194">Boolean</span></span>|<span data-ttu-id="cc568-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="cc568-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cc568-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cc568-197">roleScopeTagIds</span></span>|<span data-ttu-id="cc568-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cc568-198">String collection</span></span>|<span data-ttu-id="cc568-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="cc568-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cc568-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="cc568-201">dependentAppCount</span></span>|<span data-ttu-id="cc568-202">Int32</span><span class="sxs-lookup"><span data-stu-id="cc568-202">Int32</span></span>|<span data-ttu-id="cc568-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="cc568-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="cc568-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cc568-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cc568-205">committedContentVersion</span></span>|<span data-ttu-id="cc568-206">String</span><span class="sxs-lookup"><span data-stu-id="cc568-206">String</span></span>|<span data-ttu-id="cc568-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="cc568-207">The internal committed content version.</span></span> <span data-ttu-id="cc568-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cc568-209">fileName</span><span class="sxs-lookup"><span data-stu-id="cc568-209">fileName</span></span>|<span data-ttu-id="cc568-210">String</span><span class="sxs-lookup"><span data-stu-id="cc568-210">String</span></span>|<span data-ttu-id="cc568-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="cc568-211">The name of the main Lob application file.</span></span> <span data-ttu-id="cc568-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cc568-213">size</span><span class="sxs-lookup"><span data-stu-id="cc568-213">size</span></span>|<span data-ttu-id="cc568-214">Int64</span><span class="sxs-lookup"><span data-stu-id="cc568-214">Int64</span></span>|<span data-ttu-id="cc568-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="cc568-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="cc568-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cc568-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="cc568-217">applicableArchitectures</span></span>|[<span data-ttu-id="cc568-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="cc568-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="cc568-219">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="cc568-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="cc568-220">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="cc568-220">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="cc568-221">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="cc568-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="cc568-222">identityName</span><span class="sxs-lookup"><span data-stu-id="cc568-222">identityName</span></span>|<span data-ttu-id="cc568-223">String</span><span class="sxs-lookup"><span data-stu-id="cc568-223">String</span></span>|<span data-ttu-id="cc568-224">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="cc568-224">The Identity Name.</span></span> <span data-ttu-id="cc568-225">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cc568-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cc568-226">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="cc568-226">identityPublisherHash</span></span>|<span data-ttu-id="cc568-227">String</span><span class="sxs-lookup"><span data-stu-id="cc568-227">String</span></span>|<span data-ttu-id="cc568-228">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="cc568-228">The Identity Publisher Hash.</span></span> <span data-ttu-id="cc568-229">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cc568-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cc568-230">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="cc568-230">identityResourceIdentifier</span></span>|<span data-ttu-id="cc568-231">String</span><span class="sxs-lookup"><span data-stu-id="cc568-231">String</span></span>|<span data-ttu-id="cc568-232">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="cc568-232">The Identity Resource Identifier.</span></span> <span data-ttu-id="cc568-233">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cc568-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cc568-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cc568-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cc568-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cc568-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="cc568-236">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="cc568-236">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="cc568-237">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cc568-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cc568-238">фонепродуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="cc568-238">phoneProductIdentifier</span></span>|<span data-ttu-id="cc568-239">String</span><span class="sxs-lookup"><span data-stu-id="cc568-239">String</span></span>|<span data-ttu-id="cc568-240">Идентификатор телефонного продукта.</span><span class="sxs-lookup"><span data-stu-id="cc568-240">The Phone Product Identifier.</span></span> <span data-ttu-id="cc568-241">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cc568-241">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cc568-242">фонепублишерид</span><span class="sxs-lookup"><span data-stu-id="cc568-242">phonePublisherId</span></span>|<span data-ttu-id="cc568-243">String</span><span class="sxs-lookup"><span data-stu-id="cc568-243">String</span></span>|<span data-ttu-id="cc568-244">Идентификатор издателя телефона. наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cc568-244">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cc568-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="cc568-245">identityVersion</span></span>|<span data-ttu-id="cc568-246">String</span><span class="sxs-lookup"><span data-stu-id="cc568-246">String</span></span>|<span data-ttu-id="cc568-247">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="cc568-247">The identity version.</span></span> <span data-ttu-id="cc568-248">Наследуется от [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cc568-248">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cc568-249">аппкспаккажеинформатионлист</span><span class="sxs-lookup"><span data-stu-id="cc568-249">appXPackageInformationList</span></span>|<span data-ttu-id="cc568-250">Коллекция [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="cc568-250">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="cc568-251">Список сведений о пакете AppX.</span><span class="sxs-lookup"><span data-stu-id="cc568-251">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="cc568-252">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc568-252">Response</span></span>
<span data-ttu-id="cc568-253">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc568-253">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc568-254">Пример</span><span class="sxs-lookup"><span data-stu-id="cc568-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc568-255">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc568-255">Request</span></span>
<span data-ttu-id="cc568-256">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc568-256">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cc568-257">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc568-257">Response</span></span>
<span data-ttu-id="cc568-p129">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cc568-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






