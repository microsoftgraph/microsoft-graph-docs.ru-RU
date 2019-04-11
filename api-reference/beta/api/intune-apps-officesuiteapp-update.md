---
title: Обновление officeSuiteApp
description: Обновление свойств объекта officeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 476e7ef602c60871f64c510c5e7cea507d64c3b5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795690"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="b6b92-103">Обновление officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="b6b92-103">Update officeSuiteApp</span></span>

> <span data-ttu-id="b6b92-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6b92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6b92-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6b92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6b92-106">Обновление свойств объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="b6b92-106">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6b92-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b6b92-107">Prerequisites</span></span>
<span data-ttu-id="b6b92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6b92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6b92-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6b92-110">Permission type</span></span>|<span data-ttu-id="b6b92-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6b92-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6b92-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6b92-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6b92-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6b92-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b6b92-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6b92-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6b92-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6b92-115">Not supported.</span></span>|
|<span data-ttu-id="b6b92-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6b92-116">Application</span></span>|<span data-ttu-id="b6b92-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6b92-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6b92-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6b92-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b6b92-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6b92-119">Request headers</span></span>
|<span data-ttu-id="b6b92-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b6b92-120">Header</span></span>|<span data-ttu-id="b6b92-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b6b92-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6b92-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6b92-122">Authorization</span></span>|<span data-ttu-id="b6b92-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6b92-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6b92-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b6b92-124">Accept</span></span>|<span data-ttu-id="b6b92-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6b92-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6b92-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6b92-126">Request body</span></span>
<span data-ttu-id="b6b92-127">В тексте запроса добавьте представление объекта [OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6b92-127">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="b6b92-128">В следующей таблице приведены свойства, необходимые при создании [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-128">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="b6b92-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6b92-129">Property</span></span>|<span data-ttu-id="b6b92-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b6b92-130">Type</span></span>|<span data-ttu-id="b6b92-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b6b92-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6b92-132">id</span><span class="sxs-lookup"><span data-stu-id="b6b92-132">id</span></span>|<span data-ttu-id="b6b92-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b6b92-133">String</span></span>|<span data-ttu-id="b6b92-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b6b92-134">Key of the entity.</span></span> <span data-ttu-id="b6b92-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b6b92-136">displayName</span></span>|<span data-ttu-id="b6b92-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b6b92-137">String</span></span>|<span data-ttu-id="b6b92-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b6b92-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b6b92-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-140">description</span><span class="sxs-lookup"><span data-stu-id="b6b92-140">description</span></span>|<span data-ttu-id="b6b92-141">String</span><span class="sxs-lookup"><span data-stu-id="b6b92-141">String</span></span>|<span data-ttu-id="b6b92-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b92-142">The description of the app.</span></span> <span data-ttu-id="b6b92-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b6b92-144">publisher</span></span>|<span data-ttu-id="b6b92-145">String</span><span class="sxs-lookup"><span data-stu-id="b6b92-145">String</span></span>|<span data-ttu-id="b6b92-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b92-146">The publisher of the app.</span></span> <span data-ttu-id="b6b92-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b6b92-148">largeIcon</span></span>|[<span data-ttu-id="b6b92-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b6b92-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b6b92-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b6b92-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b6b92-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6b92-152">createdDateTime</span></span>|<span data-ttu-id="b6b92-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6b92-153">DateTimeOffset</span></span>|<span data-ttu-id="b6b92-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b92-154">The date and time the app was created.</span></span> <span data-ttu-id="b6b92-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6b92-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b6b92-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6b92-157">DateTimeOffset</span></span>|<span data-ttu-id="b6b92-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b92-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b6b92-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b6b92-160">isFeatured</span></span>|<span data-ttu-id="b6b92-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6b92-161">Boolean</span></span>|<span data-ttu-id="b6b92-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b6b92-163">privacyInformationUrl</span></span>|<span data-ttu-id="b6b92-164">String</span><span class="sxs-lookup"><span data-stu-id="b6b92-164">String</span></span>|<span data-ttu-id="b6b92-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b6b92-165">The privacy statement Url.</span></span> <span data-ttu-id="b6b92-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b6b92-167">informationUrl</span></span>|<span data-ttu-id="b6b92-168">String</span><span class="sxs-lookup"><span data-stu-id="b6b92-168">String</span></span>|<span data-ttu-id="b6b92-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b6b92-169">The more information Url.</span></span> <span data-ttu-id="b6b92-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-171">owner</span><span class="sxs-lookup"><span data-stu-id="b6b92-171">owner</span></span>|<span data-ttu-id="b6b92-172">String</span><span class="sxs-lookup"><span data-stu-id="b6b92-172">String</span></span>|<span data-ttu-id="b6b92-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b92-173">The owner of the app.</span></span> <span data-ttu-id="b6b92-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-175">developer</span><span class="sxs-lookup"><span data-stu-id="b6b92-175">developer</span></span>|<span data-ttu-id="b6b92-176">String</span><span class="sxs-lookup"><span data-stu-id="b6b92-176">String</span></span>|<span data-ttu-id="b6b92-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b92-177">The developer of the app.</span></span> <span data-ttu-id="b6b92-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-179">notes</span><span class="sxs-lookup"><span data-stu-id="b6b92-179">notes</span></span>|<span data-ttu-id="b6b92-180">String</span><span class="sxs-lookup"><span data-stu-id="b6b92-180">String</span></span>|<span data-ttu-id="b6b92-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b92-181">Notes for the app.</span></span> <span data-ttu-id="b6b92-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b6b92-183">uploadState</span></span>|<span data-ttu-id="b6b92-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b92-184">Int32</span></span>|<span data-ttu-id="b6b92-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="b6b92-185">The upload state.</span></span> <span data-ttu-id="b6b92-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b6b92-187">publishingState</span></span>|[<span data-ttu-id="b6b92-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="b6b92-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b6b92-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b92-189">The publishing state for the app.</span></span> <span data-ttu-id="b6b92-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b6b92-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b6b92-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b6b92-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b6b92-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b6b92-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b6b92-193">isAssigned</span></span>|<span data-ttu-id="b6b92-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6b92-194">Boolean</span></span>|<span data-ttu-id="b6b92-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="b6b92-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b6b92-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b6b92-197">roleScopeTagIds</span></span>|<span data-ttu-id="b6b92-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b6b92-198">String collection</span></span>|<span data-ttu-id="b6b92-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b92-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b6b92-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="b6b92-201">dependentAppCount</span></span>|<span data-ttu-id="b6b92-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b92-202">Int32</span></span>|<span data-ttu-id="b6b92-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b92-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b6b92-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6b92-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b6b92-205">Аутоакцептеула</span><span class="sxs-lookup"><span data-stu-id="b6b92-205">autoAcceptEula</span></span>|<span data-ttu-id="b6b92-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6b92-206">Boolean</span></span>|<span data-ttu-id="b6b92-207">Значение, которое будет автоматически принимать условия ЛИЦЕНЗИОНного соглашения на устройстве ендусер.</span><span class="sxs-lookup"><span data-stu-id="b6b92-207">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="b6b92-208">productIds</span><span class="sxs-lookup"><span data-stu-id="b6b92-208">productIds</span></span>|<span data-ttu-id="b6b92-209">Коллекция [оффицепродуктид](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="b6b92-209">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="b6b92-210">Идентификаторы продуктов, представляющие SKU набора Office365.</span><span class="sxs-lookup"><span data-stu-id="b6b92-210">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="b6b92-211">Возможные значения: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="b6b92-211">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="b6b92-212">excludedApps</span><span class="sxs-lookup"><span data-stu-id="b6b92-212">excludedApps</span></span>|[<span data-ttu-id="b6b92-213">excludedApps</span><span class="sxs-lookup"><span data-stu-id="b6b92-213">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="b6b92-214">Свойство для представления приложений, исключаемых из выбранного идентификатора продукта Office365.</span><span class="sxs-lookup"><span data-stu-id="b6b92-214">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="b6b92-215">Свойства usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="b6b92-215">useSharedComputerActivation</span></span>|<span data-ttu-id="b6b92-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6b92-216">Boolean</span></span>|<span data-ttu-id="b6b92-217">Свойство для представления того, используется ли активация на общем компьютере не для приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="b6b92-217">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="b6b92-218">updateChannel</span><span class="sxs-lookup"><span data-stu-id="b6b92-218">updateChannel</span></span>|[<span data-ttu-id="b6b92-219">Оффицеупдатечаннел</span><span class="sxs-lookup"><span data-stu-id="b6b92-219">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="b6b92-220">Свойство для представления канала обновления Office365.</span><span class="sxs-lookup"><span data-stu-id="b6b92-220">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="b6b92-221">Возможные значения: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="b6b92-221">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="b6b92-222">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="b6b92-222">officePlatformArchitecture</span></span>|[<span data-ttu-id="b6b92-223">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b6b92-223">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b6b92-224">Свойство для представления версии набора приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="b6b92-224">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="b6b92-225">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="b6b92-225">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b6b92-226">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="b6b92-226">localesToInstall</span></span>|<span data-ttu-id="b6b92-227">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b6b92-227">String collection</span></span>|<span data-ttu-id="b6b92-228">Свойство для представления языковых стандартов, устанавливаемых при установке приложений из Office365.</span><span class="sxs-lookup"><span data-stu-id="b6b92-228">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="b6b92-229">В нем используется стандартная спецификация RFC 6033.</span><span class="sxs-lookup"><span data-stu-id="b6b92-229">It uses standard RFC 6033.</span></span> <span data-ttu-id="b6b92-230">Словомhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="b6b92-230">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="b6b92-231">Инсталлпрогрессдисплайлевел</span><span class="sxs-lookup"><span data-stu-id="b6b92-231">installProgressDisplayLevel</span></span>|[<span data-ttu-id="b6b92-232">Оффицесуитеинсталлпрогрессдисплайлевел</span><span class="sxs-lookup"><span data-stu-id="b6b92-232">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="b6b92-233">Для указания уровня отображения ПОЛЬЗОВАТЕЛЬСКОГО интерфейса установки хода установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="b6b92-233">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="b6b92-234">Возможные значения: `none`, `full`.</span><span class="sxs-lookup"><span data-stu-id="b6b92-234">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="b6b92-235">Шаулдунинсталлолдерверсионсофоффице</span><span class="sxs-lookup"><span data-stu-id="b6b92-235">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="b6b92-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6b92-236">Boolean</span></span>|<span data-ttu-id="b6b92-237">Свойство, определяющее, следует ли удалить существующий MSI Office, если на устройстве развернут набор приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="b6b92-237">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="b6b92-238">Атрибута targetversion</span><span class="sxs-lookup"><span data-stu-id="b6b92-238">targetVersion</span></span>|<span data-ttu-id="b6b92-239">String</span><span class="sxs-lookup"><span data-stu-id="b6b92-239">String</span></span>|<span data-ttu-id="b6b92-240">Свойство, представляющее определенную целевую версию для набора приложений Office365, который должен быть развернут на устройствах.</span><span class="sxs-lookup"><span data-stu-id="b6b92-240">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="b6b92-241">Упдатеверсион</span><span class="sxs-lookup"><span data-stu-id="b6b92-241">updateVersion</span></span>|<span data-ttu-id="b6b92-242">String</span><span class="sxs-lookup"><span data-stu-id="b6b92-242">String</span></span>|<span data-ttu-id="b6b92-243">Свойство для представления версии обновления, в которой определенная Целевая версия доступна для набора приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="b6b92-243">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="b6b92-244">Оффицеконфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="b6b92-244">officeConfigurationXml</span></span>|<span data-ttu-id="b6b92-245">Binary</span><span class="sxs-lookup"><span data-stu-id="b6b92-245">Binary</span></span>|<span data-ttu-id="b6b92-246">Свойство, представляющее XML-файл конфигурации, который можно указать для приложений Office профессиональный плюс.</span><span class="sxs-lookup"><span data-stu-id="b6b92-246">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="b6b92-247">Имеет приоритет над всеми другими свойствами.</span><span class="sxs-lookup"><span data-stu-id="b6b92-247">Takes precedence over all other properties.</span></span> <span data-ttu-id="b6b92-248">Если этот параметр указан, для создания приложения будет использоваться XML-файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="b6b92-248">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="b6b92-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6b92-249">Response</span></span>
<span data-ttu-id="b6b92-250">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6b92-250">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6b92-251">Пример</span><span class="sxs-lookup"><span data-stu-id="b6b92-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6b92-252">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6b92-252">Request</span></span>
<span data-ttu-id="b6b92-253">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b6b92-253">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="b6b92-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6b92-254">Response</span></span>
<span data-ttu-id="b6b92-p125">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b6b92-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





