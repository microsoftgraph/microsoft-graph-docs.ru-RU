---
title: Create windowsUniversalAppX
description: Создание объекта windowsUniversalAppX.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 317667869e49683ccb4b41196fd23be21df2322a
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791857"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="e5d23-103">Create windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="e5d23-103">Create windowsUniversalAppX</span></span>

<span data-ttu-id="e5d23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5d23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5d23-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5d23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5d23-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5d23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5d23-107">Создание объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-107">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5d23-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e5d23-108">Prerequisites</span></span>
<span data-ttu-id="e5d23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5d23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5d23-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5d23-111">Permission type</span></span>|<span data-ttu-id="e5d23-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5d23-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5d23-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5d23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5d23-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5d23-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5d23-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5d23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5d23-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5d23-116">Not supported.</span></span>|
|<span data-ttu-id="e5d23-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e5d23-117">Application</span></span>|<span data-ttu-id="e5d23-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5d23-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5d23-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5d23-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e5d23-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e5d23-120">Request headers</span></span>
|<span data-ttu-id="e5d23-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5d23-121">Header</span></span>|<span data-ttu-id="e5d23-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5d23-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5d23-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5d23-123">Authorization</span></span>|<span data-ttu-id="e5d23-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5d23-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5d23-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5d23-125">Accept</span></span>|<span data-ttu-id="e5d23-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5d23-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5d23-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5d23-127">Request body</span></span>
<span data-ttu-id="e5d23-128">В тексте запроса добавьте представление объекта windowsUniversalAppX в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5d23-128">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="e5d23-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="e5d23-129">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="e5d23-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5d23-130">Property</span></span>|<span data-ttu-id="e5d23-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e5d23-131">Type</span></span>|<span data-ttu-id="e5d23-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e5d23-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5d23-133">id</span><span class="sxs-lookup"><span data-stu-id="e5d23-133">id</span></span>|<span data-ttu-id="e5d23-134">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-134">String</span></span>|<span data-ttu-id="e5d23-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e5d23-135">Key of the entity.</span></span> <span data-ttu-id="e5d23-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e5d23-137">displayName</span></span>|<span data-ttu-id="e5d23-138">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-138">String</span></span>|<span data-ttu-id="e5d23-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e5d23-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e5d23-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-141">description</span><span class="sxs-lookup"><span data-stu-id="e5d23-141">description</span></span>|<span data-ttu-id="e5d23-142">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-142">String</span></span>|<span data-ttu-id="e5d23-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-143">The description of the app.</span></span> <span data-ttu-id="e5d23-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e5d23-145">publisher</span></span>|<span data-ttu-id="e5d23-146">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-146">String</span></span>|<span data-ttu-id="e5d23-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-147">The publisher of the app.</span></span> <span data-ttu-id="e5d23-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e5d23-149">largeIcon</span></span>|[<span data-ttu-id="e5d23-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e5d23-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e5d23-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e5d23-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e5d23-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5d23-153">createdDateTime</span></span>|<span data-ttu-id="e5d23-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5d23-154">DateTimeOffset</span></span>|<span data-ttu-id="e5d23-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-155">The date and time the app was created.</span></span> <span data-ttu-id="e5d23-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5d23-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e5d23-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5d23-158">DateTimeOffset</span></span>|<span data-ttu-id="e5d23-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e5d23-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e5d23-161">isFeatured</span></span>|<span data-ttu-id="e5d23-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5d23-162">Boolean</span></span>|<span data-ttu-id="e5d23-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e5d23-164">privacyInformationUrl</span></span>|<span data-ttu-id="e5d23-165">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-165">String</span></span>|<span data-ttu-id="e5d23-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e5d23-166">The privacy statement Url.</span></span> <span data-ttu-id="e5d23-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e5d23-168">informationUrl</span></span>|<span data-ttu-id="e5d23-169">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-169">String</span></span>|<span data-ttu-id="e5d23-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e5d23-170">The more information Url.</span></span> <span data-ttu-id="e5d23-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-172">owner</span><span class="sxs-lookup"><span data-stu-id="e5d23-172">owner</span></span>|<span data-ttu-id="e5d23-173">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-173">String</span></span>|<span data-ttu-id="e5d23-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-174">The owner of the app.</span></span> <span data-ttu-id="e5d23-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-176">developer</span><span class="sxs-lookup"><span data-stu-id="e5d23-176">developer</span></span>|<span data-ttu-id="e5d23-177">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-177">String</span></span>|<span data-ttu-id="e5d23-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-178">The developer of the app.</span></span> <span data-ttu-id="e5d23-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-180">notes</span><span class="sxs-lookup"><span data-stu-id="e5d23-180">notes</span></span>|<span data-ttu-id="e5d23-181">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-181">String</span></span>|<span data-ttu-id="e5d23-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-182">Notes for the app.</span></span> <span data-ttu-id="e5d23-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e5d23-184">uploadState</span></span>|<span data-ttu-id="e5d23-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e5d23-185">Int32</span></span>|<span data-ttu-id="e5d23-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="e5d23-186">The upload state.</span></span> <span data-ttu-id="e5d23-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="e5d23-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="e5d23-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="e5d23-189">publishingState</span></span>|[<span data-ttu-id="e5d23-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="e5d23-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e5d23-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-191">The publishing state for the app.</span></span> <span data-ttu-id="e5d23-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e5d23-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e5d23-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e5d23-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e5d23-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e5d23-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e5d23-195">isAssigned</span></span>|<span data-ttu-id="e5d23-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5d23-196">Boolean</span></span>|<span data-ttu-id="e5d23-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="e5d23-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e5d23-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5d23-199">roleScopeTagIds</span></span>|<span data-ttu-id="e5d23-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e5d23-200">String collection</span></span>|<span data-ttu-id="e5d23-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e5d23-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="e5d23-203">dependentAppCount</span></span>|<span data-ttu-id="e5d23-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e5d23-204">Int32</span></span>|<span data-ttu-id="e5d23-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e5d23-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e5d23-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e5d23-207">committedContentVersion</span></span>|<span data-ttu-id="e5d23-208">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-208">String</span></span>|<span data-ttu-id="e5d23-209">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="e5d23-209">The internal committed content version.</span></span> <span data-ttu-id="e5d23-210">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e5d23-211">fileName</span><span class="sxs-lookup"><span data-stu-id="e5d23-211">fileName</span></span>|<span data-ttu-id="e5d23-212">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-212">String</span></span>|<span data-ttu-id="e5d23-213">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-213">The name of the main Lob application file.</span></span> <span data-ttu-id="e5d23-214">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e5d23-215">size</span><span class="sxs-lookup"><span data-stu-id="e5d23-215">size</span></span>|<span data-ttu-id="e5d23-216">Int64</span><span class="sxs-lookup"><span data-stu-id="e5d23-216">Int64</span></span>|<span data-ttu-id="e5d23-217">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="e5d23-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="e5d23-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5d23-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e5d23-219">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="e5d23-219">applicableArchitectures</span></span>|[<span data-ttu-id="e5d23-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e5d23-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e5d23-221">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="e5d23-221">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="e5d23-222">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="e5d23-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="e5d23-223">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="e5d23-223">applicableDeviceTypes</span></span>|[<span data-ttu-id="e5d23-224">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="e5d23-224">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="e5d23-225">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="e5d23-225">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="e5d23-226">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="e5d23-226">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="e5d23-227">identityName</span><span class="sxs-lookup"><span data-stu-id="e5d23-227">identityName</span></span>|<span data-ttu-id="e5d23-228">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-228">String</span></span>|<span data-ttu-id="e5d23-229">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-229">The Identity Name.</span></span>|
|<span data-ttu-id="e5d23-230">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="e5d23-230">identityPublisherHash</span></span>|<span data-ttu-id="e5d23-231">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-231">String</span></span>|<span data-ttu-id="e5d23-232">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="e5d23-232">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="e5d23-233">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e5d23-233">identityResourceIdentifier</span></span>|<span data-ttu-id="e5d23-234">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-234">String</span></span>|<span data-ttu-id="e5d23-235">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="e5d23-235">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="e5d23-236">isBundle</span><span class="sxs-lookup"><span data-stu-id="e5d23-236">isBundle</span></span>|<span data-ttu-id="e5d23-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5d23-237">Boolean</span></span>|<span data-ttu-id="e5d23-238">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="e5d23-238">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="e5d23-239">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e5d23-239">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e5d23-240">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e5d23-240">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="e5d23-241">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e5d23-241">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e5d23-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e5d23-242">identityVersion</span></span>|<span data-ttu-id="e5d23-243">String</span><span class="sxs-lookup"><span data-stu-id="e5d23-243">String</span></span>|<span data-ttu-id="e5d23-244">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e5d23-244">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e5d23-245">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5d23-245">Response</span></span>
<span data-ttu-id="e5d23-246">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e5d23-246">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5d23-247">Пример</span><span class="sxs-lookup"><span data-stu-id="e5d23-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5d23-248">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5d23-248">Request</span></span>
<span data-ttu-id="e5d23-249">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5d23-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="e5d23-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5d23-250">Response</span></span>
<span data-ttu-id="e5d23-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5d23-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



