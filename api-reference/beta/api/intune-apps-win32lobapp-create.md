---
title: Создание win32LobApp
description: Создание нового объекта win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc05e7b86c50018b7576a7839867d2896b590443
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791535"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="fb795-103">Создание win32LobApp</span><span class="sxs-lookup"><span data-stu-id="fb795-103">Create win32LobApp</span></span>

<span data-ttu-id="fb795-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb795-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb795-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb795-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb795-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb795-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb795-107">Создание нового объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="fb795-107">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb795-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fb795-108">Prerequisites</span></span>
<span data-ttu-id="fb795-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb795-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb795-111">Permission type</span></span>|<span data-ttu-id="fb795-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb795-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb795-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb795-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb795-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb795-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fb795-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb795-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb795-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb795-116">Not supported.</span></span>|
|<span data-ttu-id="fb795-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fb795-117">Application</span></span>|<span data-ttu-id="fb795-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb795-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb795-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb795-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fb795-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fb795-120">Request headers</span></span>
|<span data-ttu-id="fb795-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb795-121">Header</span></span>|<span data-ttu-id="fb795-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb795-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb795-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb795-123">Authorization</span></span>|<span data-ttu-id="fb795-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb795-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb795-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb795-125">Accept</span></span>|<span data-ttu-id="fb795-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb795-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb795-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb795-127">Request body</span></span>
<span data-ttu-id="fb795-128">В тексте запроса добавьте представление объекта win32LobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb795-128">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="fb795-129">В следующей таблице приведены свойства, необходимые при создании win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="fb795-129">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="fb795-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb795-130">Property</span></span>|<span data-ttu-id="fb795-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fb795-131">Type</span></span>|<span data-ttu-id="fb795-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fb795-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb795-133">id</span><span class="sxs-lookup"><span data-stu-id="fb795-133">id</span></span>|<span data-ttu-id="fb795-134">String</span><span class="sxs-lookup"><span data-stu-id="fb795-134">String</span></span>|<span data-ttu-id="fb795-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fb795-135">Key of the entity.</span></span> <span data-ttu-id="fb795-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fb795-137">displayName</span></span>|<span data-ttu-id="fb795-138">String</span><span class="sxs-lookup"><span data-stu-id="fb795-138">String</span></span>|<span data-ttu-id="fb795-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="fb795-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fb795-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-141">description</span><span class="sxs-lookup"><span data-stu-id="fb795-141">description</span></span>|<span data-ttu-id="fb795-142">String</span><span class="sxs-lookup"><span data-stu-id="fb795-142">String</span></span>|<span data-ttu-id="fb795-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-143">The description of the app.</span></span> <span data-ttu-id="fb795-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-145">publisher</span><span class="sxs-lookup"><span data-stu-id="fb795-145">publisher</span></span>|<span data-ttu-id="fb795-146">String</span><span class="sxs-lookup"><span data-stu-id="fb795-146">String</span></span>|<span data-ttu-id="fb795-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-147">The publisher of the app.</span></span> <span data-ttu-id="fb795-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fb795-149">largeIcon</span></span>|[<span data-ttu-id="fb795-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fb795-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fb795-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="fb795-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fb795-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb795-153">createdDateTime</span></span>|<span data-ttu-id="fb795-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb795-154">DateTimeOffset</span></span>|<span data-ttu-id="fb795-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-155">The date and time the app was created.</span></span> <span data-ttu-id="fb795-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb795-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fb795-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb795-158">DateTimeOffset</span></span>|<span data-ttu-id="fb795-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-159">The date and time the app was last modified.</span></span> <span data-ttu-id="fb795-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fb795-161">isFeatured</span></span>|<span data-ttu-id="fb795-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb795-162">Boolean</span></span>|<span data-ttu-id="fb795-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fb795-164">privacyInformationUrl</span></span>|<span data-ttu-id="fb795-165">String</span><span class="sxs-lookup"><span data-stu-id="fb795-165">String</span></span>|<span data-ttu-id="fb795-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="fb795-166">The privacy statement Url.</span></span> <span data-ttu-id="fb795-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fb795-168">informationUrl</span></span>|<span data-ttu-id="fb795-169">String</span><span class="sxs-lookup"><span data-stu-id="fb795-169">String</span></span>|<span data-ttu-id="fb795-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="fb795-170">The more information Url.</span></span> <span data-ttu-id="fb795-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-172">owner</span><span class="sxs-lookup"><span data-stu-id="fb795-172">owner</span></span>|<span data-ttu-id="fb795-173">String</span><span class="sxs-lookup"><span data-stu-id="fb795-173">String</span></span>|<span data-ttu-id="fb795-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-174">The owner of the app.</span></span> <span data-ttu-id="fb795-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-176">developer</span><span class="sxs-lookup"><span data-stu-id="fb795-176">developer</span></span>|<span data-ttu-id="fb795-177">String</span><span class="sxs-lookup"><span data-stu-id="fb795-177">String</span></span>|<span data-ttu-id="fb795-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-178">The developer of the app.</span></span> <span data-ttu-id="fb795-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-180">notes</span><span class="sxs-lookup"><span data-stu-id="fb795-180">notes</span></span>|<span data-ttu-id="fb795-181">String</span><span class="sxs-lookup"><span data-stu-id="fb795-181">String</span></span>|<span data-ttu-id="fb795-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-182">Notes for the app.</span></span> <span data-ttu-id="fb795-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="fb795-184">uploadState</span></span>|<span data-ttu-id="fb795-185">Int32</span><span class="sxs-lookup"><span data-stu-id="fb795-185">Int32</span></span>|<span data-ttu-id="fb795-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="fb795-186">The upload state.</span></span> <span data-ttu-id="fb795-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="fb795-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="fb795-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="fb795-189">publishingState</span></span>|[<span data-ttu-id="fb795-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="fb795-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fb795-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-191">The publishing state for the app.</span></span> <span data-ttu-id="fb795-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="fb795-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fb795-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="fb795-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fb795-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fb795-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fb795-195">isAssigned</span></span>|<span data-ttu-id="fb795-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb795-196">Boolean</span></span>|<span data-ttu-id="fb795-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="fb795-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="fb795-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fb795-199">roleScopeTagIds</span></span>|<span data-ttu-id="fb795-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fb795-200">String collection</span></span>|<span data-ttu-id="fb795-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="fb795-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="fb795-203">dependentAppCount</span></span>|<span data-ttu-id="fb795-204">Int32</span><span class="sxs-lookup"><span data-stu-id="fb795-204">Int32</span></span>|<span data-ttu-id="fb795-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="fb795-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb795-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fb795-207">committedContentVersion</span></span>|<span data-ttu-id="fb795-208">String</span><span class="sxs-lookup"><span data-stu-id="fb795-208">String</span></span>|<span data-ttu-id="fb795-209">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="fb795-209">The internal committed content version.</span></span> <span data-ttu-id="fb795-210">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fb795-211">fileName</span><span class="sxs-lookup"><span data-stu-id="fb795-211">fileName</span></span>|<span data-ttu-id="fb795-212">String</span><span class="sxs-lookup"><span data-stu-id="fb795-212">String</span></span>|<span data-ttu-id="fb795-213">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-213">The name of the main Lob application file.</span></span> <span data-ttu-id="fb795-214">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fb795-215">size</span><span class="sxs-lookup"><span data-stu-id="fb795-215">size</span></span>|<span data-ttu-id="fb795-216">Int64</span><span class="sxs-lookup"><span data-stu-id="fb795-216">Int64</span></span>|<span data-ttu-id="fb795-217">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="fb795-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="fb795-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb795-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fb795-219">инсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="fb795-219">installCommandLine</span></span>|<span data-ttu-id="fb795-220">String</span><span class="sxs-lookup"><span data-stu-id="fb795-220">String</span></span>|<span data-ttu-id="fb795-221">Командная строка для установки приложения</span><span class="sxs-lookup"><span data-stu-id="fb795-221">The command line to install this app</span></span>|
|<span data-ttu-id="fb795-222">унинсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="fb795-222">uninstallCommandLine</span></span>|<span data-ttu-id="fb795-223">String</span><span class="sxs-lookup"><span data-stu-id="fb795-223">String</span></span>|<span data-ttu-id="fb795-224">Командная строка для удаления приложения</span><span class="sxs-lookup"><span data-stu-id="fb795-224">The command line to uninstall this app</span></span>|
|<span data-ttu-id="fb795-225">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="fb795-225">applicableArchitectures</span></span>|[<span data-ttu-id="fb795-226">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="fb795-226">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="fb795-227">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="fb795-227">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="fb795-228">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="fb795-228">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="fb795-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fb795-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fb795-230">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fb795-230">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="fb795-231">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="fb795-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="fb795-232">минимумфридискспацеинмб</span><span class="sxs-lookup"><span data-stu-id="fb795-232">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="fb795-233">Int32</span><span class="sxs-lookup"><span data-stu-id="fb795-233">Int32</span></span>|<span data-ttu-id="fb795-234">Минимальное свободное место на диске, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-234">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="fb795-235">минимуммеморинмб</span><span class="sxs-lookup"><span data-stu-id="fb795-235">minimumMemoryInMB</span></span>|<span data-ttu-id="fb795-236">Int32</span><span class="sxs-lookup"><span data-stu-id="fb795-236">Int32</span></span>|<span data-ttu-id="fb795-237">Значение минимальной физической памяти, необходимой для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-237">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="fb795-238">минимумнумберофпроцессорс</span><span class="sxs-lookup"><span data-stu-id="fb795-238">minimumNumberOfProcessors</span></span>|<span data-ttu-id="fb795-239">Int32</span><span class="sxs-lookup"><span data-stu-id="fb795-239">Int32</span></span>|<span data-ttu-id="fb795-240">Значение минимального числа процессоров, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-240">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="fb795-241">минимумкпуспидинмхз</span><span class="sxs-lookup"><span data-stu-id="fb795-241">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="fb795-242">Int32</span><span class="sxs-lookup"><span data-stu-id="fb795-242">Int32</span></span>|<span data-ttu-id="fb795-243">Значение минимальной скорости ЦП, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-243">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="fb795-244">детектионрулес</span><span class="sxs-lookup"><span data-stu-id="fb795-244">detectionRules</span></span>|<span data-ttu-id="fb795-245">Коллекция [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="fb795-245">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="fb795-246">Правила обнаружения для определения бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="fb795-246">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="fb795-247">рекуирементрулес</span><span class="sxs-lookup"><span data-stu-id="fb795-247">requirementRules</span></span>|<span data-ttu-id="fb795-248">Коллекция [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="fb795-248">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="fb795-249">Правила требований для обнаружения бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="fb795-249">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="fb795-250">правила</span><span class="sxs-lookup"><span data-stu-id="fb795-250">rules</span></span>|<span data-ttu-id="fb795-251">Коллекция [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="fb795-251">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="fb795-252">Правила обнаружения и требований для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-252">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="fb795-253">инсталлекспериенце</span><span class="sxs-lookup"><span data-stu-id="fb795-253">installExperience</span></span>|[<span data-ttu-id="fb795-254">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="fb795-254">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="fb795-255">Установка приложения.</span><span class="sxs-lookup"><span data-stu-id="fb795-255">The install experience for this app.</span></span>|
|<span data-ttu-id="fb795-256">ретурнкодес</span><span class="sxs-lookup"><span data-stu-id="fb795-256">returnCodes</span></span>|<span data-ttu-id="fb795-257">Коллекция [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="fb795-257">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="fb795-258">Коды возврата для поведения после установки.</span><span class="sxs-lookup"><span data-stu-id="fb795-258">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="fb795-259">мсиинформатион</span><span class="sxs-lookup"><span data-stu-id="fb795-259">msiInformation</span></span>|[<span data-ttu-id="fb795-260">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="fb795-260">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="fb795-261">Сведения о MSI, если это приложение Win32 является приложением MSI.</span><span class="sxs-lookup"><span data-stu-id="fb795-261">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="fb795-262">сетупфилепас</span><span class="sxs-lookup"><span data-stu-id="fb795-262">setupFilePath</span></span>|<span data-ttu-id="fb795-263">String</span><span class="sxs-lookup"><span data-stu-id="fb795-263">String</span></span>|<span data-ttu-id="fb795-264">Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="fb795-264">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="fb795-265">installLanguage</span><span class="sxs-lookup"><span data-stu-id="fb795-265">installLanguage</span></span>|<span data-ttu-id="fb795-266">String</span><span class="sxs-lookup"><span data-stu-id="fb795-266">String</span></span>|<span data-ttu-id="fb795-267">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="fb795-267">Not yet documented</span></span>|
|<span data-ttu-id="fb795-268">минимумсуппортедвиндовсрелеасе</span><span class="sxs-lookup"><span data-stu-id="fb795-268">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="fb795-269">String</span><span class="sxs-lookup"><span data-stu-id="fb795-269">String</span></span>|<span data-ttu-id="fb795-270">Значение минимального поддерживаемого выпуска Windows.</span><span class="sxs-lookup"><span data-stu-id="fb795-270">The value for the minimum supported windows release.</span></span>|



## <a name="response"></a><span data-ttu-id="fb795-271">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb795-271">Response</span></span>
<span data-ttu-id="fb795-272">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb795-272">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb795-273">Пример</span><span class="sxs-lookup"><span data-stu-id="fb795-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb795-274">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb795-274">Request</span></span>
<span data-ttu-id="fb795-275">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb795-275">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 3304

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "installLanguage": "Install Language value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```

### <a name="response"></a><span data-ttu-id="fb795-276">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb795-276">Response</span></span>
<span data-ttu-id="fb795-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb795-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3476

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "installLanguage": "Install Language value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```



