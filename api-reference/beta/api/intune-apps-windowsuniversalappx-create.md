---
title: Create windowsUniversalAppX
description: Создание объекта windowsUniversalAppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5824afcdbdc573fdd5ced2e1a027da817ddfa393
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37171696"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="a1dfc-103">Create windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="a1dfc-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="a1dfc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1dfc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1dfc-106">Создание объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-106">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1dfc-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a1dfc-107">Prerequisites</span></span>
<span data-ttu-id="a1dfc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1dfc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1dfc-110">Permission type</span></span>|<span data-ttu-id="a1dfc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1dfc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1dfc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1dfc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1dfc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1dfc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a1dfc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1dfc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1dfc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-115">Not supported.</span></span>|
|<span data-ttu-id="a1dfc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1dfc-116">Application</span></span>|<span data-ttu-id="a1dfc-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1dfc-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1dfc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1dfc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a1dfc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1dfc-119">Request headers</span></span>
|<span data-ttu-id="a1dfc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1dfc-120">Header</span></span>|<span data-ttu-id="a1dfc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a1dfc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1dfc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1dfc-122">Authorization</span></span>|<span data-ttu-id="a1dfc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1dfc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a1dfc-124">Accept</span></span>|<span data-ttu-id="a1dfc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1dfc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1dfc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1dfc-126">Request body</span></span>
<span data-ttu-id="a1dfc-127">В тексте запроса добавьте представление объекта windowsUniversalAppX в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-127">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="a1dfc-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-128">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="a1dfc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1dfc-129">Property</span></span>|<span data-ttu-id="a1dfc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a1dfc-130">Type</span></span>|<span data-ttu-id="a1dfc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a1dfc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1dfc-132">id</span><span class="sxs-lookup"><span data-stu-id="a1dfc-132">id</span></span>|<span data-ttu-id="a1dfc-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a1dfc-133">String</span></span>|<span data-ttu-id="a1dfc-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-134">Key of the entity.</span></span> <span data-ttu-id="a1dfc-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a1dfc-136">displayName</span></span>|<span data-ttu-id="a1dfc-137">Строка</span><span class="sxs-lookup"><span data-stu-id="a1dfc-137">String</span></span>|<span data-ttu-id="a1dfc-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a1dfc-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-140">description</span><span class="sxs-lookup"><span data-stu-id="a1dfc-140">description</span></span>|<span data-ttu-id="a1dfc-141">Строка</span><span class="sxs-lookup"><span data-stu-id="a1dfc-141">String</span></span>|<span data-ttu-id="a1dfc-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-142">The description of the app.</span></span> <span data-ttu-id="a1dfc-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-144">publisher</span><span class="sxs-lookup"><span data-stu-id="a1dfc-144">publisher</span></span>|<span data-ttu-id="a1dfc-145">String.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-145">String</span></span>|<span data-ttu-id="a1dfc-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-146">The publisher of the app.</span></span> <span data-ttu-id="a1dfc-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a1dfc-148">largeIcon</span></span>|[<span data-ttu-id="a1dfc-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a1dfc-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a1dfc-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a1dfc-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1dfc-152">createdDateTime</span></span>|<span data-ttu-id="a1dfc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1dfc-153">DateTimeOffset</span></span>|<span data-ttu-id="a1dfc-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-154">The date and time the app was created.</span></span> <span data-ttu-id="a1dfc-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1dfc-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a1dfc-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1dfc-157">DateTimeOffset</span></span>|<span data-ttu-id="a1dfc-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a1dfc-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a1dfc-160">isFeatured</span></span>|<span data-ttu-id="a1dfc-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1dfc-161">Boolean</span></span>|<span data-ttu-id="a1dfc-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a1dfc-163">privacyInformationUrl</span></span>|<span data-ttu-id="a1dfc-164">String.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-164">String</span></span>|<span data-ttu-id="a1dfc-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-165">The privacy statement Url.</span></span> <span data-ttu-id="a1dfc-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a1dfc-167">informationUrl</span></span>|<span data-ttu-id="a1dfc-168">String.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-168">String</span></span>|<span data-ttu-id="a1dfc-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-169">The more information Url.</span></span> <span data-ttu-id="a1dfc-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-171">owner</span><span class="sxs-lookup"><span data-stu-id="a1dfc-171">owner</span></span>|<span data-ttu-id="a1dfc-172">String</span><span class="sxs-lookup"><span data-stu-id="a1dfc-172">String</span></span>|<span data-ttu-id="a1dfc-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-173">The owner of the app.</span></span> <span data-ttu-id="a1dfc-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-175">developer</span><span class="sxs-lookup"><span data-stu-id="a1dfc-175">developer</span></span>|<span data-ttu-id="a1dfc-176">String.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-176">String</span></span>|<span data-ttu-id="a1dfc-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-177">The developer of the app.</span></span> <span data-ttu-id="a1dfc-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-179">notes</span><span class="sxs-lookup"><span data-stu-id="a1dfc-179">notes</span></span>|<span data-ttu-id="a1dfc-180">String.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-180">String</span></span>|<span data-ttu-id="a1dfc-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-181">Notes for the app.</span></span> <span data-ttu-id="a1dfc-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="a1dfc-183">uploadState</span></span>|<span data-ttu-id="a1dfc-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a1dfc-184">Int32</span></span>|<span data-ttu-id="a1dfc-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-185">The upload state.</span></span> <span data-ttu-id="a1dfc-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="a1dfc-187">publishingState</span></span>|[<span data-ttu-id="a1dfc-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="a1dfc-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a1dfc-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-189">The publishing state for the app.</span></span> <span data-ttu-id="a1dfc-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a1dfc-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="a1dfc-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a1dfc-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a1dfc-193">isAssigned</span></span>|<span data-ttu-id="a1dfc-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1dfc-194">Boolean</span></span>|<span data-ttu-id="a1dfc-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a1dfc-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a1dfc-197">roleScopeTagIds</span></span>|<span data-ttu-id="a1dfc-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a1dfc-198">String collection</span></span>|<span data-ttu-id="a1dfc-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a1dfc-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a1dfc-201">dependentAppCount</span></span>|<span data-ttu-id="a1dfc-202">Int32</span><span class="sxs-lookup"><span data-stu-id="a1dfc-202">Int32</span></span>|<span data-ttu-id="a1dfc-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a1dfc-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a1dfc-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a1dfc-205">committedContentVersion</span></span>|<span data-ttu-id="a1dfc-206">String.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-206">String</span></span>|<span data-ttu-id="a1dfc-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-207">The internal committed content version.</span></span> <span data-ttu-id="a1dfc-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a1dfc-209">fileName</span><span class="sxs-lookup"><span data-stu-id="a1dfc-209">fileName</span></span>|<span data-ttu-id="a1dfc-210">String.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-210">String</span></span>|<span data-ttu-id="a1dfc-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-211">The name of the main Lob application file.</span></span> <span data-ttu-id="a1dfc-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a1dfc-213">size</span><span class="sxs-lookup"><span data-stu-id="a1dfc-213">size</span></span>|<span data-ttu-id="a1dfc-214">Int64</span><span class="sxs-lookup"><span data-stu-id="a1dfc-214">Int64</span></span>|<span data-ttu-id="a1dfc-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="a1dfc-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a1dfc-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a1dfc-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="a1dfc-217">applicableArchitectures</span></span>|[<span data-ttu-id="a1dfc-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a1dfc-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a1dfc-219">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="a1dfc-220">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="a1dfc-221">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="a1dfc-221">applicableDeviceTypes</span></span>|[<span data-ttu-id="a1dfc-222">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="a1dfc-222">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="a1dfc-223">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-223">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="a1dfc-224">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-224">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="a1dfc-225">identityName</span><span class="sxs-lookup"><span data-stu-id="a1dfc-225">identityName</span></span>|<span data-ttu-id="a1dfc-226">String</span><span class="sxs-lookup"><span data-stu-id="a1dfc-226">String</span></span>|<span data-ttu-id="a1dfc-227">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-227">The Identity Name.</span></span>|
|<span data-ttu-id="a1dfc-228">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="a1dfc-228">identityPublisherHash</span></span>|<span data-ttu-id="a1dfc-229">String.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-229">String</span></span>|<span data-ttu-id="a1dfc-230">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-230">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="a1dfc-231">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a1dfc-231">identityResourceIdentifier</span></span>|<span data-ttu-id="a1dfc-232">String.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-232">String</span></span>|<span data-ttu-id="a1dfc-233">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-233">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="a1dfc-234">isBundle</span><span class="sxs-lookup"><span data-stu-id="a1dfc-234">isBundle</span></span>|<span data-ttu-id="a1dfc-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1dfc-235">Boolean</span></span>|<span data-ttu-id="a1dfc-236">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-236">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="a1dfc-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a1dfc-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a1dfc-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a1dfc-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="a1dfc-239">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a1dfc-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="a1dfc-240">identityVersion</span></span>|<span data-ttu-id="a1dfc-241">String</span><span class="sxs-lookup"><span data-stu-id="a1dfc-241">String</span></span>|<span data-ttu-id="a1dfc-242">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="a1dfc-243">Ответ</span><span class="sxs-lookup"><span data-stu-id="a1dfc-243">Response</span></span>
<span data-ttu-id="a1dfc-244">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-244">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1dfc-245">Пример</span><span class="sxs-lookup"><span data-stu-id="a1dfc-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1dfc-246">Запрос</span><span class="sxs-lookup"><span data-stu-id="a1dfc-246">Request</span></span>
<span data-ttu-id="a1dfc-247">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-247">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1dfc-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1dfc-248">Response</span></span>
<span data-ttu-id="a1dfc-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1dfc-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




