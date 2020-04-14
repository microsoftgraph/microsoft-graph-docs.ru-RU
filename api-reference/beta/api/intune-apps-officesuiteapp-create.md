---
title: Создание officeSuiteApp
description: Создание нового объекта officeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 28e0301fed4e7dc9f12939d6e18ae938e573ce8c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43414355"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="5182e-103">Создание officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="5182e-103">Create officeSuiteApp</span></span>

<span data-ttu-id="5182e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5182e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5182e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5182e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5182e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5182e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5182e-107">Создание нового объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="5182e-107">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5182e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5182e-108">Prerequisites</span></span>
<span data-ttu-id="5182e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5182e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5182e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5182e-111">Permission type</span></span>|<span data-ttu-id="5182e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5182e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5182e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5182e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5182e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5182e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5182e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5182e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5182e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5182e-116">Not supported.</span></span>|
|<span data-ttu-id="5182e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5182e-117">Application</span></span>|<span data-ttu-id="5182e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5182e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5182e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5182e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="5182e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5182e-120">Request headers</span></span>
|<span data-ttu-id="5182e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5182e-121">Header</span></span>|<span data-ttu-id="5182e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5182e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5182e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5182e-123">Authorization</span></span>|<span data-ttu-id="5182e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5182e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5182e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5182e-125">Accept</span></span>|<span data-ttu-id="5182e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5182e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5182e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5182e-127">Request body</span></span>
<span data-ttu-id="5182e-128">В тексте запроса добавьте представление объекта officeSuiteApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5182e-128">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="5182e-129">В следующей таблице приведены свойства, необходимые при создании officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="5182e-129">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="5182e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5182e-130">Property</span></span>|<span data-ttu-id="5182e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5182e-131">Type</span></span>|<span data-ttu-id="5182e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5182e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5182e-133">id</span><span class="sxs-lookup"><span data-stu-id="5182e-133">id</span></span>|<span data-ttu-id="5182e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5182e-134">String</span></span>|<span data-ttu-id="5182e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5182e-135">Key of the entity.</span></span> <span data-ttu-id="5182e-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5182e-137">displayName</span></span>|<span data-ttu-id="5182e-138">Строка</span><span class="sxs-lookup"><span data-stu-id="5182e-138">String</span></span>|<span data-ttu-id="5182e-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="5182e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5182e-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-141">description</span><span class="sxs-lookup"><span data-stu-id="5182e-141">description</span></span>|<span data-ttu-id="5182e-142">Строка</span><span class="sxs-lookup"><span data-stu-id="5182e-142">String</span></span>|<span data-ttu-id="5182e-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="5182e-143">The description of the app.</span></span> <span data-ttu-id="5182e-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="5182e-145">publisher</span></span>|<span data-ttu-id="5182e-146">String</span><span class="sxs-lookup"><span data-stu-id="5182e-146">String</span></span>|<span data-ttu-id="5182e-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="5182e-147">The publisher of the app.</span></span> <span data-ttu-id="5182e-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5182e-149">largeIcon</span></span>|[<span data-ttu-id="5182e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5182e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5182e-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="5182e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5182e-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5182e-153">createdDateTime</span></span>|<span data-ttu-id="5182e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5182e-154">DateTimeOffset</span></span>|<span data-ttu-id="5182e-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="5182e-155">The date and time the app was created.</span></span> <span data-ttu-id="5182e-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5182e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="5182e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5182e-158">DateTimeOffset</span></span>|<span data-ttu-id="5182e-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="5182e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="5182e-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5182e-161">isFeatured</span></span>|<span data-ttu-id="5182e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5182e-162">Boolean</span></span>|<span data-ttu-id="5182e-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5182e-164">privacyInformationUrl</span></span>|<span data-ttu-id="5182e-165">String</span><span class="sxs-lookup"><span data-stu-id="5182e-165">String</span></span>|<span data-ttu-id="5182e-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5182e-166">The privacy statement Url.</span></span> <span data-ttu-id="5182e-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5182e-168">informationUrl</span></span>|<span data-ttu-id="5182e-169">String</span><span class="sxs-lookup"><span data-stu-id="5182e-169">String</span></span>|<span data-ttu-id="5182e-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5182e-170">The more information Url.</span></span> <span data-ttu-id="5182e-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-172">owner</span><span class="sxs-lookup"><span data-stu-id="5182e-172">owner</span></span>|<span data-ttu-id="5182e-173">String</span><span class="sxs-lookup"><span data-stu-id="5182e-173">String</span></span>|<span data-ttu-id="5182e-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="5182e-174">The owner of the app.</span></span> <span data-ttu-id="5182e-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-176">developer</span><span class="sxs-lookup"><span data-stu-id="5182e-176">developer</span></span>|<span data-ttu-id="5182e-177">String</span><span class="sxs-lookup"><span data-stu-id="5182e-177">String</span></span>|<span data-ttu-id="5182e-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="5182e-178">The developer of the app.</span></span> <span data-ttu-id="5182e-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-180">notes</span><span class="sxs-lookup"><span data-stu-id="5182e-180">notes</span></span>|<span data-ttu-id="5182e-181">String</span><span class="sxs-lookup"><span data-stu-id="5182e-181">String</span></span>|<span data-ttu-id="5182e-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="5182e-182">Notes for the app.</span></span> <span data-ttu-id="5182e-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="5182e-184">uploadState</span></span>|<span data-ttu-id="5182e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="5182e-185">Int32</span></span>|<span data-ttu-id="5182e-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="5182e-186">The upload state.</span></span> <span data-ttu-id="5182e-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="5182e-188">publishingState</span></span>|[<span data-ttu-id="5182e-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="5182e-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5182e-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="5182e-190">The publishing state for the app.</span></span> <span data-ttu-id="5182e-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="5182e-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5182e-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="5182e-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5182e-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5182e-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5182e-194">isAssigned</span></span>|<span data-ttu-id="5182e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="5182e-195">Boolean</span></span>|<span data-ttu-id="5182e-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="5182e-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5182e-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5182e-198">roleScopeTagIds</span></span>|<span data-ttu-id="5182e-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5182e-199">String collection</span></span>|<span data-ttu-id="5182e-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="5182e-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5182e-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="5182e-202">dependentAppCount</span></span>|<span data-ttu-id="5182e-203">Int32</span><span class="sxs-lookup"><span data-stu-id="5182e-203">Int32</span></span>|<span data-ttu-id="5182e-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="5182e-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="5182e-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5182e-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5182e-206">аутоакцептеула</span><span class="sxs-lookup"><span data-stu-id="5182e-206">autoAcceptEula</span></span>|<span data-ttu-id="5182e-207">Логическое</span><span class="sxs-lookup"><span data-stu-id="5182e-207">Boolean</span></span>|<span data-ttu-id="5182e-208">Значение, которое будет автоматически принимать условия лицензионного соглашения на устройстве ендусер.</span><span class="sxs-lookup"><span data-stu-id="5182e-208">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="5182e-209">productIds</span><span class="sxs-lookup"><span data-stu-id="5182e-209">productIds</span></span>|<span data-ttu-id="5182e-210">Коллекция [оффицепродуктид](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="5182e-210">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="5182e-211">Идентификаторы продуктов, представляющие SKU набора Office365.</span><span class="sxs-lookup"><span data-stu-id="5182e-211">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="5182e-212">Возможные значения: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="5182e-212">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="5182e-213">excludedApps</span><span class="sxs-lookup"><span data-stu-id="5182e-213">excludedApps</span></span>|<span data-ttu-id="5182e-214">[excludedApps](../resources/intune-apps-excludedapps.md);</span><span class="sxs-lookup"><span data-stu-id="5182e-214">[excludedApps](../resources/intune-apps-excludedapps.md)</span></span>|<span data-ttu-id="5182e-215">Свойство для представления приложений, исключаемых из выбранного идентификатора продукта Office365.</span><span class="sxs-lookup"><span data-stu-id="5182e-215">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="5182e-216">Свойства usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="5182e-216">useSharedComputerActivation</span></span>|<span data-ttu-id="5182e-217">Логическое</span><span class="sxs-lookup"><span data-stu-id="5182e-217">Boolean</span></span>|<span data-ttu-id="5182e-218">Свойство для представления того, используется ли активация на общем компьютере не для приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="5182e-218">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="5182e-219">updateChannel</span><span class="sxs-lookup"><span data-stu-id="5182e-219">updateChannel</span></span>|[<span data-ttu-id="5182e-220">оффицеупдатечаннел</span><span class="sxs-lookup"><span data-stu-id="5182e-220">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="5182e-221">Свойство для представления канала обновления Office365.</span><span class="sxs-lookup"><span data-stu-id="5182e-221">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="5182e-222">Возможные значения: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="5182e-222">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="5182e-223">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="5182e-223">officePlatformArchitecture</span></span>|[<span data-ttu-id="5182e-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="5182e-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="5182e-225">Свойство для представления версии набора приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="5182e-225">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="5182e-226">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="5182e-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="5182e-227">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="5182e-227">localesToInstall</span></span>|<span data-ttu-id="5182e-228">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5182e-228">String collection</span></span>|<span data-ttu-id="5182e-229">Свойство для представления языковых стандартов, устанавливаемых при установке приложений из Office365.</span><span class="sxs-lookup"><span data-stu-id="5182e-229">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="5182e-230">В нем используется стандартная спецификация RFC 6033.</span><span class="sxs-lookup"><span data-stu-id="5182e-230">It uses standard RFC 6033.</span></span> <span data-ttu-id="5182e-231">Словомhttps://technet.microsoft.com/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="5182e-231">Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="5182e-232">инсталлпрогрессдисплайлевел</span><span class="sxs-lookup"><span data-stu-id="5182e-232">installProgressDisplayLevel</span></span>|[<span data-ttu-id="5182e-233">оффицесуитеинсталлпрогрессдисплайлевел</span><span class="sxs-lookup"><span data-stu-id="5182e-233">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="5182e-234">Для указания уровня отображения пользовательского интерфейса установки хода установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5182e-234">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="5182e-235">Возможные значения: `none`, `full`.</span><span class="sxs-lookup"><span data-stu-id="5182e-235">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="5182e-236">шаулдунинсталлолдерверсионсофоффице</span><span class="sxs-lookup"><span data-stu-id="5182e-236">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="5182e-237">Логическое</span><span class="sxs-lookup"><span data-stu-id="5182e-237">Boolean</span></span>|<span data-ttu-id="5182e-238">Свойство, определяющее, следует ли удалить существующий MSI Office, если на устройстве развернут набор приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="5182e-238">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="5182e-239">Атрибута targetversion</span><span class="sxs-lookup"><span data-stu-id="5182e-239">targetVersion</span></span>|<span data-ttu-id="5182e-240">String</span><span class="sxs-lookup"><span data-stu-id="5182e-240">String</span></span>|<span data-ttu-id="5182e-241">Свойство, представляющее определенную целевую версию для набора приложений Office365, который должен быть развернут на устройствах.</span><span class="sxs-lookup"><span data-stu-id="5182e-241">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="5182e-242">упдатеверсион</span><span class="sxs-lookup"><span data-stu-id="5182e-242">updateVersion</span></span>|<span data-ttu-id="5182e-243">String</span><span class="sxs-lookup"><span data-stu-id="5182e-243">String</span></span>|<span data-ttu-id="5182e-244">Свойство для представления версии обновления, в которой определенная Целевая версия доступна для набора приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="5182e-244">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="5182e-245">оффицеконфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="5182e-245">officeConfigurationXml</span></span>|<span data-ttu-id="5182e-246">Binary</span><span class="sxs-lookup"><span data-stu-id="5182e-246">Binary</span></span>|<span data-ttu-id="5182e-247">Свойство, представляющее XML-файл конфигурации, который можно указать для приложений Office профессиональный плюс.</span><span class="sxs-lookup"><span data-stu-id="5182e-247">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="5182e-248">Имеет приоритет над всеми другими свойствами.</span><span class="sxs-lookup"><span data-stu-id="5182e-248">Takes precedence over all other properties.</span></span> <span data-ttu-id="5182e-249">Если этот параметр указан, для создания приложения будет использоваться XML-файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="5182e-249">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="5182e-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="5182e-250">Response</span></span>
<span data-ttu-id="5182e-251">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5182e-251">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5182e-252">Пример</span><span class="sxs-lookup"><span data-stu-id="5182e-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="5182e-253">Запрос</span><span class="sxs-lookup"><span data-stu-id="5182e-253">Request</span></span>
<span data-ttu-id="5182e-254">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5182e-254">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5182e-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="5182e-255">Response</span></span>
<span data-ttu-id="5182e-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5182e-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



