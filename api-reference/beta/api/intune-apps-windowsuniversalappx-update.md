---
title: Update windowsUniversalAppX
description: Обновление свойств объекта windowsUniversalAppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 003b4450c17025cf44f4d7bde88c7cbd02277412
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32485910"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="64401-103">Update windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="64401-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="64401-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64401-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64401-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64401-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64401-106">Обновление свойств объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="64401-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64401-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="64401-107">Prerequisites</span></span>
<span data-ttu-id="64401-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64401-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64401-110">Permission type</span></span>|<span data-ttu-id="64401-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64401-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64401-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64401-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64401-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64401-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="64401-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64401-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64401-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64401-115">Not supported.</span></span>|
|<span data-ttu-id="64401-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64401-116">Application</span></span>|<span data-ttu-id="64401-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64401-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64401-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64401-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="64401-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64401-119">Request headers</span></span>
|<span data-ttu-id="64401-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64401-120">Header</span></span>|<span data-ttu-id="64401-121">Значение</span><span class="sxs-lookup"><span data-stu-id="64401-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64401-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64401-122">Authorization</span></span>|<span data-ttu-id="64401-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64401-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64401-124">Accept</span><span class="sxs-lookup"><span data-stu-id="64401-124">Accept</span></span>|<span data-ttu-id="64401-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64401-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64401-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64401-126">Request body</span></span>
<span data-ttu-id="64401-127">В теле запроса добавьте представление объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64401-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="64401-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="64401-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="64401-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="64401-129">Property</span></span>|<span data-ttu-id="64401-130">Тип</span><span class="sxs-lookup"><span data-stu-id="64401-130">Type</span></span>|<span data-ttu-id="64401-131">Описание</span><span class="sxs-lookup"><span data-stu-id="64401-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64401-132">id</span><span class="sxs-lookup"><span data-stu-id="64401-132">id</span></span>|<span data-ttu-id="64401-133">Строка</span><span class="sxs-lookup"><span data-stu-id="64401-133">String</span></span>|<span data-ttu-id="64401-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="64401-134">Key of the entity.</span></span> <span data-ttu-id="64401-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-136">displayName</span><span class="sxs-lookup"><span data-stu-id="64401-136">displayName</span></span>|<span data-ttu-id="64401-137">Строка</span><span class="sxs-lookup"><span data-stu-id="64401-137">String</span></span>|<span data-ttu-id="64401-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="64401-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="64401-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-140">description</span><span class="sxs-lookup"><span data-stu-id="64401-140">description</span></span>|<span data-ttu-id="64401-141">String</span><span class="sxs-lookup"><span data-stu-id="64401-141">String</span></span>|<span data-ttu-id="64401-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="64401-142">The description of the app.</span></span> <span data-ttu-id="64401-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-144">publisher</span><span class="sxs-lookup"><span data-stu-id="64401-144">publisher</span></span>|<span data-ttu-id="64401-145">String</span><span class="sxs-lookup"><span data-stu-id="64401-145">String</span></span>|<span data-ttu-id="64401-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="64401-146">The publisher of the app.</span></span> <span data-ttu-id="64401-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="64401-148">largeIcon</span></span>|[<span data-ttu-id="64401-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="64401-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="64401-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="64401-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="64401-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64401-152">createdDateTime</span></span>|<span data-ttu-id="64401-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64401-153">DateTimeOffset</span></span>|<span data-ttu-id="64401-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="64401-154">The date and time the app was created.</span></span> <span data-ttu-id="64401-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64401-156">lastModifiedDateTime</span></span>|<span data-ttu-id="64401-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64401-157">DateTimeOffset</span></span>|<span data-ttu-id="64401-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="64401-158">The date and time the app was last modified.</span></span> <span data-ttu-id="64401-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="64401-160">isFeatured</span></span>|<span data-ttu-id="64401-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="64401-161">Boolean</span></span>|<span data-ttu-id="64401-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="64401-163">privacyInformationUrl</span></span>|<span data-ttu-id="64401-164">String</span><span class="sxs-lookup"><span data-stu-id="64401-164">String</span></span>|<span data-ttu-id="64401-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="64401-165">The privacy statement Url.</span></span> <span data-ttu-id="64401-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="64401-167">informationUrl</span></span>|<span data-ttu-id="64401-168">String</span><span class="sxs-lookup"><span data-stu-id="64401-168">String</span></span>|<span data-ttu-id="64401-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="64401-169">The more information Url.</span></span> <span data-ttu-id="64401-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-171">owner</span><span class="sxs-lookup"><span data-stu-id="64401-171">owner</span></span>|<span data-ttu-id="64401-172">String</span><span class="sxs-lookup"><span data-stu-id="64401-172">String</span></span>|<span data-ttu-id="64401-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="64401-173">The owner of the app.</span></span> <span data-ttu-id="64401-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-175">developer</span><span class="sxs-lookup"><span data-stu-id="64401-175">developer</span></span>|<span data-ttu-id="64401-176">String</span><span class="sxs-lookup"><span data-stu-id="64401-176">String</span></span>|<span data-ttu-id="64401-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="64401-177">The developer of the app.</span></span> <span data-ttu-id="64401-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-179">notes</span><span class="sxs-lookup"><span data-stu-id="64401-179">notes</span></span>|<span data-ttu-id="64401-180">String</span><span class="sxs-lookup"><span data-stu-id="64401-180">String</span></span>|<span data-ttu-id="64401-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="64401-181">Notes for the app.</span></span> <span data-ttu-id="64401-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="64401-183">uploadState</span></span>|<span data-ttu-id="64401-184">Int32</span><span class="sxs-lookup"><span data-stu-id="64401-184">Int32</span></span>|<span data-ttu-id="64401-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="64401-185">The upload state.</span></span> <span data-ttu-id="64401-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="64401-187">publishingState</span></span>|[<span data-ttu-id="64401-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="64401-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="64401-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="64401-189">The publishing state for the app.</span></span> <span data-ttu-id="64401-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="64401-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="64401-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="64401-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="64401-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="64401-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="64401-193">isAssigned</span></span>|<span data-ttu-id="64401-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="64401-194">Boolean</span></span>|<span data-ttu-id="64401-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="64401-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="64401-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64401-197">roleScopeTagIds</span></span>|<span data-ttu-id="64401-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="64401-198">String collection</span></span>|<span data-ttu-id="64401-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="64401-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="64401-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="64401-201">dependentAppCount</span></span>|<span data-ttu-id="64401-202">Int32</span><span class="sxs-lookup"><span data-stu-id="64401-202">Int32</span></span>|<span data-ttu-id="64401-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="64401-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="64401-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64401-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="64401-205">committedContentVersion</span></span>|<span data-ttu-id="64401-206">String</span><span class="sxs-lookup"><span data-stu-id="64401-206">String</span></span>|<span data-ttu-id="64401-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="64401-207">The internal committed content version.</span></span> <span data-ttu-id="64401-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="64401-209">fileName</span><span class="sxs-lookup"><span data-stu-id="64401-209">fileName</span></span>|<span data-ttu-id="64401-210">String</span><span class="sxs-lookup"><span data-stu-id="64401-210">String</span></span>|<span data-ttu-id="64401-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="64401-211">The name of the main Lob application file.</span></span> <span data-ttu-id="64401-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="64401-213">size</span><span class="sxs-lookup"><span data-stu-id="64401-213">size</span></span>|<span data-ttu-id="64401-214">Int64</span><span class="sxs-lookup"><span data-stu-id="64401-214">Int64</span></span>|<span data-ttu-id="64401-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="64401-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="64401-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="64401-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="64401-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="64401-217">applicableArchitectures</span></span>|[<span data-ttu-id="64401-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="64401-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="64401-219">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="64401-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="64401-220">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="64401-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="64401-221">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="64401-221">applicableDeviceTypes</span></span>|[<span data-ttu-id="64401-222">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="64401-222">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="64401-223">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="64401-223">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="64401-224">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="64401-224">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="64401-225">identityName</span><span class="sxs-lookup"><span data-stu-id="64401-225">identityName</span></span>|<span data-ttu-id="64401-226">String</span><span class="sxs-lookup"><span data-stu-id="64401-226">String</span></span>|<span data-ttu-id="64401-227">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="64401-227">The Identity Name.</span></span>|
|<span data-ttu-id="64401-228">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="64401-228">identityPublisherHash</span></span>|<span data-ttu-id="64401-229">String</span><span class="sxs-lookup"><span data-stu-id="64401-229">String</span></span>|<span data-ttu-id="64401-230">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="64401-230">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="64401-231">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="64401-231">identityResourceIdentifier</span></span>|<span data-ttu-id="64401-232">String</span><span class="sxs-lookup"><span data-stu-id="64401-232">String</span></span>|<span data-ttu-id="64401-233">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="64401-233">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="64401-234">isBundle</span><span class="sxs-lookup"><span data-stu-id="64401-234">isBundle</span></span>|<span data-ttu-id="64401-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="64401-235">Boolean</span></span>|<span data-ttu-id="64401-236">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="64401-236">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="64401-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="64401-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="64401-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="64401-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="64401-239">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="64401-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="64401-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="64401-240">identityVersion</span></span>|<span data-ttu-id="64401-241">String</span><span class="sxs-lookup"><span data-stu-id="64401-241">String</span></span>|<span data-ttu-id="64401-242">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="64401-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="64401-243">Ответ</span><span class="sxs-lookup"><span data-stu-id="64401-243">Response</span></span>
<span data-ttu-id="64401-244">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="64401-244">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64401-245">Пример</span><span class="sxs-lookup"><span data-stu-id="64401-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="64401-246">Запрос</span><span class="sxs-lookup"><span data-stu-id="64401-246">Request</span></span>
<span data-ttu-id="64401-247">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64401-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1415

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="64401-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="64401-248">Response</span></span>
<span data-ttu-id="64401-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64401-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1587

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```





