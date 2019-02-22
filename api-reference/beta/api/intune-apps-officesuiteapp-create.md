---
title: Создание officeSuiteApp
description: Создание нового объекта officeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f58d25a38de891647b450a61b2dea03404e68bab
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157129"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="a3afc-103">Создание officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="a3afc-103">Create officeSuiteApp</span></span>

> <span data-ttu-id="a3afc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3afc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3afc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3afc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3afc-106">Создание нового объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a3afc-106">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3afc-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a3afc-107">Prerequisites</span></span>
<span data-ttu-id="a3afc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a3afc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3afc-110">Permission type</span></span>|<span data-ttu-id="a3afc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3afc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3afc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3afc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3afc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3afc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a3afc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3afc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3afc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3afc-115">Not supported.</span></span>|
|<span data-ttu-id="a3afc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3afc-116">Application</span></span>|<span data-ttu-id="a3afc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3afc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3afc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3afc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a3afc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3afc-119">Request headers</span></span>
|<span data-ttu-id="a3afc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3afc-120">Header</span></span>|<span data-ttu-id="a3afc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a3afc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3afc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3afc-122">Authorization</span></span>|<span data-ttu-id="a3afc-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a3afc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3afc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a3afc-124">Accept</span></span>|<span data-ttu-id="a3afc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3afc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3afc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3afc-126">Request body</span></span>
<span data-ttu-id="a3afc-127">В тексте запроса добавьте представление объекта officeSuiteApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3afc-127">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="a3afc-128">В следующей таблице приведены свойства, необходимые при создании officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="a3afc-128">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="a3afc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3afc-129">Property</span></span>|<span data-ttu-id="a3afc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a3afc-130">Type</span></span>|<span data-ttu-id="a3afc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a3afc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3afc-132">id</span><span class="sxs-lookup"><span data-stu-id="a3afc-132">id</span></span>|<span data-ttu-id="a3afc-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a3afc-133">String</span></span>|<span data-ttu-id="a3afc-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a3afc-134">Key of the entity.</span></span> <span data-ttu-id="a3afc-135">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a3afc-136">displayName</span></span>|<span data-ttu-id="a3afc-137">String</span><span class="sxs-lookup"><span data-stu-id="a3afc-137">String</span></span>|<span data-ttu-id="a3afc-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a3afc-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a3afc-139">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-140">description</span><span class="sxs-lookup"><span data-stu-id="a3afc-140">description</span></span>|<span data-ttu-id="a3afc-141">Строка</span><span class="sxs-lookup"><span data-stu-id="a3afc-141">String</span></span>|<span data-ttu-id="a3afc-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a3afc-142">The description of the app.</span></span> <span data-ttu-id="a3afc-143">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-144">publisher</span><span class="sxs-lookup"><span data-stu-id="a3afc-144">publisher</span></span>|<span data-ttu-id="a3afc-145">String</span><span class="sxs-lookup"><span data-stu-id="a3afc-145">String</span></span>|<span data-ttu-id="a3afc-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a3afc-146">The publisher of the app.</span></span> <span data-ttu-id="a3afc-147">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a3afc-148">largeIcon</span></span>|[<span data-ttu-id="a3afc-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a3afc-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a3afc-150">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a3afc-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a3afc-151">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3afc-152">createdDateTime</span></span>|<span data-ttu-id="a3afc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3afc-153">DateTimeOffset</span></span>|<span data-ttu-id="a3afc-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a3afc-154">The date and time the app was created.</span></span> <span data-ttu-id="a3afc-155">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3afc-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a3afc-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3afc-157">DateTimeOffset</span></span>|<span data-ttu-id="a3afc-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a3afc-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a3afc-159">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a3afc-160">isFeatured</span></span>|<span data-ttu-id="a3afc-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3afc-161">Boolean</span></span>|<span data-ttu-id="a3afc-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a3afc-163">privacyInformationUrl</span></span>|<span data-ttu-id="a3afc-164">String</span><span class="sxs-lookup"><span data-stu-id="a3afc-164">String</span></span>|<span data-ttu-id="a3afc-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a3afc-165">The privacy statement Url.</span></span> <span data-ttu-id="a3afc-166">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a3afc-167">informationUrl</span></span>|<span data-ttu-id="a3afc-168">String</span><span class="sxs-lookup"><span data-stu-id="a3afc-168">String</span></span>|<span data-ttu-id="a3afc-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a3afc-169">The more information Url.</span></span> <span data-ttu-id="a3afc-170">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-171">owner</span><span class="sxs-lookup"><span data-stu-id="a3afc-171">owner</span></span>|<span data-ttu-id="a3afc-172">String</span><span class="sxs-lookup"><span data-stu-id="a3afc-172">String</span></span>|<span data-ttu-id="a3afc-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a3afc-173">The owner of the app.</span></span> <span data-ttu-id="a3afc-174">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-175">developer</span><span class="sxs-lookup"><span data-stu-id="a3afc-175">developer</span></span>|<span data-ttu-id="a3afc-176">String</span><span class="sxs-lookup"><span data-stu-id="a3afc-176">String</span></span>|<span data-ttu-id="a3afc-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a3afc-177">The developer of the app.</span></span> <span data-ttu-id="a3afc-178">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-179">notes</span><span class="sxs-lookup"><span data-stu-id="a3afc-179">notes</span></span>|<span data-ttu-id="a3afc-180">String</span><span class="sxs-lookup"><span data-stu-id="a3afc-180">String</span></span>|<span data-ttu-id="a3afc-181">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="a3afc-181">Notes for the app.</span></span> <span data-ttu-id="a3afc-182">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="a3afc-183">uploadState</span></span>|<span data-ttu-id="a3afc-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a3afc-184">Int32</span></span>|<span data-ttu-id="a3afc-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="a3afc-185">The upload state.</span></span> <span data-ttu-id="a3afc-186">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="a3afc-187">publishingState</span></span>|[<span data-ttu-id="a3afc-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="a3afc-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a3afc-189">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="a3afc-189">The publishing state for the app.</span></span> <span data-ttu-id="a3afc-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a3afc-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a3afc-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a3afc-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a3afc-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a3afc-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a3afc-193">isAssigned</span></span>|<span data-ttu-id="a3afc-194">Логический</span><span class="sxs-lookup"><span data-stu-id="a3afc-194">Boolean</span></span>|<span data-ttu-id="a3afc-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="a3afc-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a3afc-196">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a3afc-197">roleScopeTagIds</span></span>|<span data-ttu-id="a3afc-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a3afc-198">String collection</span></span>|<span data-ttu-id="a3afc-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="a3afc-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a3afc-200">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3afc-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a3afc-201">Аутоакцептеула</span><span class="sxs-lookup"><span data-stu-id="a3afc-201">autoAcceptEula</span></span>|<span data-ttu-id="a3afc-202">Логический</span><span class="sxs-lookup"><span data-stu-id="a3afc-202">Boolean</span></span>|<span data-ttu-id="a3afc-203">Значение, которое будет автоматически принимать условия ЛИЦЕНЗИОНного соглашения на устройстве ендусер.</span><span class="sxs-lookup"><span data-stu-id="a3afc-203">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="a3afc-204">productIds</span><span class="sxs-lookup"><span data-stu-id="a3afc-204">productIds</span></span>|<span data-ttu-id="a3afc-205">Коллекция [оффицепродуктид](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="a3afc-205">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="a3afc-206">Идентификаторы продуктов, представляющие SKU набора Office365.</span><span class="sxs-lookup"><span data-stu-id="a3afc-206">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="a3afc-207">Возможные значения: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="a3afc-207">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="a3afc-208">excludedApps;</span><span class="sxs-lookup"><span data-stu-id="a3afc-208">excludedApps</span></span>|<span data-ttu-id="a3afc-209">[excludedApps](../resources/intune-apps-excludedapps.md);</span><span class="sxs-lookup"><span data-stu-id="a3afc-209">[excludedApps](../resources/intune-apps-excludedapps.md)</span></span>|<span data-ttu-id="a3afc-210">Свойство для представления приложений, исключаемых из выбранного идентификатора продукта Office365.</span><span class="sxs-lookup"><span data-stu-id="a3afc-210">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="a3afc-211">Свойства usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="a3afc-211">useSharedComputerActivation</span></span>|<span data-ttu-id="a3afc-212">Логический</span><span class="sxs-lookup"><span data-stu-id="a3afc-212">Boolean</span></span>|<span data-ttu-id="a3afc-213">Свойство для представления того, используется ли активация на общем компьютере не для приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="a3afc-213">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="a3afc-214">updateChannel</span><span class="sxs-lookup"><span data-stu-id="a3afc-214">updateChannel</span></span>|[<span data-ttu-id="a3afc-215">Оффицеупдатечаннел</span><span class="sxs-lookup"><span data-stu-id="a3afc-215">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="a3afc-216">Свойство для представления канала обновления Office365.</span><span class="sxs-lookup"><span data-stu-id="a3afc-216">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="a3afc-217">Возможные значения: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="a3afc-217">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="a3afc-218">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="a3afc-218">officePlatformArchitecture</span></span>|[<span data-ttu-id="a3afc-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a3afc-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a3afc-220">Свойство для представления версии набора приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="a3afc-220">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="a3afc-221">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="a3afc-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="a3afc-222">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="a3afc-222">localesToInstall</span></span>|<span data-ttu-id="a3afc-223">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a3afc-223">String collection</span></span>|<span data-ttu-id="a3afc-224">Свойство для представления языковых стандартов, устанавливаемых при установке приложений из Office365.</span><span class="sxs-lookup"><span data-stu-id="a3afc-224">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="a3afc-225">В нем используется стандартная спецификация RFC 6033.</span><span class="sxs-lookup"><span data-stu-id="a3afc-225">It uses standard RFC 6033.</span></span> <span data-ttu-id="a3afc-226">Словомhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="a3afc-226">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="a3afc-227">Инсталлпрогрессдисплайлевел</span><span class="sxs-lookup"><span data-stu-id="a3afc-227">installProgressDisplayLevel</span></span>|[<span data-ttu-id="a3afc-228">Оффицесуитеинсталлпрогрессдисплайлевел</span><span class="sxs-lookup"><span data-stu-id="a3afc-228">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="a3afc-229">Для указания уровня отображения ПОЛЬЗОВАТЕЛЬСКОГО интерфейса установки хода установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a3afc-229">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="a3afc-230">Возможные значения: `none`, `full`.</span><span class="sxs-lookup"><span data-stu-id="a3afc-230">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="a3afc-231">Шаулдунинсталлолдерверсионсофоффице</span><span class="sxs-lookup"><span data-stu-id="a3afc-231">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="a3afc-232">Логический</span><span class="sxs-lookup"><span data-stu-id="a3afc-232">Boolean</span></span>|<span data-ttu-id="a3afc-233">Свойство, определяющее, следует ли удалить существующий MSI Office, если на устройстве развернут набор приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="a3afc-233">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="a3afc-234">Атрибута targetversion</span><span class="sxs-lookup"><span data-stu-id="a3afc-234">targetVersion</span></span>|<span data-ttu-id="a3afc-235">String</span><span class="sxs-lookup"><span data-stu-id="a3afc-235">String</span></span>|<span data-ttu-id="a3afc-236">Свойство, представляющее определенную целевую версию для набора приложений Office365, который должен быть развернут на устройствах.</span><span class="sxs-lookup"><span data-stu-id="a3afc-236">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="a3afc-237">Упдатеверсион</span><span class="sxs-lookup"><span data-stu-id="a3afc-237">updateVersion</span></span>|<span data-ttu-id="a3afc-238">String</span><span class="sxs-lookup"><span data-stu-id="a3afc-238">String</span></span>|<span data-ttu-id="a3afc-239">Свойство для представления версии обновления, в которой определенная Целевая версия доступна для набора приложений Office365.</span><span class="sxs-lookup"><span data-stu-id="a3afc-239">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="a3afc-240">Оффицеконфигуратионксмл</span><span class="sxs-lookup"><span data-stu-id="a3afc-240">officeConfigurationXml</span></span>|<span data-ttu-id="a3afc-241">Binary</span><span class="sxs-lookup"><span data-stu-id="a3afc-241">Binary</span></span>|<span data-ttu-id="a3afc-242">Свойство, представляющее XML-файл конфигурации, который можно указать для приложений Office профессиональный плюс.</span><span class="sxs-lookup"><span data-stu-id="a3afc-242">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="a3afc-243">Имеет приоритет над всеми другими свойствами.</span><span class="sxs-lookup"><span data-stu-id="a3afc-243">Takes precedence over all other properties.</span></span> <span data-ttu-id="a3afc-244">Если этот параметр указан, для создания приложения будет использоваться XML-файл конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a3afc-244">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="a3afc-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3afc-245">Response</span></span>
<span data-ttu-id="a3afc-246">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3afc-246">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3afc-247">Пример</span><span class="sxs-lookup"><span data-stu-id="a3afc-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3afc-248">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3afc-248">Request</span></span>
<span data-ttu-id="a3afc-249">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3afc-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1552

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

### <a name="response"></a><span data-ttu-id="a3afc-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3afc-250">Response</span></span>
<span data-ttu-id="a3afc-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3afc-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1724

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




