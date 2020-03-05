---
title: Создание объекта androidStoreApp
description: Создание объекта androidStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 30c4f26f640cce9ab51fcc84061a20e070195c50
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445829"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="50518-103">Создание объекта androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="50518-103">Create androidStoreApp</span></span>

<span data-ttu-id="50518-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="50518-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50518-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50518-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50518-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50518-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50518-107">Создание объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-107">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50518-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="50518-108">Prerequisites</span></span>
<span data-ttu-id="50518-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50518-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50518-111">Permission type</span></span>|<span data-ttu-id="50518-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="50518-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50518-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50518-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50518-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50518-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50518-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50518-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50518-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50518-116">Not supported.</span></span>|
|<span data-ttu-id="50518-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50518-117">Application</span></span>|<span data-ttu-id="50518-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50518-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50518-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50518-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="50518-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="50518-120">Request headers</span></span>
|<span data-ttu-id="50518-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="50518-121">Header</span></span>|<span data-ttu-id="50518-122">Значение</span><span class="sxs-lookup"><span data-stu-id="50518-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50518-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50518-123">Authorization</span></span>|<span data-ttu-id="50518-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50518-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50518-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50518-125">Accept</span></span>|<span data-ttu-id="50518-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50518-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50518-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50518-127">Request body</span></span>
<span data-ttu-id="50518-128">В тексте запроса добавьте представление объекта androidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50518-128">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="50518-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="50518-129">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="50518-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="50518-130">Property</span></span>|<span data-ttu-id="50518-131">Тип</span><span class="sxs-lookup"><span data-stu-id="50518-131">Type</span></span>|<span data-ttu-id="50518-132">Описание</span><span class="sxs-lookup"><span data-stu-id="50518-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50518-133">id</span><span class="sxs-lookup"><span data-stu-id="50518-133">id</span></span>|<span data-ttu-id="50518-134">Строка</span><span class="sxs-lookup"><span data-stu-id="50518-134">String</span></span>|<span data-ttu-id="50518-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="50518-135">Key of the entity.</span></span> <span data-ttu-id="50518-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-137">displayName</span><span class="sxs-lookup"><span data-stu-id="50518-137">displayName</span></span>|<span data-ttu-id="50518-138">Строка</span><span class="sxs-lookup"><span data-stu-id="50518-138">String</span></span>|<span data-ttu-id="50518-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="50518-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="50518-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-141">description</span><span class="sxs-lookup"><span data-stu-id="50518-141">description</span></span>|<span data-ttu-id="50518-142">Строка</span><span class="sxs-lookup"><span data-stu-id="50518-142">String</span></span>|<span data-ttu-id="50518-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="50518-143">The description of the app.</span></span> <span data-ttu-id="50518-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-145">publisher</span><span class="sxs-lookup"><span data-stu-id="50518-145">publisher</span></span>|<span data-ttu-id="50518-146">String</span><span class="sxs-lookup"><span data-stu-id="50518-146">String</span></span>|<span data-ttu-id="50518-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="50518-147">The publisher of the app.</span></span> <span data-ttu-id="50518-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="50518-149">largeIcon</span></span>|[<span data-ttu-id="50518-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="50518-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="50518-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="50518-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="50518-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50518-153">createdDateTime</span></span>|<span data-ttu-id="50518-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50518-154">DateTimeOffset</span></span>|<span data-ttu-id="50518-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="50518-155">The date and time the app was created.</span></span> <span data-ttu-id="50518-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50518-157">lastModifiedDateTime</span></span>|<span data-ttu-id="50518-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50518-158">DateTimeOffset</span></span>|<span data-ttu-id="50518-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="50518-159">The date and time the app was last modified.</span></span> <span data-ttu-id="50518-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="50518-161">isFeatured</span></span>|<span data-ttu-id="50518-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="50518-162">Boolean</span></span>|<span data-ttu-id="50518-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="50518-164">privacyInformationUrl</span></span>|<span data-ttu-id="50518-165">String</span><span class="sxs-lookup"><span data-stu-id="50518-165">String</span></span>|<span data-ttu-id="50518-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="50518-166">The privacy statement Url.</span></span> <span data-ttu-id="50518-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="50518-168">informationUrl</span></span>|<span data-ttu-id="50518-169">String</span><span class="sxs-lookup"><span data-stu-id="50518-169">String</span></span>|<span data-ttu-id="50518-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="50518-170">The more information Url.</span></span> <span data-ttu-id="50518-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-172">owner</span><span class="sxs-lookup"><span data-stu-id="50518-172">owner</span></span>|<span data-ttu-id="50518-173">String</span><span class="sxs-lookup"><span data-stu-id="50518-173">String</span></span>|<span data-ttu-id="50518-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="50518-174">The owner of the app.</span></span> <span data-ttu-id="50518-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-176">developer</span><span class="sxs-lookup"><span data-stu-id="50518-176">developer</span></span>|<span data-ttu-id="50518-177">String</span><span class="sxs-lookup"><span data-stu-id="50518-177">String</span></span>|<span data-ttu-id="50518-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="50518-178">The developer of the app.</span></span> <span data-ttu-id="50518-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-180">notes</span><span class="sxs-lookup"><span data-stu-id="50518-180">notes</span></span>|<span data-ttu-id="50518-181">String</span><span class="sxs-lookup"><span data-stu-id="50518-181">String</span></span>|<span data-ttu-id="50518-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="50518-182">Notes for the app.</span></span> <span data-ttu-id="50518-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="50518-184">uploadState</span></span>|<span data-ttu-id="50518-185">Int32</span><span class="sxs-lookup"><span data-stu-id="50518-185">Int32</span></span>|<span data-ttu-id="50518-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="50518-186">The upload state.</span></span> <span data-ttu-id="50518-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="50518-188">publishingState</span></span>|[<span data-ttu-id="50518-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="50518-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="50518-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="50518-190">The publishing state for the app.</span></span> <span data-ttu-id="50518-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="50518-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="50518-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="50518-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="50518-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="50518-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="50518-194">isAssigned</span></span>|<span data-ttu-id="50518-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="50518-195">Boolean</span></span>|<span data-ttu-id="50518-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="50518-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="50518-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50518-198">roleScopeTagIds</span></span>|<span data-ttu-id="50518-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="50518-199">String collection</span></span>|<span data-ttu-id="50518-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="50518-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="50518-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="50518-202">dependentAppCount</span></span>|<span data-ttu-id="50518-203">Int32</span><span class="sxs-lookup"><span data-stu-id="50518-203">Int32</span></span>|<span data-ttu-id="50518-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="50518-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="50518-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50518-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50518-206">packageId</span><span class="sxs-lookup"><span data-stu-id="50518-206">packageId</span></span>|<span data-ttu-id="50518-207">String</span><span class="sxs-lookup"><span data-stu-id="50518-207">String</span></span>|<span data-ttu-id="50518-208">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="50518-208">The package identifier.</span></span>|
|<span data-ttu-id="50518-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="50518-209">appIdentifier</span></span>|<span data-ttu-id="50518-210">String</span><span class="sxs-lookup"><span data-stu-id="50518-210">String</span></span>|<span data-ttu-id="50518-211">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="50518-211">The Identity Name.</span></span>|
|<span data-ttu-id="50518-212">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="50518-212">appStoreUrl</span></span>|<span data-ttu-id="50518-213">String</span><span class="sxs-lookup"><span data-stu-id="50518-213">String</span></span>|<span data-ttu-id="50518-214">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="50518-214">The Android app store URL.</span></span>|
|<span data-ttu-id="50518-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="50518-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="50518-216">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="50518-216">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="50518-217">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="50518-217">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="50518-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="50518-218">Response</span></span>
<span data-ttu-id="50518-219">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50518-219">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50518-220">Пример</span><span class="sxs-lookup"><span data-stu-id="50518-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="50518-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="50518-221">Request</span></span>
<span data-ttu-id="50518-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50518-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1230

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="50518-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="50518-223">Response</span></span>
<span data-ttu-id="50518-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50518-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1402

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```





