---
title: Создание officeSuiteApp
description: Создание нового объекта officeSuiteApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c1821c88f974bf61fe23de6bb34cfeb06d9250f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405844"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="64d75-103">Создание officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="64d75-103">Create officeSuiteApp</span></span>

> <span data-ttu-id="64d75-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64d75-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="64d75-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64d75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64d75-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64d75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64d75-107">Создание нового объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="64d75-107">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64d75-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="64d75-108">Prerequisites</span></span>
<span data-ttu-id="64d75-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="64d75-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64d75-111">Permission type</span></span>|<span data-ttu-id="64d75-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64d75-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64d75-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64d75-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64d75-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64d75-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="64d75-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64d75-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64d75-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64d75-116">Not supported.</span></span>|
|<span data-ttu-id="64d75-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64d75-117">Application</span></span>|<span data-ttu-id="64d75-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64d75-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64d75-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64d75-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="64d75-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64d75-120">Request headers</span></span>
|<span data-ttu-id="64d75-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64d75-121">Header</span></span>|<span data-ttu-id="64d75-122">Значение</span><span class="sxs-lookup"><span data-stu-id="64d75-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64d75-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64d75-123">Authorization</span></span>|<span data-ttu-id="64d75-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="64d75-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64d75-125">Accept</span><span class="sxs-lookup"><span data-stu-id="64d75-125">Accept</span></span>|<span data-ttu-id="64d75-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64d75-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64d75-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64d75-127">Request body</span></span>
<span data-ttu-id="64d75-128">В тексте запроса укажите представление JSON для объекта officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="64d75-128">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="64d75-129">В следующей таблице показаны свойства, которые необходимы для создания officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="64d75-129">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="64d75-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="64d75-130">Property</span></span>|<span data-ttu-id="64d75-131">Тип</span><span class="sxs-lookup"><span data-stu-id="64d75-131">Type</span></span>|<span data-ttu-id="64d75-132">Описание</span><span class="sxs-lookup"><span data-stu-id="64d75-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64d75-133">id</span><span class="sxs-lookup"><span data-stu-id="64d75-133">id</span></span>|<span data-ttu-id="64d75-134">String</span><span class="sxs-lookup"><span data-stu-id="64d75-134">String</span></span>|<span data-ttu-id="64d75-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="64d75-135">Key of the entity.</span></span> <span data-ttu-id="64d75-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-137">displayName</span><span class="sxs-lookup"><span data-stu-id="64d75-137">displayName</span></span>|<span data-ttu-id="64d75-138">String</span><span class="sxs-lookup"><span data-stu-id="64d75-138">String</span></span>|<span data-ttu-id="64d75-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="64d75-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="64d75-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-141">description</span><span class="sxs-lookup"><span data-stu-id="64d75-141">description</span></span>|<span data-ttu-id="64d75-142">String</span><span class="sxs-lookup"><span data-stu-id="64d75-142">String</span></span>|<span data-ttu-id="64d75-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="64d75-143">The description of the app.</span></span> <span data-ttu-id="64d75-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-145">publisher</span><span class="sxs-lookup"><span data-stu-id="64d75-145">publisher</span></span>|<span data-ttu-id="64d75-146">String</span><span class="sxs-lookup"><span data-stu-id="64d75-146">String</span></span>|<span data-ttu-id="64d75-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="64d75-147">The publisher of the app.</span></span> <span data-ttu-id="64d75-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="64d75-149">largeIcon</span></span>|[<span data-ttu-id="64d75-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="64d75-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="64d75-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="64d75-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="64d75-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64d75-153">createdDateTime</span></span>|<span data-ttu-id="64d75-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64d75-154">DateTimeOffset</span></span>|<span data-ttu-id="64d75-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="64d75-155">The date and time the app was created.</span></span> <span data-ttu-id="64d75-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64d75-157">lastModifiedDateTime</span></span>|<span data-ttu-id="64d75-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64d75-158">DateTimeOffset</span></span>|<span data-ttu-id="64d75-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="64d75-159">The date and time the app was last modified.</span></span> <span data-ttu-id="64d75-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="64d75-161">isFeatured</span></span>|<span data-ttu-id="64d75-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="64d75-162">Boolean</span></span>|<span data-ttu-id="64d75-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="64d75-164">privacyInformationUrl</span></span>|<span data-ttu-id="64d75-165">String</span><span class="sxs-lookup"><span data-stu-id="64d75-165">String</span></span>|<span data-ttu-id="64d75-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="64d75-166">The privacy statement Url.</span></span> <span data-ttu-id="64d75-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="64d75-168">informationUrl</span></span>|<span data-ttu-id="64d75-169">String</span><span class="sxs-lookup"><span data-stu-id="64d75-169">String</span></span>|<span data-ttu-id="64d75-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="64d75-170">The more information Url.</span></span> <span data-ttu-id="64d75-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-172">owner</span><span class="sxs-lookup"><span data-stu-id="64d75-172">owner</span></span>|<span data-ttu-id="64d75-173">String</span><span class="sxs-lookup"><span data-stu-id="64d75-173">String</span></span>|<span data-ttu-id="64d75-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="64d75-174">The owner of the app.</span></span> <span data-ttu-id="64d75-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-176">developer</span><span class="sxs-lookup"><span data-stu-id="64d75-176">developer</span></span>|<span data-ttu-id="64d75-177">String</span><span class="sxs-lookup"><span data-stu-id="64d75-177">String</span></span>|<span data-ttu-id="64d75-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="64d75-178">The developer of the app.</span></span> <span data-ttu-id="64d75-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-180">notes</span><span class="sxs-lookup"><span data-stu-id="64d75-180">notes</span></span>|<span data-ttu-id="64d75-181">String</span><span class="sxs-lookup"><span data-stu-id="64d75-181">String</span></span>|<span data-ttu-id="64d75-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="64d75-182">Notes for the app.</span></span> <span data-ttu-id="64d75-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="64d75-184">uploadState</span></span>|<span data-ttu-id="64d75-185">Int32</span><span class="sxs-lookup"><span data-stu-id="64d75-185">Int32</span></span>|<span data-ttu-id="64d75-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="64d75-186">The upload state.</span></span> <span data-ttu-id="64d75-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="64d75-188">publishingState</span></span>|[<span data-ttu-id="64d75-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="64d75-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="64d75-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="64d75-190">The publishing state for the app.</span></span> <span data-ttu-id="64d75-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="64d75-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="64d75-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="64d75-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="64d75-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="64d75-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="64d75-194">isAssigned</span></span>|<span data-ttu-id="64d75-195">Логический</span><span class="sxs-lookup"><span data-stu-id="64d75-195">Boolean</span></span>|<span data-ttu-id="64d75-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="64d75-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="64d75-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64d75-198">roleScopeTagIds</span></span>|<span data-ttu-id="64d75-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="64d75-199">String collection</span></span>|<span data-ttu-id="64d75-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="64d75-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="64d75-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64d75-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="64d75-202">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="64d75-202">autoAcceptEula</span></span>|<span data-ttu-id="64d75-203">Логический</span><span class="sxs-lookup"><span data-stu-id="64d75-203">Boolean</span></span>|<span data-ttu-id="64d75-204">Значение, чтобы принять условия лицензионного соглашения автоматически на устройстве enduser.</span><span class="sxs-lookup"><span data-stu-id="64d75-204">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="64d75-205">productIds</span><span class="sxs-lookup"><span data-stu-id="64d75-205">productIds</span></span>|<span data-ttu-id="64d75-206">[officeProductId](../resources/intune-apps-officeproductid.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="64d75-206">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="64d75-207">Коды продуктов, представляющих SKU набора приложений Office 365.</span><span class="sxs-lookup"><span data-stu-id="64d75-207">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="64d75-208">Возможные значения: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="64d75-208">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="64d75-209">excludedApps;</span><span class="sxs-lookup"><span data-stu-id="64d75-209">excludedApps</span></span>|<span data-ttu-id="64d75-210">[excludedApps](../resources/intune-apps-excludedapps.md);</span><span class="sxs-lookup"><span data-stu-id="64d75-210">[excludedApps](../resources/intune-apps-excludedapps.md)</span></span>|<span data-ttu-id="64d75-211">Свойство для представления приложения, исключенных из выбранного продукта Office 365 идентификатор.</span><span class="sxs-lookup"><span data-stu-id="64d75-211">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="64d75-212">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="64d75-212">useSharedComputerActivation</span></span>|<span data-ttu-id="64d75-213">Логический</span><span class="sxs-lookup"><span data-stu-id="64d75-213">Boolean</span></span>|<span data-ttu-id="64d75-214">Свойство для представления, является ли активация совместно используемый компьютер используется не для набора приложений Office 365.</span><span class="sxs-lookup"><span data-stu-id="64d75-214">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="64d75-215">updateChannel</span><span class="sxs-lookup"><span data-stu-id="64d75-215">updateChannel</span></span>|[<span data-ttu-id="64d75-216">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="64d75-216">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="64d75-217">Свойство для представления канала обновления Office 365.</span><span class="sxs-lookup"><span data-stu-id="64d75-217">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="64d75-218">Возможные значения: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="64d75-218">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="64d75-219">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="64d75-219">officePlatformArchitecture</span></span>|[<span data-ttu-id="64d75-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="64d75-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="64d75-221">Свойство для представления версию пакета приложения Office 365.</span><span class="sxs-lookup"><span data-stu-id="64d75-221">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="64d75-222">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="64d75-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="64d75-223">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="64d75-223">localesToInstall</span></span>|<span data-ttu-id="64d75-224">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="64d75-224">String collection</span></span>|<span data-ttu-id="64d75-225">Свойство для представления языковых стандартов, которые устанавливаются при установке приложения из Office 365.</span><span class="sxs-lookup"><span data-stu-id="64d75-225">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="64d75-226">Используется стандартный 6033 RFC.</span><span class="sxs-lookup"><span data-stu-id="64d75-226">It uses standard RFC 6033.</span></span> <span data-ttu-id="64d75-227">Параметры REF:https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="64d75-227">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="64d75-228">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="64d75-228">installProgressDisplayLevel</span></span>|[<span data-ttu-id="64d75-229">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="64d75-229">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="64d75-230">Чтобы задать уровень отображения для пользовательского интерфейса программы установки ход выполнения установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="64d75-230">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="64d75-231">Возможные значения: `none`, `full`.</span><span class="sxs-lookup"><span data-stu-id="64d75-231">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="64d75-232">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="64d75-232">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="64d75-233">Логический</span><span class="sxs-lookup"><span data-stu-id="64d75-233">Boolean</span></span>|<span data-ttu-id="64d75-234">Свойство, позволяющее определить, нужно ли удалить существующий MSI Office, если пакет приложений Office 365 развертывается на устройство или нет.</span><span class="sxs-lookup"><span data-stu-id="64d75-234">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="64d75-235">targetVersion</span><span class="sxs-lookup"><span data-stu-id="64d75-235">targetVersion</span></span>|<span data-ttu-id="64d75-236">String</span><span class="sxs-lookup"><span data-stu-id="64d75-236">String</span></span>|<span data-ttu-id="64d75-237">Свойство для представления конкретной версия набора приложений Office 365, должны оставаться развернутое на устройствах.</span><span class="sxs-lookup"><span data-stu-id="64d75-237">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="64d75-238">updateVersion</span><span class="sxs-lookup"><span data-stu-id="64d75-238">updateVersion</span></span>|<span data-ttu-id="64d75-239">String</span><span class="sxs-lookup"><span data-stu-id="64d75-239">String</span></span>|<span data-ttu-id="64d75-240">Свойство для представления версии обновления, в котором версия целевой доступна для набора приложений Office 365.</span><span class="sxs-lookup"><span data-stu-id="64d75-240">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="64d75-241">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="64d75-241">officeConfigurationXml</span></span>|<span data-ttu-id="64d75-242">Binary</span><span class="sxs-lookup"><span data-stu-id="64d75-242">Binary</span></span>|<span data-ttu-id="64d75-243">Свойство для представления XML-файл конфигурации, который может использоваться для приложений Office профессиональный плюс.</span><span class="sxs-lookup"><span data-stu-id="64d75-243">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="64d75-244">Приоритет над другие свойства.</span><span class="sxs-lookup"><span data-stu-id="64d75-244">Takes precedence over all other properties.</span></span> <span data-ttu-id="64d75-245">Если этот параметр указан, XML-файл конфигурации будет использоваться для создания приложения.</span><span class="sxs-lookup"><span data-stu-id="64d75-245">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="64d75-246">Отклик</span><span class="sxs-lookup"><span data-stu-id="64d75-246">Response</span></span>
<span data-ttu-id="64d75-247">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="64d75-247">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64d75-248">Пример</span><span class="sxs-lookup"><span data-stu-id="64d75-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="64d75-249">Запрос</span><span class="sxs-lookup"><span data-stu-id="64d75-249">Request</span></span>
<span data-ttu-id="64d75-250">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64d75-250">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="64d75-251">Отклик</span><span class="sxs-lookup"><span data-stu-id="64d75-251">Response</span></span>
<span data-ttu-id="64d75-p125">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="64d75-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




