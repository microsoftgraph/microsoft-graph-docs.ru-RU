---
title: Create iosLobApp
description: Создание нового объекта iosLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b33d36a16c375bc80524f4696bb3fc459834fe46
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32496207"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="5d92c-103">Create iosLobApp</span><span class="sxs-lookup"><span data-stu-id="5d92c-103">Create iosLobApp</span></span>

> <span data-ttu-id="5d92c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d92c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d92c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d92c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d92c-106">Создание нового объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-106">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d92c-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5d92c-107">Prerequisites</span></span>
<span data-ttu-id="5d92c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d92c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d92c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d92c-110">Permission type</span></span>|<span data-ttu-id="5d92c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d92c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d92c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d92c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5d92c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d92c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5d92c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d92c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d92c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d92c-115">Not supported.</span></span>|
|<span data-ttu-id="5d92c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d92c-116">Application</span></span>|<span data-ttu-id="5d92c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d92c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d92c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d92c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5d92c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d92c-119">Request headers</span></span>
|<span data-ttu-id="5d92c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d92c-120">Header</span></span>|<span data-ttu-id="5d92c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5d92c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d92c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d92c-122">Authorization</span></span>|<span data-ttu-id="5d92c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d92c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d92c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5d92c-124">Accept</span></span>|<span data-ttu-id="5d92c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5d92c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d92c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d92c-126">Request body</span></span>
<span data-ttu-id="5d92c-127">В теле запроса добавьте представление объекта iosLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d92c-127">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="5d92c-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="5d92c-128">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="5d92c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d92c-129">Property</span></span>|<span data-ttu-id="5d92c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5d92c-130">Type</span></span>|<span data-ttu-id="5d92c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5d92c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d92c-132">id</span><span class="sxs-lookup"><span data-stu-id="5d92c-132">id</span></span>|<span data-ttu-id="5d92c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5d92c-133">String</span></span>|<span data-ttu-id="5d92c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5d92c-134">Key of the entity.</span></span> <span data-ttu-id="5d92c-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5d92c-136">displayName</span></span>|<span data-ttu-id="5d92c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="5d92c-137">String</span></span>|<span data-ttu-id="5d92c-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="5d92c-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5d92c-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-140">description</span><span class="sxs-lookup"><span data-stu-id="5d92c-140">description</span></span>|<span data-ttu-id="5d92c-141">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-141">String</span></span>|<span data-ttu-id="5d92c-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-142">The description of the app.</span></span> <span data-ttu-id="5d92c-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-144">publisher</span><span class="sxs-lookup"><span data-stu-id="5d92c-144">publisher</span></span>|<span data-ttu-id="5d92c-145">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-145">String</span></span>|<span data-ttu-id="5d92c-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-146">The publisher of the app.</span></span> <span data-ttu-id="5d92c-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5d92c-148">largeIcon</span></span>|[<span data-ttu-id="5d92c-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5d92c-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5d92c-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="5d92c-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5d92c-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d92c-152">createdDateTime</span></span>|<span data-ttu-id="5d92c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d92c-153">DateTimeOffset</span></span>|<span data-ttu-id="5d92c-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-154">The date and time the app was created.</span></span> <span data-ttu-id="5d92c-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d92c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="5d92c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d92c-157">DateTimeOffset</span></span>|<span data-ttu-id="5d92c-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-158">The date and time the app was last modified.</span></span> <span data-ttu-id="5d92c-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5d92c-160">isFeatured</span></span>|<span data-ttu-id="5d92c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d92c-161">Boolean</span></span>|<span data-ttu-id="5d92c-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5d92c-163">privacyInformationUrl</span></span>|<span data-ttu-id="5d92c-164">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-164">String</span></span>|<span data-ttu-id="5d92c-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5d92c-165">The privacy statement Url.</span></span> <span data-ttu-id="5d92c-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5d92c-167">informationUrl</span></span>|<span data-ttu-id="5d92c-168">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-168">String</span></span>|<span data-ttu-id="5d92c-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5d92c-169">The more information Url.</span></span> <span data-ttu-id="5d92c-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-171">owner</span><span class="sxs-lookup"><span data-stu-id="5d92c-171">owner</span></span>|<span data-ttu-id="5d92c-172">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-172">String</span></span>|<span data-ttu-id="5d92c-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-173">The owner of the app.</span></span> <span data-ttu-id="5d92c-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-175">developer</span><span class="sxs-lookup"><span data-stu-id="5d92c-175">developer</span></span>|<span data-ttu-id="5d92c-176">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-176">String</span></span>|<span data-ttu-id="5d92c-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-177">The developer of the app.</span></span> <span data-ttu-id="5d92c-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-179">notes</span><span class="sxs-lookup"><span data-stu-id="5d92c-179">notes</span></span>|<span data-ttu-id="5d92c-180">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-180">String</span></span>|<span data-ttu-id="5d92c-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-181">Notes for the app.</span></span> <span data-ttu-id="5d92c-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="5d92c-183">uploadState</span></span>|<span data-ttu-id="5d92c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="5d92c-184">Int32</span></span>|<span data-ttu-id="5d92c-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="5d92c-185">The upload state.</span></span> <span data-ttu-id="5d92c-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="5d92c-187">publishingState</span></span>|[<span data-ttu-id="5d92c-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="5d92c-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5d92c-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-189">The publishing state for the app.</span></span> <span data-ttu-id="5d92c-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="5d92c-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5d92c-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5d92c-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5d92c-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5d92c-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5d92c-193">isAssigned</span></span>|<span data-ttu-id="5d92c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d92c-194">Boolean</span></span>|<span data-ttu-id="5d92c-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="5d92c-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5d92c-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5d92c-197">roleScopeTagIds</span></span>|<span data-ttu-id="5d92c-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5d92c-198">String collection</span></span>|<span data-ttu-id="5d92c-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5d92c-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="5d92c-201">dependentAppCount</span></span>|<span data-ttu-id="5d92c-202">Int32</span><span class="sxs-lookup"><span data-stu-id="5d92c-202">Int32</span></span>|<span data-ttu-id="5d92c-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="5d92c-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5d92c-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5d92c-205">committedContentVersion</span></span>|<span data-ttu-id="5d92c-206">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-206">String</span></span>|<span data-ttu-id="5d92c-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="5d92c-207">The internal committed content version.</span></span> <span data-ttu-id="5d92c-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5d92c-209">fileName</span><span class="sxs-lookup"><span data-stu-id="5d92c-209">fileName</span></span>|<span data-ttu-id="5d92c-210">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-210">String</span></span>|<span data-ttu-id="5d92c-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-211">The name of the main Lob application file.</span></span> <span data-ttu-id="5d92c-212">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5d92c-213">size</span><span class="sxs-lookup"><span data-stu-id="5d92c-213">size</span></span>|<span data-ttu-id="5d92c-214">Int64</span><span class="sxs-lookup"><span data-stu-id="5d92c-214">Int64</span></span>|<span data-ttu-id="5d92c-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="5d92c-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="5d92c-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d92c-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5d92c-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="5d92c-217">bundleId</span></span>|<span data-ttu-id="5d92c-218">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-218">String</span></span>|<span data-ttu-id="5d92c-219">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-219">The Identity Name.</span></span>|
|<span data-ttu-id="5d92c-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="5d92c-220">applicableDeviceType</span></span>|[<span data-ttu-id="5d92c-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="5d92c-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="5d92c-222">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="5d92c-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="5d92c-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5d92c-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5d92c-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5d92c-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="5d92c-225">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="5d92c-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="5d92c-226">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5d92c-226">expirationDateTime</span></span>|<span data-ttu-id="5d92c-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d92c-227">DateTimeOffset</span></span>|<span data-ttu-id="5d92c-228">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="5d92c-228">The expiration time.</span></span>|
|<span data-ttu-id="5d92c-229">versionNumber</span><span class="sxs-lookup"><span data-stu-id="5d92c-229">versionNumber</span></span>|<span data-ttu-id="5d92c-230">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-230">String</span></span>|<span data-ttu-id="5d92c-231">Номер версии бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="5d92c-231">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5d92c-232">buildNumber</span><span class="sxs-lookup"><span data-stu-id="5d92c-232">buildNumber</span></span>|<span data-ttu-id="5d92c-233">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-233">String</span></span>|<span data-ttu-id="5d92c-234">Номер сборки бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="5d92c-234">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5d92c-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="5d92c-235">identityVersion</span></span>|<span data-ttu-id="5d92c-236">String</span><span class="sxs-lookup"><span data-stu-id="5d92c-236">String</span></span>|<span data-ttu-id="5d92c-237">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="5d92c-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="5d92c-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="5d92c-238">Response</span></span>
<span data-ttu-id="5d92c-239">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosLobApp](../resources/intune-apps-ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5d92c-239">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d92c-240">Пример</span><span class="sxs-lookup"><span data-stu-id="5d92c-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d92c-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d92c-241">Request</span></span>
<span data-ttu-id="5d92c-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d92c-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5d92c-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d92c-243">Response</span></span>
<span data-ttu-id="5d92c-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d92c-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





