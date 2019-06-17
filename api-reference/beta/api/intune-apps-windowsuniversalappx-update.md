---
title: Update windowsUniversalAppX
description: Обновление свойств объекта windowsUniversalAppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42f0b7b9f2a1073b065248a7d7a247ef63b4be0e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972699"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="85404-103">Update windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="85404-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="85404-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85404-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85404-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85404-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85404-106">Обновление свойств объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="85404-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85404-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="85404-107">Prerequisites</span></span>
<span data-ttu-id="85404-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85404-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85404-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85404-110">Permission type</span></span>|<span data-ttu-id="85404-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85404-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85404-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85404-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85404-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85404-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="85404-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85404-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85404-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85404-115">Not supported.</span></span>|
|<span data-ttu-id="85404-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85404-116">Application</span></span>|<span data-ttu-id="85404-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85404-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85404-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85404-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="85404-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85404-119">Request headers</span></span>
|<span data-ttu-id="85404-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85404-120">Header</span></span>|<span data-ttu-id="85404-121">Значение</span><span class="sxs-lookup"><span data-stu-id="85404-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85404-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85404-122">Authorization</span></span>|<span data-ttu-id="85404-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85404-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85404-124">Accept</span><span class="sxs-lookup"><span data-stu-id="85404-124">Accept</span></span>|<span data-ttu-id="85404-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85404-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85404-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85404-126">Request body</span></span>
<span data-ttu-id="85404-127">В теле запроса добавьте представление объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85404-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="85404-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="85404-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="85404-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="85404-129">Property</span></span>|<span data-ttu-id="85404-130">Тип</span><span class="sxs-lookup"><span data-stu-id="85404-130">Type</span></span>|<span data-ttu-id="85404-131">Описание</span><span class="sxs-lookup"><span data-stu-id="85404-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85404-132">id</span><span class="sxs-lookup"><span data-stu-id="85404-132">id</span></span>|<span data-ttu-id="85404-133">Строка</span><span class="sxs-lookup"><span data-stu-id="85404-133">String</span></span>|<span data-ttu-id="85404-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="85404-134">Key of the entity.</span></span> <span data-ttu-id="85404-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-136">displayName</span><span class="sxs-lookup"><span data-stu-id="85404-136">displayName</span></span>|<span data-ttu-id="85404-137">Строка</span><span class="sxs-lookup"><span data-stu-id="85404-137">String</span></span>|<span data-ttu-id="85404-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="85404-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="85404-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-140">description</span><span class="sxs-lookup"><span data-stu-id="85404-140">description</span></span>|<span data-ttu-id="85404-141">Строка</span><span class="sxs-lookup"><span data-stu-id="85404-141">String</span></span>|<span data-ttu-id="85404-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="85404-142">The description of the app.</span></span> <span data-ttu-id="85404-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-144">publisher</span><span class="sxs-lookup"><span data-stu-id="85404-144">publisher</span></span>|<span data-ttu-id="85404-145">String</span><span class="sxs-lookup"><span data-stu-id="85404-145">String</span></span>|<span data-ttu-id="85404-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="85404-146">The publisher of the app.</span></span> <span data-ttu-id="85404-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="85404-148">largeIcon</span></span>|[<span data-ttu-id="85404-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="85404-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="85404-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="85404-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="85404-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85404-152">createdDateTime</span></span>|<span data-ttu-id="85404-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85404-153">DateTimeOffset</span></span>|<span data-ttu-id="85404-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="85404-154">The date and time the app was created.</span></span> <span data-ttu-id="85404-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85404-156">lastModifiedDateTime</span></span>|<span data-ttu-id="85404-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85404-157">DateTimeOffset</span></span>|<span data-ttu-id="85404-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="85404-158">The date and time the app was last modified.</span></span> <span data-ttu-id="85404-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="85404-160">isFeatured</span></span>|<span data-ttu-id="85404-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="85404-161">Boolean</span></span>|<span data-ttu-id="85404-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="85404-163">privacyInformationUrl</span></span>|<span data-ttu-id="85404-164">String</span><span class="sxs-lookup"><span data-stu-id="85404-164">String</span></span>|<span data-ttu-id="85404-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="85404-165">The privacy statement Url.</span></span> <span data-ttu-id="85404-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="85404-167">informationUrl</span></span>|<span data-ttu-id="85404-168">String</span><span class="sxs-lookup"><span data-stu-id="85404-168">String</span></span>|<span data-ttu-id="85404-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="85404-169">The more information Url.</span></span> <span data-ttu-id="85404-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-171">owner</span><span class="sxs-lookup"><span data-stu-id="85404-171">owner</span></span>|<span data-ttu-id="85404-172">String</span><span class="sxs-lookup"><span data-stu-id="85404-172">String</span></span>|<span data-ttu-id="85404-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="85404-173">The owner of the app.</span></span> <span data-ttu-id="85404-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-175">developer</span><span class="sxs-lookup"><span data-stu-id="85404-175">developer</span></span>|<span data-ttu-id="85404-176">String</span><span class="sxs-lookup"><span data-stu-id="85404-176">String</span></span>|<span data-ttu-id="85404-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="85404-177">The developer of the app.</span></span> <span data-ttu-id="85404-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-179">notes</span><span class="sxs-lookup"><span data-stu-id="85404-179">notes</span></span>|<span data-ttu-id="85404-180">String</span><span class="sxs-lookup"><span data-stu-id="85404-180">String</span></span>|<span data-ttu-id="85404-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="85404-181">Notes for the app.</span></span> <span data-ttu-id="85404-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="85404-183">uploadState</span></span>|<span data-ttu-id="85404-184">Int32</span><span class="sxs-lookup"><span data-stu-id="85404-184">Int32</span></span>|<span data-ttu-id="85404-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="85404-185">The upload state.</span></span> <span data-ttu-id="85404-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="85404-187">publishingState</span></span>|[<span data-ttu-id="85404-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="85404-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="85404-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="85404-189">The publishing state for the app.</span></span> <span data-ttu-id="85404-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="85404-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="85404-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="85404-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="85404-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="85404-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="85404-193">isAssigned</span></span>|<span data-ttu-id="85404-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="85404-194">Boolean</span></span>|<span data-ttu-id="85404-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="85404-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="85404-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="85404-197">roleScopeTagIds</span></span>|<span data-ttu-id="85404-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="85404-198">String collection</span></span>|<span data-ttu-id="85404-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="85404-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="85404-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="85404-201">dependentAppCount</span></span>|<span data-ttu-id="85404-202">Int32</span><span class="sxs-lookup"><span data-stu-id="85404-202">Int32</span></span>|<span data-ttu-id="85404-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="85404-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="85404-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85404-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="85404-205">committedContentVersion</span></span>|<span data-ttu-id="85404-206">String</span><span class="sxs-lookup"><span data-stu-id="85404-206">String</span></span>|<span data-ttu-id="85404-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="85404-207">The internal committed content version.</span></span> <span data-ttu-id="85404-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="85404-209">fileName</span><span class="sxs-lookup"><span data-stu-id="85404-209">fileName</span></span>|<span data-ttu-id="85404-210">String</span><span class="sxs-lookup"><span data-stu-id="85404-210">String</span></span>|<span data-ttu-id="85404-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="85404-211">The name of the main Lob application file.</span></span> <span data-ttu-id="85404-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="85404-213">size</span><span class="sxs-lookup"><span data-stu-id="85404-213">size</span></span>|<span data-ttu-id="85404-214">Int64</span><span class="sxs-lookup"><span data-stu-id="85404-214">Int64</span></span>|<span data-ttu-id="85404-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="85404-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="85404-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="85404-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="85404-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="85404-217">applicableArchitectures</span></span>|[<span data-ttu-id="85404-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="85404-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="85404-219">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="85404-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="85404-220">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="85404-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="85404-221">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="85404-221">applicableDeviceTypes</span></span>|[<span data-ttu-id="85404-222">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="85404-222">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="85404-223">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="85404-223">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="85404-224">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="85404-224">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="85404-225">identityName</span><span class="sxs-lookup"><span data-stu-id="85404-225">identityName</span></span>|<span data-ttu-id="85404-226">String</span><span class="sxs-lookup"><span data-stu-id="85404-226">String</span></span>|<span data-ttu-id="85404-227">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="85404-227">The Identity Name.</span></span>|
|<span data-ttu-id="85404-228">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="85404-228">identityPublisherHash</span></span>|<span data-ttu-id="85404-229">String</span><span class="sxs-lookup"><span data-stu-id="85404-229">String</span></span>|<span data-ttu-id="85404-230">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="85404-230">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="85404-231">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="85404-231">identityResourceIdentifier</span></span>|<span data-ttu-id="85404-232">String</span><span class="sxs-lookup"><span data-stu-id="85404-232">String</span></span>|<span data-ttu-id="85404-233">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="85404-233">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="85404-234">isBundle</span><span class="sxs-lookup"><span data-stu-id="85404-234">isBundle</span></span>|<span data-ttu-id="85404-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="85404-235">Boolean</span></span>|<span data-ttu-id="85404-236">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="85404-236">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="85404-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="85404-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="85404-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="85404-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="85404-239">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="85404-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="85404-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="85404-240">identityVersion</span></span>|<span data-ttu-id="85404-241">String</span><span class="sxs-lookup"><span data-stu-id="85404-241">String</span></span>|<span data-ttu-id="85404-242">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="85404-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="85404-243">Ответ</span><span class="sxs-lookup"><span data-stu-id="85404-243">Response</span></span>
<span data-ttu-id="85404-244">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="85404-244">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85404-245">Пример</span><span class="sxs-lookup"><span data-stu-id="85404-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="85404-246">Запрос</span><span class="sxs-lookup"><span data-stu-id="85404-246">Request</span></span>
<span data-ttu-id="85404-247">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85404-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1461

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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="85404-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="85404-248">Response</span></span>
<span data-ttu-id="85404-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85404-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```





