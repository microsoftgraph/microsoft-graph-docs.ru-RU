---
title: Create iosLobApp
description: Создание нового объекта iosLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 482e2bf60be2f8cef510dd3277453dbe37a2dde5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966231"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="73898-103">Create iosLobApp</span><span class="sxs-lookup"><span data-stu-id="73898-103">Create iosLobApp</span></span>

> <span data-ttu-id="73898-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73898-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73898-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73898-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73898-106">Создание нового объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-106">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73898-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="73898-107">Prerequisites</span></span>
<span data-ttu-id="73898-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73898-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73898-110">Permission type</span></span>|<span data-ttu-id="73898-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73898-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73898-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73898-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73898-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73898-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73898-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73898-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73898-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73898-115">Not supported.</span></span>|
|<span data-ttu-id="73898-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73898-116">Application</span></span>|<span data-ttu-id="73898-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73898-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73898-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73898-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="73898-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73898-119">Request headers</span></span>
|<span data-ttu-id="73898-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73898-120">Header</span></span>|<span data-ttu-id="73898-121">Значение</span><span class="sxs-lookup"><span data-stu-id="73898-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73898-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73898-122">Authorization</span></span>|<span data-ttu-id="73898-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73898-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73898-124">Accept</span><span class="sxs-lookup"><span data-stu-id="73898-124">Accept</span></span>|<span data-ttu-id="73898-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73898-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73898-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="73898-126">Request body</span></span>
<span data-ttu-id="73898-127">В теле запроса добавьте представление объекта iosLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73898-127">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="73898-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="73898-128">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="73898-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="73898-129">Property</span></span>|<span data-ttu-id="73898-130">Тип</span><span class="sxs-lookup"><span data-stu-id="73898-130">Type</span></span>|<span data-ttu-id="73898-131">Описание</span><span class="sxs-lookup"><span data-stu-id="73898-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73898-132">id</span><span class="sxs-lookup"><span data-stu-id="73898-132">id</span></span>|<span data-ttu-id="73898-133">Строка</span><span class="sxs-lookup"><span data-stu-id="73898-133">String</span></span>|<span data-ttu-id="73898-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="73898-134">Key of the entity.</span></span> <span data-ttu-id="73898-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-136">displayName</span><span class="sxs-lookup"><span data-stu-id="73898-136">displayName</span></span>|<span data-ttu-id="73898-137">Строка</span><span class="sxs-lookup"><span data-stu-id="73898-137">String</span></span>|<span data-ttu-id="73898-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="73898-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="73898-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-140">description</span><span class="sxs-lookup"><span data-stu-id="73898-140">description</span></span>|<span data-ttu-id="73898-141">Строка</span><span class="sxs-lookup"><span data-stu-id="73898-141">String</span></span>|<span data-ttu-id="73898-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="73898-142">The description of the app.</span></span> <span data-ttu-id="73898-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-144">publisher</span><span class="sxs-lookup"><span data-stu-id="73898-144">publisher</span></span>|<span data-ttu-id="73898-145">String</span><span class="sxs-lookup"><span data-stu-id="73898-145">String</span></span>|<span data-ttu-id="73898-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="73898-146">The publisher of the app.</span></span> <span data-ttu-id="73898-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="73898-148">largeIcon</span></span>|[<span data-ttu-id="73898-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="73898-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="73898-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="73898-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="73898-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73898-152">createdDateTime</span></span>|<span data-ttu-id="73898-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73898-153">DateTimeOffset</span></span>|<span data-ttu-id="73898-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="73898-154">The date and time the app was created.</span></span> <span data-ttu-id="73898-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73898-156">lastModifiedDateTime</span></span>|<span data-ttu-id="73898-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73898-157">DateTimeOffset</span></span>|<span data-ttu-id="73898-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="73898-158">The date and time the app was last modified.</span></span> <span data-ttu-id="73898-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="73898-160">isFeatured</span></span>|<span data-ttu-id="73898-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="73898-161">Boolean</span></span>|<span data-ttu-id="73898-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="73898-163">privacyInformationUrl</span></span>|<span data-ttu-id="73898-164">String</span><span class="sxs-lookup"><span data-stu-id="73898-164">String</span></span>|<span data-ttu-id="73898-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="73898-165">The privacy statement Url.</span></span> <span data-ttu-id="73898-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="73898-167">informationUrl</span></span>|<span data-ttu-id="73898-168">String</span><span class="sxs-lookup"><span data-stu-id="73898-168">String</span></span>|<span data-ttu-id="73898-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="73898-169">The more information Url.</span></span> <span data-ttu-id="73898-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-171">owner</span><span class="sxs-lookup"><span data-stu-id="73898-171">owner</span></span>|<span data-ttu-id="73898-172">String</span><span class="sxs-lookup"><span data-stu-id="73898-172">String</span></span>|<span data-ttu-id="73898-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="73898-173">The owner of the app.</span></span> <span data-ttu-id="73898-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-175">developer</span><span class="sxs-lookup"><span data-stu-id="73898-175">developer</span></span>|<span data-ttu-id="73898-176">String</span><span class="sxs-lookup"><span data-stu-id="73898-176">String</span></span>|<span data-ttu-id="73898-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="73898-177">The developer of the app.</span></span> <span data-ttu-id="73898-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-179">notes</span><span class="sxs-lookup"><span data-stu-id="73898-179">notes</span></span>|<span data-ttu-id="73898-180">String</span><span class="sxs-lookup"><span data-stu-id="73898-180">String</span></span>|<span data-ttu-id="73898-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="73898-181">Notes for the app.</span></span> <span data-ttu-id="73898-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="73898-183">uploadState</span></span>|<span data-ttu-id="73898-184">Int32</span><span class="sxs-lookup"><span data-stu-id="73898-184">Int32</span></span>|<span data-ttu-id="73898-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="73898-185">The upload state.</span></span> <span data-ttu-id="73898-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="73898-187">publishingState</span></span>|[<span data-ttu-id="73898-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="73898-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="73898-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="73898-189">The publishing state for the app.</span></span> <span data-ttu-id="73898-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="73898-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="73898-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="73898-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="73898-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="73898-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="73898-193">isAssigned</span></span>|<span data-ttu-id="73898-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="73898-194">Boolean</span></span>|<span data-ttu-id="73898-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="73898-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="73898-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73898-197">roleScopeTagIds</span></span>|<span data-ttu-id="73898-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="73898-198">String collection</span></span>|<span data-ttu-id="73898-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="73898-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="73898-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="73898-201">dependentAppCount</span></span>|<span data-ttu-id="73898-202">Int32</span><span class="sxs-lookup"><span data-stu-id="73898-202">Int32</span></span>|<span data-ttu-id="73898-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="73898-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="73898-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73898-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="73898-205">committedContentVersion</span></span>|<span data-ttu-id="73898-206">String</span><span class="sxs-lookup"><span data-stu-id="73898-206">String</span></span>|<span data-ttu-id="73898-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="73898-207">The internal committed content version.</span></span> <span data-ttu-id="73898-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="73898-209">fileName</span><span class="sxs-lookup"><span data-stu-id="73898-209">fileName</span></span>|<span data-ttu-id="73898-210">String</span><span class="sxs-lookup"><span data-stu-id="73898-210">String</span></span>|<span data-ttu-id="73898-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="73898-211">The name of the main Lob application file.</span></span> <span data-ttu-id="73898-212">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="73898-213">size</span><span class="sxs-lookup"><span data-stu-id="73898-213">size</span></span>|<span data-ttu-id="73898-214">Int64</span><span class="sxs-lookup"><span data-stu-id="73898-214">Int64</span></span>|<span data-ttu-id="73898-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="73898-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="73898-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="73898-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="73898-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="73898-217">bundleId</span></span>|<span data-ttu-id="73898-218">String</span><span class="sxs-lookup"><span data-stu-id="73898-218">String</span></span>|<span data-ttu-id="73898-219">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="73898-219">The Identity Name.</span></span>|
|<span data-ttu-id="73898-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="73898-220">applicableDeviceType</span></span>|[<span data-ttu-id="73898-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="73898-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="73898-222">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="73898-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="73898-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="73898-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="73898-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="73898-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="73898-225">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="73898-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="73898-226">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="73898-226">expirationDateTime</span></span>|<span data-ttu-id="73898-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73898-227">DateTimeOffset</span></span>|<span data-ttu-id="73898-228">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="73898-228">The expiration time.</span></span>|
|<span data-ttu-id="73898-229">versionNumber</span><span class="sxs-lookup"><span data-stu-id="73898-229">versionNumber</span></span>|<span data-ttu-id="73898-230">String</span><span class="sxs-lookup"><span data-stu-id="73898-230">String</span></span>|<span data-ttu-id="73898-231">Номер версии бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="73898-231">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="73898-232">buildNumber</span><span class="sxs-lookup"><span data-stu-id="73898-232">buildNumber</span></span>|<span data-ttu-id="73898-233">String</span><span class="sxs-lookup"><span data-stu-id="73898-233">String</span></span>|<span data-ttu-id="73898-234">Номер сборки бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="73898-234">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="73898-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="73898-235">identityVersion</span></span>|<span data-ttu-id="73898-236">String</span><span class="sxs-lookup"><span data-stu-id="73898-236">String</span></span>|<span data-ttu-id="73898-237">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="73898-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="73898-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="73898-238">Response</span></span>
<span data-ttu-id="73898-239">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosLobApp](../resources/intune-apps-ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="73898-239">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73898-240">Пример</span><span class="sxs-lookup"><span data-stu-id="73898-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="73898-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="73898-241">Request</span></span>
<span data-ttu-id="73898-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73898-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1391

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="73898-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="73898-243">Response</span></span>
<span data-ttu-id="73898-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73898-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1563

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```





