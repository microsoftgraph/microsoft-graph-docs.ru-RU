---
title: Создание win32LobApp
description: Создание нового объекта win32LobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e10d059e907f5987710c68999d2b7a9981d03119
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328797"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="6da69-103">Создание win32LobApp</span><span class="sxs-lookup"><span data-stu-id="6da69-103">Create win32LobApp</span></span>

> <span data-ttu-id="6da69-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6da69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6da69-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6da69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6da69-106">Создание нового объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="6da69-106">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6da69-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6da69-107">Prerequisites</span></span>
<span data-ttu-id="6da69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6da69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6da69-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6da69-110">Permission type</span></span>|<span data-ttu-id="6da69-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6da69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6da69-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6da69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6da69-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6da69-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6da69-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6da69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6da69-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6da69-115">Not supported.</span></span>|
|<span data-ttu-id="6da69-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6da69-116">Application</span></span>|<span data-ttu-id="6da69-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6da69-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6da69-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6da69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6da69-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6da69-119">Request headers</span></span>
|<span data-ttu-id="6da69-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6da69-120">Header</span></span>|<span data-ttu-id="6da69-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6da69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6da69-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6da69-122">Authorization</span></span>|<span data-ttu-id="6da69-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6da69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6da69-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6da69-124">Accept</span></span>|<span data-ttu-id="6da69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6da69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6da69-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6da69-126">Request body</span></span>
<span data-ttu-id="6da69-127">В тексте запроса добавьте представление объекта win32LobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6da69-127">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="6da69-128">В следующей таблице приведены свойства, необходимые при создании win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="6da69-128">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="6da69-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6da69-129">Property</span></span>|<span data-ttu-id="6da69-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6da69-130">Type</span></span>|<span data-ttu-id="6da69-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6da69-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6da69-132">id</span><span class="sxs-lookup"><span data-stu-id="6da69-132">id</span></span>|<span data-ttu-id="6da69-133">Строка</span><span class="sxs-lookup"><span data-stu-id="6da69-133">String</span></span>|<span data-ttu-id="6da69-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6da69-134">Key of the entity.</span></span> <span data-ttu-id="6da69-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6da69-136">displayName</span></span>|<span data-ttu-id="6da69-137">Строка</span><span class="sxs-lookup"><span data-stu-id="6da69-137">String</span></span>|<span data-ttu-id="6da69-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="6da69-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6da69-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-140">description</span><span class="sxs-lookup"><span data-stu-id="6da69-140">description</span></span>|<span data-ttu-id="6da69-141">Строка</span><span class="sxs-lookup"><span data-stu-id="6da69-141">String</span></span>|<span data-ttu-id="6da69-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-142">The description of the app.</span></span> <span data-ttu-id="6da69-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-144">publisher</span><span class="sxs-lookup"><span data-stu-id="6da69-144">publisher</span></span>|<span data-ttu-id="6da69-145">String</span><span class="sxs-lookup"><span data-stu-id="6da69-145">String</span></span>|<span data-ttu-id="6da69-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-146">The publisher of the app.</span></span> <span data-ttu-id="6da69-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6da69-148">largeIcon</span></span>|[<span data-ttu-id="6da69-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6da69-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6da69-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="6da69-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6da69-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6da69-152">createdDateTime</span></span>|<span data-ttu-id="6da69-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6da69-153">DateTimeOffset</span></span>|<span data-ttu-id="6da69-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-154">The date and time the app was created.</span></span> <span data-ttu-id="6da69-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6da69-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6da69-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6da69-157">DateTimeOffset</span></span>|<span data-ttu-id="6da69-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-158">The date and time the app was last modified.</span></span> <span data-ttu-id="6da69-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6da69-160">isFeatured</span></span>|<span data-ttu-id="6da69-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6da69-161">Boolean</span></span>|<span data-ttu-id="6da69-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6da69-163">privacyInformationUrl</span></span>|<span data-ttu-id="6da69-164">String</span><span class="sxs-lookup"><span data-stu-id="6da69-164">String</span></span>|<span data-ttu-id="6da69-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="6da69-165">The privacy statement Url.</span></span> <span data-ttu-id="6da69-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6da69-167">informationUrl</span></span>|<span data-ttu-id="6da69-168">String</span><span class="sxs-lookup"><span data-stu-id="6da69-168">String</span></span>|<span data-ttu-id="6da69-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="6da69-169">The more information Url.</span></span> <span data-ttu-id="6da69-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-171">owner</span><span class="sxs-lookup"><span data-stu-id="6da69-171">owner</span></span>|<span data-ttu-id="6da69-172">String</span><span class="sxs-lookup"><span data-stu-id="6da69-172">String</span></span>|<span data-ttu-id="6da69-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-173">The owner of the app.</span></span> <span data-ttu-id="6da69-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-175">developer</span><span class="sxs-lookup"><span data-stu-id="6da69-175">developer</span></span>|<span data-ttu-id="6da69-176">String</span><span class="sxs-lookup"><span data-stu-id="6da69-176">String</span></span>|<span data-ttu-id="6da69-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-177">The developer of the app.</span></span> <span data-ttu-id="6da69-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-179">notes</span><span class="sxs-lookup"><span data-stu-id="6da69-179">notes</span></span>|<span data-ttu-id="6da69-180">String</span><span class="sxs-lookup"><span data-stu-id="6da69-180">String</span></span>|<span data-ttu-id="6da69-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-181">Notes for the app.</span></span> <span data-ttu-id="6da69-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="6da69-183">uploadState</span></span>|<span data-ttu-id="6da69-184">Int32</span><span class="sxs-lookup"><span data-stu-id="6da69-184">Int32</span></span>|<span data-ttu-id="6da69-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="6da69-185">The upload state.</span></span> <span data-ttu-id="6da69-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="6da69-187">publishingState</span></span>|[<span data-ttu-id="6da69-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="6da69-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6da69-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-189">The publishing state for the app.</span></span> <span data-ttu-id="6da69-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="6da69-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6da69-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="6da69-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6da69-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6da69-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6da69-193">isAssigned</span></span>|<span data-ttu-id="6da69-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6da69-194">Boolean</span></span>|<span data-ttu-id="6da69-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="6da69-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6da69-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6da69-197">roleScopeTagIds</span></span>|<span data-ttu-id="6da69-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6da69-198">String collection</span></span>|<span data-ttu-id="6da69-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6da69-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="6da69-201">dependentAppCount</span></span>|<span data-ttu-id="6da69-202">Int32</span><span class="sxs-lookup"><span data-stu-id="6da69-202">Int32</span></span>|<span data-ttu-id="6da69-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6da69-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6da69-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="6da69-205">committedContentVersion</span></span>|<span data-ttu-id="6da69-206">String</span><span class="sxs-lookup"><span data-stu-id="6da69-206">String</span></span>|<span data-ttu-id="6da69-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="6da69-207">The internal committed content version.</span></span> <span data-ttu-id="6da69-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6da69-209">fileName</span><span class="sxs-lookup"><span data-stu-id="6da69-209">fileName</span></span>|<span data-ttu-id="6da69-210">String</span><span class="sxs-lookup"><span data-stu-id="6da69-210">String</span></span>|<span data-ttu-id="6da69-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-211">The name of the main Lob application file.</span></span> <span data-ttu-id="6da69-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6da69-213">size</span><span class="sxs-lookup"><span data-stu-id="6da69-213">size</span></span>|<span data-ttu-id="6da69-214">Int64</span><span class="sxs-lookup"><span data-stu-id="6da69-214">Int64</span></span>|<span data-ttu-id="6da69-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="6da69-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="6da69-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6da69-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6da69-217">инсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="6da69-217">installCommandLine</span></span>|<span data-ttu-id="6da69-218">String</span><span class="sxs-lookup"><span data-stu-id="6da69-218">String</span></span>|<span data-ttu-id="6da69-219">Командная строка для установки приложения</span><span class="sxs-lookup"><span data-stu-id="6da69-219">The command line to install this app</span></span>|
|<span data-ttu-id="6da69-220">унинсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="6da69-220">uninstallCommandLine</span></span>|<span data-ttu-id="6da69-221">String</span><span class="sxs-lookup"><span data-stu-id="6da69-221">String</span></span>|<span data-ttu-id="6da69-222">Командная строка для удаления приложения</span><span class="sxs-lookup"><span data-stu-id="6da69-222">The command line to uninstall this app</span></span>|
|<span data-ttu-id="6da69-223">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="6da69-223">applicableArchitectures</span></span>|[<span data-ttu-id="6da69-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="6da69-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="6da69-225">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="6da69-225">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="6da69-226">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="6da69-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="6da69-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6da69-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6da69-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6da69-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="6da69-229">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="6da69-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="6da69-230">минимумфридискспацеинмб</span><span class="sxs-lookup"><span data-stu-id="6da69-230">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="6da69-231">Int32</span><span class="sxs-lookup"><span data-stu-id="6da69-231">Int32</span></span>|<span data-ttu-id="6da69-232">Минимальное свободное место на диске, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-232">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="6da69-233">минимуммеморинмб</span><span class="sxs-lookup"><span data-stu-id="6da69-233">minimumMemoryInMB</span></span>|<span data-ttu-id="6da69-234">Int32</span><span class="sxs-lookup"><span data-stu-id="6da69-234">Int32</span></span>|<span data-ttu-id="6da69-235">Значение минимальной физической памяти, необходимой для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-235">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="6da69-236">минимумнумберофпроцессорс</span><span class="sxs-lookup"><span data-stu-id="6da69-236">minimumNumberOfProcessors</span></span>|<span data-ttu-id="6da69-237">Int32</span><span class="sxs-lookup"><span data-stu-id="6da69-237">Int32</span></span>|<span data-ttu-id="6da69-238">Значение минимального числа процессоров, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-238">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="6da69-239">минимумкпуспидинмхз</span><span class="sxs-lookup"><span data-stu-id="6da69-239">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="6da69-240">Int32</span><span class="sxs-lookup"><span data-stu-id="6da69-240">Int32</span></span>|<span data-ttu-id="6da69-241">Значение минимальной скорости ЦП, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-241">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="6da69-242">детектионрулес</span><span class="sxs-lookup"><span data-stu-id="6da69-242">detectionRules</span></span>|<span data-ttu-id="6da69-243">Коллекция [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="6da69-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="6da69-244">Правила обнаружения для определения бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="6da69-244">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="6da69-245">рекуирементрулес</span><span class="sxs-lookup"><span data-stu-id="6da69-245">requirementRules</span></span>|<span data-ttu-id="6da69-246">Коллекция [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="6da69-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="6da69-247">Правила требований для обнаружения бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="6da69-247">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="6da69-248">инсталлекспериенце</span><span class="sxs-lookup"><span data-stu-id="6da69-248">installExperience</span></span>|[<span data-ttu-id="6da69-249">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="6da69-249">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="6da69-250">Установка приложения.</span><span class="sxs-lookup"><span data-stu-id="6da69-250">The install experience for this app.</span></span>|
|<span data-ttu-id="6da69-251">ретурнкодес</span><span class="sxs-lookup"><span data-stu-id="6da69-251">returnCodes</span></span>|<span data-ttu-id="6da69-252">Коллекция [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="6da69-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="6da69-253">Коды возврата для поведения после установки.</span><span class="sxs-lookup"><span data-stu-id="6da69-253">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="6da69-254">мсиинформатион</span><span class="sxs-lookup"><span data-stu-id="6da69-254">msiInformation</span></span>|[<span data-ttu-id="6da69-255">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="6da69-255">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="6da69-256">Сведения о MSI, если это приложение Win32 является приложением MSI.</span><span class="sxs-lookup"><span data-stu-id="6da69-256">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="6da69-257">сетупфилепас</span><span class="sxs-lookup"><span data-stu-id="6da69-257">setupFilePath</span></span>|<span data-ttu-id="6da69-258">String</span><span class="sxs-lookup"><span data-stu-id="6da69-258">String</span></span>|<span data-ttu-id="6da69-259">Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="6da69-259">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="6da69-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="6da69-260">Response</span></span>
<span data-ttu-id="6da69-261">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6da69-261">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6da69-262">Пример</span><span class="sxs-lookup"><span data-stu-id="6da69-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="6da69-263">Запрос</span><span class="sxs-lookup"><span data-stu-id="6da69-263">Request</span></span>
<span data-ttu-id="6da69-264">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6da69-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2778

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
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
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
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="6da69-265">Отклик</span><span class="sxs-lookup"><span data-stu-id="6da69-265">Response</span></span>
<span data-ttu-id="6da69-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6da69-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2950

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
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
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
  "setupFilePath": "Setup File Path value"
}
```






