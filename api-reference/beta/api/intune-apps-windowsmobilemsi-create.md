---
title: Create windowsMobileMSI
description: Создание объекта windowsMobileMSI.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 175b8d4cbeda00dcd1da6e9e8ab3aa262f111e4c
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535053"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="35f5e-103">Create windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="35f5e-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="35f5e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35f5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35f5e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35f5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35f5e-106">Создание объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-106">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35f5e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="35f5e-107">Prerequisites</span></span>
<span data-ttu-id="35f5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35f5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35f5e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35f5e-110">Permission type</span></span>|<span data-ttu-id="35f5e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35f5e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35f5e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35f5e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35f5e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35f5e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="35f5e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35f5e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35f5e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35f5e-115">Not supported.</span></span>|
|<span data-ttu-id="35f5e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="35f5e-116">Application</span></span>|<span data-ttu-id="35f5e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35f5e-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35f5e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35f5e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="35f5e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35f5e-119">Request headers</span></span>
|<span data-ttu-id="35f5e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35f5e-120">Header</span></span>|<span data-ttu-id="35f5e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="35f5e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35f5e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35f5e-122">Authorization</span></span>|<span data-ttu-id="35f5e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35f5e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35f5e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="35f5e-124">Accept</span></span>|<span data-ttu-id="35f5e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35f5e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35f5e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35f5e-126">Request body</span></span>
<span data-ttu-id="35f5e-127">В тексте запроса добавьте представление объекта windowsMobileMSI в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35f5e-127">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="35f5e-128">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="35f5e-128">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="35f5e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="35f5e-129">Property</span></span>|<span data-ttu-id="35f5e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="35f5e-130">Type</span></span>|<span data-ttu-id="35f5e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="35f5e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35f5e-132">id</span><span class="sxs-lookup"><span data-stu-id="35f5e-132">id</span></span>|<span data-ttu-id="35f5e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="35f5e-133">String</span></span>|<span data-ttu-id="35f5e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="35f5e-134">Key of the entity.</span></span> <span data-ttu-id="35f5e-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="35f5e-136">displayName</span></span>|<span data-ttu-id="35f5e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="35f5e-137">String</span></span>|<span data-ttu-id="35f5e-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="35f5e-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="35f5e-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-140">description</span><span class="sxs-lookup"><span data-stu-id="35f5e-140">description</span></span>|<span data-ttu-id="35f5e-141">Строка</span><span class="sxs-lookup"><span data-stu-id="35f5e-141">String</span></span>|<span data-ttu-id="35f5e-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="35f5e-142">The description of the app.</span></span> <span data-ttu-id="35f5e-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-144">publisher</span><span class="sxs-lookup"><span data-stu-id="35f5e-144">publisher</span></span>|<span data-ttu-id="35f5e-145">String</span><span class="sxs-lookup"><span data-stu-id="35f5e-145">String</span></span>|<span data-ttu-id="35f5e-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="35f5e-146">The publisher of the app.</span></span> <span data-ttu-id="35f5e-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="35f5e-148">largeIcon</span></span>|[<span data-ttu-id="35f5e-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="35f5e-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="35f5e-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="35f5e-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="35f5e-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35f5e-152">createdDateTime</span></span>|<span data-ttu-id="35f5e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f5e-153">DateTimeOffset</span></span>|<span data-ttu-id="35f5e-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="35f5e-154">The date and time the app was created.</span></span> <span data-ttu-id="35f5e-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35f5e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="35f5e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f5e-157">DateTimeOffset</span></span>|<span data-ttu-id="35f5e-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="35f5e-158">The date and time the app was last modified.</span></span> <span data-ttu-id="35f5e-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="35f5e-160">isFeatured</span></span>|<span data-ttu-id="35f5e-161">Логический</span><span class="sxs-lookup"><span data-stu-id="35f5e-161">Boolean</span></span>|<span data-ttu-id="35f5e-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="35f5e-163">privacyInformationUrl</span></span>|<span data-ttu-id="35f5e-164">String</span><span class="sxs-lookup"><span data-stu-id="35f5e-164">String</span></span>|<span data-ttu-id="35f5e-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="35f5e-165">The privacy statement Url.</span></span> <span data-ttu-id="35f5e-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="35f5e-167">informationUrl</span></span>|<span data-ttu-id="35f5e-168">String</span><span class="sxs-lookup"><span data-stu-id="35f5e-168">String</span></span>|<span data-ttu-id="35f5e-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="35f5e-169">The more information Url.</span></span> <span data-ttu-id="35f5e-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-171">owner</span><span class="sxs-lookup"><span data-stu-id="35f5e-171">owner</span></span>|<span data-ttu-id="35f5e-172">String</span><span class="sxs-lookup"><span data-stu-id="35f5e-172">String</span></span>|<span data-ttu-id="35f5e-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="35f5e-173">The owner of the app.</span></span> <span data-ttu-id="35f5e-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-175">developer</span><span class="sxs-lookup"><span data-stu-id="35f5e-175">developer</span></span>|<span data-ttu-id="35f5e-176">String</span><span class="sxs-lookup"><span data-stu-id="35f5e-176">String</span></span>|<span data-ttu-id="35f5e-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="35f5e-177">The developer of the app.</span></span> <span data-ttu-id="35f5e-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-179">notes</span><span class="sxs-lookup"><span data-stu-id="35f5e-179">notes</span></span>|<span data-ttu-id="35f5e-180">String</span><span class="sxs-lookup"><span data-stu-id="35f5e-180">String</span></span>|<span data-ttu-id="35f5e-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="35f5e-181">Notes for the app.</span></span> <span data-ttu-id="35f5e-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="35f5e-183">uploadState</span></span>|<span data-ttu-id="35f5e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="35f5e-184">Int32</span></span>|<span data-ttu-id="35f5e-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="35f5e-185">The upload state.</span></span> <span data-ttu-id="35f5e-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="35f5e-187">publishingState</span></span>|[<span data-ttu-id="35f5e-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="35f5e-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="35f5e-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="35f5e-189">The publishing state for the app.</span></span> <span data-ttu-id="35f5e-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="35f5e-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="35f5e-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="35f5e-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="35f5e-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="35f5e-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="35f5e-193">isAssigned</span></span>|<span data-ttu-id="35f5e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f5e-194">Boolean</span></span>|<span data-ttu-id="35f5e-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="35f5e-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="35f5e-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35f5e-197">roleScopeTagIds</span></span>|<span data-ttu-id="35f5e-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="35f5e-198">String collection</span></span>|<span data-ttu-id="35f5e-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="35f5e-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="35f5e-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="35f5e-201">dependentAppCount</span></span>|<span data-ttu-id="35f5e-202">Int32</span><span class="sxs-lookup"><span data-stu-id="35f5e-202">Int32</span></span>|<span data-ttu-id="35f5e-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="35f5e-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="35f5e-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f5e-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="35f5e-205">committedContentVersion</span></span>|<span data-ttu-id="35f5e-206">String</span><span class="sxs-lookup"><span data-stu-id="35f5e-206">String</span></span>|<span data-ttu-id="35f5e-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="35f5e-207">The internal committed content version.</span></span> <span data-ttu-id="35f5e-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="35f5e-209">fileName</span><span class="sxs-lookup"><span data-stu-id="35f5e-209">fileName</span></span>|<span data-ttu-id="35f5e-210">String</span><span class="sxs-lookup"><span data-stu-id="35f5e-210">String</span></span>|<span data-ttu-id="35f5e-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="35f5e-211">The name of the main Lob application file.</span></span> <span data-ttu-id="35f5e-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="35f5e-213">size</span><span class="sxs-lookup"><span data-stu-id="35f5e-213">size</span></span>|<span data-ttu-id="35f5e-214">Int64</span><span class="sxs-lookup"><span data-stu-id="35f5e-214">Int64</span></span>|<span data-ttu-id="35f5e-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="35f5e-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="35f5e-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="35f5e-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="35f5e-217">commandLine</span><span class="sxs-lookup"><span data-stu-id="35f5e-217">commandLine</span></span>|<span data-ttu-id="35f5e-218">String</span><span class="sxs-lookup"><span data-stu-id="35f5e-218">String</span></span>|<span data-ttu-id="35f5e-219">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="35f5e-219">The command line.</span></span>|
|<span data-ttu-id="35f5e-220">productCode</span><span class="sxs-lookup"><span data-stu-id="35f5e-220">productCode</span></span>|<span data-ttu-id="35f5e-221">String</span><span class="sxs-lookup"><span data-stu-id="35f5e-221">String</span></span>|<span data-ttu-id="35f5e-222">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="35f5e-222">The product code.</span></span>|
|<span data-ttu-id="35f5e-223">productVersion</span><span class="sxs-lookup"><span data-stu-id="35f5e-223">productVersion</span></span>|<span data-ttu-id="35f5e-224">String</span><span class="sxs-lookup"><span data-stu-id="35f5e-224">String</span></span>|<span data-ttu-id="35f5e-225">Версия бизнес-приложения, к которому применяется MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="35f5e-225">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="35f5e-226">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="35f5e-226">ignoreVersionDetection</span></span>|<span data-ttu-id="35f5e-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f5e-227">Boolean</span></span>|<span data-ttu-id="35f5e-228">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="35f5e-228">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="35f5e-229">Задайте значение true для бизнес-приложений MSI для Windows Mobile с функцией самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="35f5e-229">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="35f5e-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="35f5e-230">identityVersion</span></span>|<span data-ttu-id="35f5e-231">String</span><span class="sxs-lookup"><span data-stu-id="35f5e-231">String</span></span>|<span data-ttu-id="35f5e-232">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="35f5e-232">The identity version.</span></span>|
|<span data-ttu-id="35f5e-233">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="35f5e-233">useDeviceContext</span></span>|<span data-ttu-id="35f5e-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f5e-234">Boolean</span></span>|<span data-ttu-id="35f5e-235">Указывает, следует ли установить MSI с двойным режимом в контексте устройства.</span><span class="sxs-lookup"><span data-stu-id="35f5e-235">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="35f5e-236">Если задано значение true, приложение будет установлено для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="35f5e-236">If true, app will be installed for all users.</span></span> <span data-ttu-id="35f5e-237">Если задано значение false, приложение будет установлено для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="35f5e-237">If false, app will be installed per-user.</span></span> <span data-ttu-id="35f5e-238">Если значение равно null, служба будет использовать стандартный контекст установки пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="35f5e-238">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="35f5e-239">В случае с двойным режимом MSI это значение по умолчанию будет иметь значение "на пользователя".</span><span class="sxs-lookup"><span data-stu-id="35f5e-239">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="35f5e-240">Не может быть задано для приложений с несдвоенным режимом.</span><span class="sxs-lookup"><span data-stu-id="35f5e-240">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="35f5e-241">После первоначального создания приложения его невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="35f5e-241">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="35f5e-242">Ответ</span><span class="sxs-lookup"><span data-stu-id="35f5e-242">Response</span></span>
<span data-ttu-id="35f5e-243">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="35f5e-243">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35f5e-244">Пример</span><span class="sxs-lookup"><span data-stu-id="35f5e-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="35f5e-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="35f5e-245">Request</span></span>
<span data-ttu-id="35f5e-246">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35f5e-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1066

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="35f5e-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="35f5e-247">Response</span></span>
<span data-ttu-id="35f5e-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35f5e-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1238

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```






