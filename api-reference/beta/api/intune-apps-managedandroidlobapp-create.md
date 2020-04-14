---
title: Create managedAndroidLobApp
description: Создание объекта managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f9787b88055896b41c0816ba58d49798a6aa2ea3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406409"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="de788-103">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="de788-103">Create managedAndroidLobApp</span></span>

<span data-ttu-id="de788-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de788-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de788-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de788-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de788-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de788-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de788-107">Создание объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de788-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="de788-108">Prerequisites</span></span>
<span data-ttu-id="de788-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de788-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de788-111">Permission type</span></span>|<span data-ttu-id="de788-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de788-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de788-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de788-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de788-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de788-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="de788-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de788-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de788-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de788-116">Not supported.</span></span>|
|<span data-ttu-id="de788-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="de788-117">Application</span></span>|<span data-ttu-id="de788-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de788-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de788-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de788-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="de788-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="de788-120">Request headers</span></span>
|<span data-ttu-id="de788-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de788-121">Header</span></span>|<span data-ttu-id="de788-122">Значение</span><span class="sxs-lookup"><span data-stu-id="de788-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de788-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de788-123">Authorization</span></span>|<span data-ttu-id="de788-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de788-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de788-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de788-125">Accept</span></span>|<span data-ttu-id="de788-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de788-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de788-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de788-127">Request body</span></span>
<span data-ttu-id="de788-128">В тексте запроса добавьте представление объекта managedAndroidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de788-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="de788-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="de788-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="de788-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="de788-130">Property</span></span>|<span data-ttu-id="de788-131">Тип</span><span class="sxs-lookup"><span data-stu-id="de788-131">Type</span></span>|<span data-ttu-id="de788-132">Описание</span><span class="sxs-lookup"><span data-stu-id="de788-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de788-133">id</span><span class="sxs-lookup"><span data-stu-id="de788-133">id</span></span>|<span data-ttu-id="de788-134">Строка</span><span class="sxs-lookup"><span data-stu-id="de788-134">String</span></span>|<span data-ttu-id="de788-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="de788-135">Key of the entity.</span></span> <span data-ttu-id="de788-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-137">displayName</span><span class="sxs-lookup"><span data-stu-id="de788-137">displayName</span></span>|<span data-ttu-id="de788-138">Строка</span><span class="sxs-lookup"><span data-stu-id="de788-138">String</span></span>|<span data-ttu-id="de788-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="de788-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="de788-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-141">description</span><span class="sxs-lookup"><span data-stu-id="de788-141">description</span></span>|<span data-ttu-id="de788-142">String</span><span class="sxs-lookup"><span data-stu-id="de788-142">String</span></span>|<span data-ttu-id="de788-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-143">The description of the app.</span></span> <span data-ttu-id="de788-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-145">publisher</span><span class="sxs-lookup"><span data-stu-id="de788-145">publisher</span></span>|<span data-ttu-id="de788-146">String</span><span class="sxs-lookup"><span data-stu-id="de788-146">String</span></span>|<span data-ttu-id="de788-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-147">The publisher of the app.</span></span> <span data-ttu-id="de788-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="de788-149">largeIcon</span></span>|[<span data-ttu-id="de788-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="de788-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="de788-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="de788-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="de788-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de788-153">createdDateTime</span></span>|<span data-ttu-id="de788-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de788-154">DateTimeOffset</span></span>|<span data-ttu-id="de788-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-155">The date and time the app was created.</span></span> <span data-ttu-id="de788-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de788-157">lastModifiedDateTime</span></span>|<span data-ttu-id="de788-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de788-158">DateTimeOffset</span></span>|<span data-ttu-id="de788-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-159">The date and time the app was last modified.</span></span> <span data-ttu-id="de788-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="de788-161">isFeatured</span></span>|<span data-ttu-id="de788-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="de788-162">Boolean</span></span>|<span data-ttu-id="de788-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="de788-164">privacyInformationUrl</span></span>|<span data-ttu-id="de788-165">String</span><span class="sxs-lookup"><span data-stu-id="de788-165">String</span></span>|<span data-ttu-id="de788-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="de788-166">The privacy statement Url.</span></span> <span data-ttu-id="de788-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="de788-168">informationUrl</span></span>|<span data-ttu-id="de788-169">String</span><span class="sxs-lookup"><span data-stu-id="de788-169">String</span></span>|<span data-ttu-id="de788-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="de788-170">The more information Url.</span></span> <span data-ttu-id="de788-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-172">owner</span><span class="sxs-lookup"><span data-stu-id="de788-172">owner</span></span>|<span data-ttu-id="de788-173">String</span><span class="sxs-lookup"><span data-stu-id="de788-173">String</span></span>|<span data-ttu-id="de788-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-174">The owner of the app.</span></span> <span data-ttu-id="de788-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-176">developer</span><span class="sxs-lookup"><span data-stu-id="de788-176">developer</span></span>|<span data-ttu-id="de788-177">String</span><span class="sxs-lookup"><span data-stu-id="de788-177">String</span></span>|<span data-ttu-id="de788-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-178">The developer of the app.</span></span> <span data-ttu-id="de788-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-180">notes</span><span class="sxs-lookup"><span data-stu-id="de788-180">notes</span></span>|<span data-ttu-id="de788-181">String</span><span class="sxs-lookup"><span data-stu-id="de788-181">String</span></span>|<span data-ttu-id="de788-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-182">Notes for the app.</span></span> <span data-ttu-id="de788-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="de788-184">uploadState</span></span>|<span data-ttu-id="de788-185">Int32</span><span class="sxs-lookup"><span data-stu-id="de788-185">Int32</span></span>|<span data-ttu-id="de788-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="de788-186">The upload state.</span></span> <span data-ttu-id="de788-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="de788-188">publishingState</span></span>|[<span data-ttu-id="de788-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="de788-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="de788-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-190">The publishing state for the app.</span></span> <span data-ttu-id="de788-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="de788-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="de788-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="de788-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="de788-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="de788-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="de788-194">isAssigned</span></span>|<span data-ttu-id="de788-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="de788-195">Boolean</span></span>|<span data-ttu-id="de788-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="de788-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="de788-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="de788-198">roleScopeTagIds</span></span>|<span data-ttu-id="de788-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="de788-199">String collection</span></span>|<span data-ttu-id="de788-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="de788-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="de788-202">dependentAppCount</span></span>|<span data-ttu-id="de788-203">Int32</span><span class="sxs-lookup"><span data-stu-id="de788-203">Int32</span></span>|<span data-ttu-id="de788-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="de788-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="de788-206">appAvailability</span><span class="sxs-lookup"><span data-stu-id="de788-206">appAvailability</span></span>|[<span data-ttu-id="de788-207">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="de788-207">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="de788-208">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-208">The Application's availability.</span></span> <span data-ttu-id="de788-209">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="de788-210">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="de788-210">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="de788-211">version</span><span class="sxs-lookup"><span data-stu-id="de788-211">version</span></span>|<span data-ttu-id="de788-212">String</span><span class="sxs-lookup"><span data-stu-id="de788-212">String</span></span>|<span data-ttu-id="de788-213">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-213">The Application's version.</span></span> <span data-ttu-id="de788-214">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-214">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="de788-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="de788-215">committedContentVersion</span></span>|<span data-ttu-id="de788-216">String</span><span class="sxs-lookup"><span data-stu-id="de788-216">String</span></span>|<span data-ttu-id="de788-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="de788-217">The internal committed content version.</span></span> <span data-ttu-id="de788-218">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="de788-219">fileName</span><span class="sxs-lookup"><span data-stu-id="de788-219">fileName</span></span>|<span data-ttu-id="de788-220">String</span><span class="sxs-lookup"><span data-stu-id="de788-220">String</span></span>|<span data-ttu-id="de788-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="de788-221">The name of the main Lob application file.</span></span> <span data-ttu-id="de788-222">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="de788-223">size</span><span class="sxs-lookup"><span data-stu-id="de788-223">size</span></span>|<span data-ttu-id="de788-224">Int64</span><span class="sxs-lookup"><span data-stu-id="de788-224">Int64</span></span>|<span data-ttu-id="de788-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="de788-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="de788-226">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="de788-226">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="de788-227">packageId</span><span class="sxs-lookup"><span data-stu-id="de788-227">packageId</span></span>|<span data-ttu-id="de788-228">String</span><span class="sxs-lookup"><span data-stu-id="de788-228">String</span></span>|<span data-ttu-id="de788-229">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="de788-229">The package identifier.</span></span>|
|<span data-ttu-id="de788-230">identityName</span><span class="sxs-lookup"><span data-stu-id="de788-230">identityName</span></span>|<span data-ttu-id="de788-231">String</span><span class="sxs-lookup"><span data-stu-id="de788-231">String</span></span>|<span data-ttu-id="de788-232">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="de788-232">The Identity Name.</span></span>|
|<span data-ttu-id="de788-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="de788-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="de788-234">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="de788-234">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="de788-235">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="de788-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="de788-236">versionName</span><span class="sxs-lookup"><span data-stu-id="de788-236">versionName</span></span>|<span data-ttu-id="de788-237">String</span><span class="sxs-lookup"><span data-stu-id="de788-237">String</span></span>|<span data-ttu-id="de788-238">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="de788-238">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="de788-239">versionCode</span><span class="sxs-lookup"><span data-stu-id="de788-239">versionCode</span></span>|<span data-ttu-id="de788-240">String</span><span class="sxs-lookup"><span data-stu-id="de788-240">String</span></span>|<span data-ttu-id="de788-241">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="de788-241">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="de788-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="de788-242">identityVersion</span></span>|<span data-ttu-id="de788-243">String</span><span class="sxs-lookup"><span data-stu-id="de788-243">String</span></span>|<span data-ttu-id="de788-244">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="de788-244">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="de788-245">Ответ</span><span class="sxs-lookup"><span data-stu-id="de788-245">Response</span></span>
<span data-ttu-id="de788-246">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="de788-246">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de788-247">Пример</span><span class="sxs-lookup"><span data-stu-id="de788-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="de788-248">Запрос</span><span class="sxs-lookup"><span data-stu-id="de788-248">Request</span></span>
<span data-ttu-id="de788-249">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de788-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1491

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="de788-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="de788-250">Response</span></span>
<span data-ttu-id="de788-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de788-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1663

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```



