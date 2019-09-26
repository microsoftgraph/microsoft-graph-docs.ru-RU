---
title: Создание officeSuiteApp
description: Создание нового объекта officeSuiteApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 28135804ab9f27f41b7f5f9fedd511574b402999
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37172354"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="b39f3-103">Создание officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="b39f3-103">Create officeSuiteApp</span></span>

> <span data-ttu-id="b39f3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b39f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b39f3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b39f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b39f3-106">Создание нового объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b39f3-106">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b39f3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b39f3-107">Prerequisites</span></span>
<span data-ttu-id="b39f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b39f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b39f3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b39f3-110">Permission type</span></span>|<span data-ttu-id="b39f3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b39f3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b39f3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b39f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b39f3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b39f3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b39f3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b39f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b39f3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b39f3-115">Not supported.</span></span>|
|<span data-ttu-id="b39f3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b39f3-116">Application</span></span>|<span data-ttu-id="b39f3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b39f3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b39f3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b39f3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b39f3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b39f3-119">Request headers</span></span>
|<span data-ttu-id="b39f3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b39f3-120">Header</span></span>|<span data-ttu-id="b39f3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b39f3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b39f3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b39f3-122">Authorization</span></span>|<span data-ttu-id="b39f3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b39f3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b39f3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b39f3-124">Accept</span></span>|<span data-ttu-id="b39f3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b39f3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b39f3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b39f3-126">Request body</span></span>
<span data-ttu-id="b39f3-127">В тексте запроса добавьте представление объекта officeSuiteApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b39f3-127">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="b39f3-128">В следующей таблице приведены свойства, необходимые при создании officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="b39f3-128">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="b39f3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b39f3-129">Property</span></span>|<span data-ttu-id="b39f3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b39f3-130">Type</span></span>|<span data-ttu-id="b39f3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b39f3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b39f3-132">id</span><span class="sxs-lookup"><span data-stu-id="b39f3-132">id</span></span>|<span data-ttu-id="b39f3-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b39f3-133">String</span></span>|<span data-ttu-id="b39f3-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b39f3-134">Key of the entity.</span></span> <span data-ttu-id="b39f3-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b39f3-136">displayName</span></span>|<span data-ttu-id="b39f3-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b39f3-137">String</span></span>|<span data-ttu-id="b39f3-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b39f3-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b39f3-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-140">description</span><span class="sxs-lookup"><span data-stu-id="b39f3-140">description</span></span>|<span data-ttu-id="b39f3-141">Строка</span><span class="sxs-lookup"><span data-stu-id="b39f3-141">String</span></span>|<span data-ttu-id="b39f3-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b39f3-142">The description of the app.</span></span> <span data-ttu-id="b39f3-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b39f3-144">publisher</span></span>|<span data-ttu-id="b39f3-145">String.</span><span class="sxs-lookup"><span data-stu-id="b39f3-145">String</span></span>|<span data-ttu-id="b39f3-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b39f3-146">The publisher of the app.</span></span> <span data-ttu-id="b39f3-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b39f3-148">largeIcon</span></span>|[<span data-ttu-id="b39f3-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b39f3-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b39f3-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b39f3-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b39f3-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b39f3-152">createdDateTime</span></span>|<span data-ttu-id="b39f3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b39f3-153">DateTimeOffset</span></span>|<span data-ttu-id="b39f3-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b39f3-154">The date and time the app was created.</span></span> <span data-ttu-id="b39f3-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b39f3-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b39f3-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b39f3-157">DateTimeOffset</span></span>|<span data-ttu-id="b39f3-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b39f3-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b39f3-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b39f3-160">isFeatured</span></span>|<span data-ttu-id="b39f3-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b39f3-161">Boolean</span></span>|<span data-ttu-id="b39f3-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b39f3-163">privacyInformationUrl</span></span>|<span data-ttu-id="b39f3-164">String.</span><span class="sxs-lookup"><span data-stu-id="b39f3-164">String</span></span>|<span data-ttu-id="b39f3-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b39f3-165">The privacy statement Url.</span></span> <span data-ttu-id="b39f3-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b39f3-167">informationUrl</span></span>|<span data-ttu-id="b39f3-168">String.</span><span class="sxs-lookup"><span data-stu-id="b39f3-168">String</span></span>|<span data-ttu-id="b39f3-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b39f3-169">The more information Url.</span></span> <span data-ttu-id="b39f3-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-171">owner</span><span class="sxs-lookup"><span data-stu-id="b39f3-171">owner</span></span>|<span data-ttu-id="b39f3-172">String</span><span class="sxs-lookup"><span data-stu-id="b39f3-172">String</span></span>|<span data-ttu-id="b39f3-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b39f3-173">The owner of the app.</span></span> <span data-ttu-id="b39f3-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-175">developer</span><span class="sxs-lookup"><span data-stu-id="b39f3-175">developer</span></span>|<span data-ttu-id="b39f3-176">String.</span><span class="sxs-lookup"><span data-stu-id="b39f3-176">String</span></span>|<span data-ttu-id="b39f3-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b39f3-177">The developer of the app.</span></span> <span data-ttu-id="b39f3-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-179">notes</span><span class="sxs-lookup"><span data-stu-id="b39f3-179">notes</span></span>|<span data-ttu-id="b39f3-180">String</span><span class="sxs-lookup"><span data-stu-id="b39f3-180">String</span></span>|<span data-ttu-id="b39f3-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="b39f3-181">Notes for the app.</span></span> <span data-ttu-id="b39f3-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b39f3-183">uploadState</span></span>|<span data-ttu-id="b39f3-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b39f3-184">Int32</span></span>|<span data-ttu-id="b39f3-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="b39f3-185">The upload state.</span></span> <span data-ttu-id="b39f3-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b39f3-187">publishingState</span></span>|[<span data-ttu-id="b39f3-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="b39f3-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b39f3-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="b39f3-189">The publishing state for the app.</span></span> <span data-ttu-id="b39f3-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b39f3-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b39f3-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="b39f3-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b39f3-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b39f3-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b39f3-193">isAssigned</span></span>|<span data-ttu-id="b39f3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b39f3-194">Boolean</span></span>|<span data-ttu-id="b39f3-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="b39f3-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b39f3-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b39f3-197">roleScopeTagIds</span></span>|<span data-ttu-id="b39f3-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b39f3-198">String collection</span></span>|<span data-ttu-id="b39f3-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b39f3-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b39f3-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="b39f3-201">dependentAppCount</span></span>|<span data-ttu-id="b39f3-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b39f3-202">Int32</span></span>|<span data-ttu-id="b39f3-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="b39f3-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b39f3-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b39f3-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b39f3-205">аутоакцептеула</span><span class="sxs-lookup"><span data-stu-id="b39f3-205">autoAcceptEula</span></span>|<span data-ttu-id="b39f3-206">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b39f3-206">Boolean</span></span>|<span data-ttu-id="b39f3-207">Значение, которое будет автоматически принимать условия лицензионного соглашения на устройстве ендусер.</span><span class="sxs-lookup"><span data-stu-id="b39f3-207">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="b39f3-208">productIds</span><span class="sxs-lookup"><span data-stu-id="b39f3-208">productIds</span></span>|<span data-ttu-id="b39f3-209">Коллекция [оффицепродуктид](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="b39f3-209">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="b39f3-210">Идентификаторы продуктов, представляющие SKU набора Office365.</span><span class="sxs-lookup"><span data-stu-id="b39f3-210">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="b39f3-211">Возможные значения: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="b39f3-211">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="b39f3-212">excludedApps</span><span class="sxs-lookup"><span data-stu-id="b39f3-212">excludedApps</span></span>|<span data-ttu-id="b39f3-213">[excludedApps](../resources/intune-apps-excludedapps.md);</span><span class="sxs-lookup"><span data-stu-id="b39f3-213">[excludedApps](../resources/intune-apps-excludedapps.md)</span></span>|<span data-ttu-id="b39f3-214">Свойство для представления приложений, исключаемых из выбранного идентификатора продукта Office365.</span><span class="sxs-lookup"><span data-stu-id="b39f3-214">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="b39f3-215">Свойства usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="b39f3-215">useSharedComputerActivation</span></span>|<span data-ttu-id="b39f3-216">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b39f3-216">Boolean</span></span>|<span data-ttu-id="b39f3-217">Свойство для представления того, используется ли активация на общем компьютере не для приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="b39f3-217">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="b39f3-218">updateChannel</span><span class="sxs-lookup"><span data-stu-id="b39f3-218">updateChannel</span></span>|[<span data-ttu-id="b39f3-219">оффицеупдатечаннел</span><span class="sxs-lookup"><span data-stu-id="b39f3-219">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="b39f3-220">Свойство для представления канала обновления Office365.</span><span class="sxs-lookup"><span data-stu-id="b39f3-220">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="b39f3-221">Возможные значения: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="b39f3-221">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="b39f3-222">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="b39f3-222">officePlatformArchitecture</span></span>|[<span data-ttu-id="b39f3-223">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b39f3-223">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b39f3-224">Свойство для представления версии набора приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="b39f3-224">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="b39f3-225">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="b39f3-225">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b39f3-226">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="b39f3-226">localesToInstall</span></span>|<span data-ttu-id="b39f3-227">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b39f3-227">String collection</span></span>|<span data-ttu-id="b39f3-228">Свойство для представления языковых стандартов, устанавливаемых при установке приложений из Office365.</span><span class="sxs-lookup"><span data-stu-id="b39f3-228">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="b39f3-229">В нем используется стандартная спецификация RFC 6033.</span><span class="sxs-lookup"><span data-stu-id="b39f3-229">It uses standard RFC 6033.</span></span> <span data-ttu-id="b39f3-230">Словомhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="b39f3-230">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="b39f3-231">инсталлпрогрессдисплайлевел</span><span class="sxs-lookup"><span data-stu-id="b39f3-231">installProgressDisplayLevel</span></span>|[<span data-ttu-id="b39f3-232">оффицесуитеинсталлпрогрессдисплайлевел</span><span class="sxs-lookup"><span data-stu-id="b39f3-232">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="b39f3-233">Для указания уровня отображения пользовательского интерфейса установки хода установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b39f3-233">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="b39f3-234">Возможные значения: `none`, `full`.</span><span class="sxs-lookup"><span data-stu-id="b39f3-234">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="b39f3-235">шаулдунинсталлолдерверсионсофоффице</span><span class="sxs-lookup"><span data-stu-id="b39f3-235">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="b39f3-236">Boolean.</span><span class="sxs-lookup"><span data-stu-id="b39f3-236">Boolean</span></span>|<span data-ttu-id="b39f3-237">Свойство, определяющее, следует ли удалить существующий MSI Office, если на устройстве развернут набор приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="b39f3-237">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="b39f3-238">Атрибута targetversion</span><span class="sxs-lookup"><span data-stu-id="b39f3-238">targetVersion</span></span>|<span data-ttu-id="b39f3-239">String.</span><span class="sxs-lookup"><span data-stu-id="b39f3-239">String</span></span>|<span data-ttu-id="b39f3-240">Свойство, представляющее определенную целевую версию для набора приложений Office365, который должен быть развернут на устройствах.</span><span class="sxs-lookup"><span data-stu-id="b39f3-240">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="b39f3-241">упдатеверсион</span><span class="sxs-lookup"><span data-stu-id="b39f3-241">updateVersion</span></span>|<span data-ttu-id="b39f3-242">String.</span><span class="sxs-lookup"><span data-stu-id="b39f3-242">String</span></span>|<span data-ttu-id="b39f3-243">Свойство для представления версии обновления, в которой определенная Целевая версия доступна для набора приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="b39f3-243">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="b39f3-244">оффицеконфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="b39f3-244">officeConfigurationXml</span></span>|<span data-ttu-id="b39f3-245">Binary</span><span class="sxs-lookup"><span data-stu-id="b39f3-245">Binary</span></span>|<span data-ttu-id="b39f3-246">Свойство, представляющее XML-файл конфигурации, который можно указать для приложений Office профессиональный плюс.</span><span class="sxs-lookup"><span data-stu-id="b39f3-246">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="b39f3-247">Имеет приоритет над всеми другими свойствами.</span><span class="sxs-lookup"><span data-stu-id="b39f3-247">Takes precedence over all other properties.</span></span> <span data-ttu-id="b39f3-248">Если этот параметр указан, для создания приложения будет использоваться XML-файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="b39f3-248">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="b39f3-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="b39f3-249">Response</span></span>
<span data-ttu-id="b39f3-250">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b39f3-250">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b39f3-251">Пример</span><span class="sxs-lookup"><span data-stu-id="b39f3-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="b39f3-252">Запрос</span><span class="sxs-lookup"><span data-stu-id="b39f3-252">Request</span></span>
<span data-ttu-id="b39f3-253">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b39f3-253">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1599

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="b39f3-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="b39f3-254">Response</span></span>
<span data-ttu-id="b39f3-p125">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b39f3-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1771

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```




