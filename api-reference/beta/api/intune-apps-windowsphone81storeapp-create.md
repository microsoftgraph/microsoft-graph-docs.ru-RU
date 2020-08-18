---
title: Создание windowsPhone81StoreApp
description: Создание нового объекта windowsPhone81StoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34bf8ee73a2be649e493bba6ddc5ede89b0004fe
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790051"
---
# <a name="create-windowsphone81storeapp"></a><span data-ttu-id="a9e93-103">Создание windowsPhone81StoreApp</span><span class="sxs-lookup"><span data-stu-id="a9e93-103">Create windowsPhone81StoreApp</span></span>

<span data-ttu-id="a9e93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9e93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9e93-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9e93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9e93-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9e93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9e93-107">Создание нового объекта [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a9e93-107">Create a new [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9e93-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a9e93-108">Prerequisites</span></span>
<span data-ttu-id="a9e93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9e93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9e93-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9e93-111">Permission type</span></span>|<span data-ttu-id="a9e93-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9e93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9e93-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9e93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9e93-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9e93-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a9e93-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9e93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9e93-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9e93-116">Not supported.</span></span>|
|<span data-ttu-id="a9e93-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a9e93-117">Application</span></span>|<span data-ttu-id="a9e93-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9e93-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9e93-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9e93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a9e93-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a9e93-120">Request headers</span></span>
|<span data-ttu-id="a9e93-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9e93-121">Header</span></span>|<span data-ttu-id="a9e93-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a9e93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9e93-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9e93-123">Authorization</span></span>|<span data-ttu-id="a9e93-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9e93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9e93-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9e93-125">Accept</span></span>|<span data-ttu-id="a9e93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9e93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9e93-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9e93-127">Request body</span></span>
<span data-ttu-id="a9e93-128">В тексте запроса добавьте представление объекта windowsPhone81StoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9e93-128">In the request body, supply a JSON representation for the windowsPhone81StoreApp object.</span></span>

<span data-ttu-id="a9e93-129">В следующей таблице приведены свойства, необходимые при создании windowsPhone81StoreApp.</span><span class="sxs-lookup"><span data-stu-id="a9e93-129">The following table shows the properties that are required when you create the windowsPhone81StoreApp.</span></span>

|<span data-ttu-id="a9e93-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9e93-130">Property</span></span>|<span data-ttu-id="a9e93-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a9e93-131">Type</span></span>|<span data-ttu-id="a9e93-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a9e93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9e93-133">id</span><span class="sxs-lookup"><span data-stu-id="a9e93-133">id</span></span>|<span data-ttu-id="a9e93-134">String</span><span class="sxs-lookup"><span data-stu-id="a9e93-134">String</span></span>|<span data-ttu-id="a9e93-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a9e93-135">Key of the entity.</span></span> <span data-ttu-id="a9e93-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a9e93-137">displayName</span></span>|<span data-ttu-id="a9e93-138">String</span><span class="sxs-lookup"><span data-stu-id="a9e93-138">String</span></span>|<span data-ttu-id="a9e93-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a9e93-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a9e93-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-141">description</span><span class="sxs-lookup"><span data-stu-id="a9e93-141">description</span></span>|<span data-ttu-id="a9e93-142">String</span><span class="sxs-lookup"><span data-stu-id="a9e93-142">String</span></span>|<span data-ttu-id="a9e93-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a9e93-143">The description of the app.</span></span> <span data-ttu-id="a9e93-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a9e93-145">publisher</span></span>|<span data-ttu-id="a9e93-146">String</span><span class="sxs-lookup"><span data-stu-id="a9e93-146">String</span></span>|<span data-ttu-id="a9e93-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a9e93-147">The publisher of the app.</span></span> <span data-ttu-id="a9e93-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a9e93-149">largeIcon</span></span>|[<span data-ttu-id="a9e93-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a9e93-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a9e93-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a9e93-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a9e93-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9e93-153">createdDateTime</span></span>|<span data-ttu-id="a9e93-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9e93-154">DateTimeOffset</span></span>|<span data-ttu-id="a9e93-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a9e93-155">The date and time the app was created.</span></span> <span data-ttu-id="a9e93-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9e93-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a9e93-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9e93-158">DateTimeOffset</span></span>|<span data-ttu-id="a9e93-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a9e93-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a9e93-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a9e93-161">isFeatured</span></span>|<span data-ttu-id="a9e93-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9e93-162">Boolean</span></span>|<span data-ttu-id="a9e93-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a9e93-164">privacyInformationUrl</span></span>|<span data-ttu-id="a9e93-165">String</span><span class="sxs-lookup"><span data-stu-id="a9e93-165">String</span></span>|<span data-ttu-id="a9e93-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a9e93-166">The privacy statement Url.</span></span> <span data-ttu-id="a9e93-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a9e93-168">informationUrl</span></span>|<span data-ttu-id="a9e93-169">String</span><span class="sxs-lookup"><span data-stu-id="a9e93-169">String</span></span>|<span data-ttu-id="a9e93-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a9e93-170">The more information Url.</span></span> <span data-ttu-id="a9e93-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-172">owner</span><span class="sxs-lookup"><span data-stu-id="a9e93-172">owner</span></span>|<span data-ttu-id="a9e93-173">String</span><span class="sxs-lookup"><span data-stu-id="a9e93-173">String</span></span>|<span data-ttu-id="a9e93-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a9e93-174">The owner of the app.</span></span> <span data-ttu-id="a9e93-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-176">developer</span><span class="sxs-lookup"><span data-stu-id="a9e93-176">developer</span></span>|<span data-ttu-id="a9e93-177">String</span><span class="sxs-lookup"><span data-stu-id="a9e93-177">String</span></span>|<span data-ttu-id="a9e93-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a9e93-178">The developer of the app.</span></span> <span data-ttu-id="a9e93-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-180">notes</span><span class="sxs-lookup"><span data-stu-id="a9e93-180">notes</span></span>|<span data-ttu-id="a9e93-181">String</span><span class="sxs-lookup"><span data-stu-id="a9e93-181">String</span></span>|<span data-ttu-id="a9e93-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="a9e93-182">Notes for the app.</span></span> <span data-ttu-id="a9e93-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a9e93-184">uploadState</span></span>|<span data-ttu-id="a9e93-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a9e93-185">Int32</span></span>|<span data-ttu-id="a9e93-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="a9e93-186">The upload state.</span></span> <span data-ttu-id="a9e93-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="a9e93-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="a9e93-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="a9e93-189">publishingState</span></span>|[<span data-ttu-id="a9e93-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="a9e93-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a9e93-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="a9e93-191">The publishing state for the app.</span></span> <span data-ttu-id="a9e93-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a9e93-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a9e93-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="a9e93-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a9e93-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a9e93-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a9e93-195">isAssigned</span></span>|<span data-ttu-id="a9e93-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9e93-196">Boolean</span></span>|<span data-ttu-id="a9e93-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="a9e93-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a9e93-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9e93-199">roleScopeTagIds</span></span>|<span data-ttu-id="a9e93-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a9e93-200">String collection</span></span>|<span data-ttu-id="a9e93-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="a9e93-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a9e93-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a9e93-203">dependentAppCount</span></span>|<span data-ttu-id="a9e93-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a9e93-204">Int32</span></span>|<span data-ttu-id="a9e93-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="a9e93-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a9e93-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9e93-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e93-207">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a9e93-207">appStoreUrl</span></span>|<span data-ttu-id="a9e93-208">String</span><span class="sxs-lookup"><span data-stu-id="a9e93-208">String</span></span>|<span data-ttu-id="a9e93-209">URL-адрес магазина приложений Windows Phone 8,1.</span><span class="sxs-lookup"><span data-stu-id="a9e93-209">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="a9e93-210">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9e93-210">Response</span></span>
<span data-ttu-id="a9e93-211">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9e93-211">If successful, this method returns a `201 Created` response code and a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9e93-212">Пример</span><span class="sxs-lookup"><span data-stu-id="a9e93-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9e93-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9e93-213">Request</span></span>
<span data-ttu-id="a9e93-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9e93-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 775

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="a9e93-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9e93-215">Response</span></span>
<span data-ttu-id="a9e93-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9e93-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 947

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
  "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```



