---
title: Обновление officeSuiteApp
description: Обновление свойства объекта officeSuiteApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 24d5a8031580fa1d7cfe74415d84de32f49fa398
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979329"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="8f984-103">Обновление officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="8f984-103">Update officeSuiteApp</span></span>

> <span data-ttu-id="8f984-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8f984-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f984-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f984-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f984-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8f984-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f984-107">Обновление свойства объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8f984-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f984-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8f984-108">Prerequisites</span></span>
<span data-ttu-id="8f984-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f984-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f984-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f984-111">Permission type</span></span>|<span data-ttu-id="8f984-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f984-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f984-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f984-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f984-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f984-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8f984-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f984-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f984-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f984-116">Not supported.</span></span>|
|<span data-ttu-id="8f984-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f984-117">Application</span></span>|<span data-ttu-id="8f984-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f984-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f984-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f984-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8f984-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f984-120">Request headers</span></span>
|<span data-ttu-id="8f984-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f984-121">Header</span></span>|<span data-ttu-id="8f984-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8f984-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f984-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f984-123">Authorization</span></span>|<span data-ttu-id="8f984-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8f984-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f984-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8f984-125">Accept</span></span>|<span data-ttu-id="8f984-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f984-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f984-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f984-127">Request body</span></span>
<span data-ttu-id="8f984-128">В тексте запроса укажите представление JSON для объекта [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="8f984-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="8f984-129">В следующей таблице показаны свойства, которые необходимы для создания [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="8f984-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f984-130">Property</span></span>|<span data-ttu-id="8f984-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8f984-131">Type</span></span>|<span data-ttu-id="8f984-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8f984-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f984-133">id</span><span class="sxs-lookup"><span data-stu-id="8f984-133">id</span></span>|<span data-ttu-id="8f984-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8f984-134">String</span></span>|<span data-ttu-id="8f984-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8f984-135">Key of the entity.</span></span> <span data-ttu-id="8f984-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8f984-137">displayName</span></span>|<span data-ttu-id="8f984-138">String</span><span class="sxs-lookup"><span data-stu-id="8f984-138">String</span></span>|<span data-ttu-id="8f984-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="8f984-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8f984-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-141">описание</span><span class="sxs-lookup"><span data-stu-id="8f984-141">description</span></span>|<span data-ttu-id="8f984-142">String</span><span class="sxs-lookup"><span data-stu-id="8f984-142">String</span></span>|<span data-ttu-id="8f984-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="8f984-143">The description of the app.</span></span> <span data-ttu-id="8f984-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8f984-145">publisher</span></span>|<span data-ttu-id="8f984-146">String</span><span class="sxs-lookup"><span data-stu-id="8f984-146">String</span></span>|<span data-ttu-id="8f984-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="8f984-147">The publisher of the app.</span></span> <span data-ttu-id="8f984-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8f984-149">largeIcon</span></span>|[<span data-ttu-id="8f984-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8f984-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8f984-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="8f984-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8f984-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f984-153">createdDateTime</span></span>|<span data-ttu-id="8f984-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f984-154">DateTimeOffset</span></span>|<span data-ttu-id="8f984-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="8f984-155">The date and time the app was created.</span></span> <span data-ttu-id="8f984-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f984-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8f984-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f984-158">DateTimeOffset</span></span>|<span data-ttu-id="8f984-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="8f984-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8f984-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8f984-161">isFeatured</span></span>|<span data-ttu-id="8f984-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f984-162">Boolean</span></span>|<span data-ttu-id="8f984-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8f984-164">privacyInformationUrl</span></span>|<span data-ttu-id="8f984-165">String</span><span class="sxs-lookup"><span data-stu-id="8f984-165">String</span></span>|<span data-ttu-id="8f984-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8f984-166">The privacy statement Url.</span></span> <span data-ttu-id="8f984-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8f984-168">informationUrl</span></span>|<span data-ttu-id="8f984-169">String</span><span class="sxs-lookup"><span data-stu-id="8f984-169">String</span></span>|<span data-ttu-id="8f984-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="8f984-170">The more information Url.</span></span> <span data-ttu-id="8f984-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-172">owner</span><span class="sxs-lookup"><span data-stu-id="8f984-172">owner</span></span>|<span data-ttu-id="8f984-173">String</span><span class="sxs-lookup"><span data-stu-id="8f984-173">String</span></span>|<span data-ttu-id="8f984-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="8f984-174">The owner of the app.</span></span> <span data-ttu-id="8f984-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-176">developer</span><span class="sxs-lookup"><span data-stu-id="8f984-176">developer</span></span>|<span data-ttu-id="8f984-177">String</span><span class="sxs-lookup"><span data-stu-id="8f984-177">String</span></span>|<span data-ttu-id="8f984-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="8f984-178">The developer of the app.</span></span> <span data-ttu-id="8f984-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-180">notes</span><span class="sxs-lookup"><span data-stu-id="8f984-180">notes</span></span>|<span data-ttu-id="8f984-181">String</span><span class="sxs-lookup"><span data-stu-id="8f984-181">String</span></span>|<span data-ttu-id="8f984-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="8f984-182">Notes for the app.</span></span> <span data-ttu-id="8f984-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8f984-184">uploadState</span></span>|<span data-ttu-id="8f984-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8f984-185">Int32</span></span>|<span data-ttu-id="8f984-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="8f984-186">The upload state.</span></span> <span data-ttu-id="8f984-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8f984-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8f984-188">publishingState</span></span>|[<span data-ttu-id="8f984-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8f984-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8f984-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="8f984-190">The publishing state for the app.</span></span> <span data-ttu-id="8f984-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="8f984-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8f984-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8f984-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8f984-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8f984-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8f984-194">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="8f984-194">autoAcceptEula</span></span>|<span data-ttu-id="8f984-195">Логический</span><span class="sxs-lookup"><span data-stu-id="8f984-195">Boolean</span></span>|<span data-ttu-id="8f984-196">Значение, чтобы принять условия лицензионного соглашения автоматически на устройстве enduser.</span><span class="sxs-lookup"><span data-stu-id="8f984-196">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="8f984-197">productIds</span><span class="sxs-lookup"><span data-stu-id="8f984-197">productIds</span></span>|<span data-ttu-id="8f984-198">[officeProductId](../resources/intune-apps-officeproductid.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8f984-198">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="8f984-199">Коды продуктов, представляющих SKU набора приложений Office 365.</span><span class="sxs-lookup"><span data-stu-id="8f984-199">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="8f984-200">Возможные значения: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="8f984-200">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="8f984-201">excludedApps;</span><span class="sxs-lookup"><span data-stu-id="8f984-201">excludedApps</span></span>|<span data-ttu-id="8f984-202">[excludedApps](../resources/intune-apps-excludedapps.md);</span><span class="sxs-lookup"><span data-stu-id="8f984-202">[excludedApps](../resources/intune-apps-excludedapps.md)</span></span>|<span data-ttu-id="8f984-203">Свойство для представления приложения, исключенных из выбранного продукта Office 365 идентификатор.</span><span class="sxs-lookup"><span data-stu-id="8f984-203">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="8f984-204">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="8f984-204">useSharedComputerActivation</span></span>|<span data-ttu-id="8f984-205">Логический</span><span class="sxs-lookup"><span data-stu-id="8f984-205">Boolean</span></span>|<span data-ttu-id="8f984-206">Свойство для представления, является ли активация совместно используемый компьютер используется не для набора приложений Office 365.</span><span class="sxs-lookup"><span data-stu-id="8f984-206">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="8f984-207">updateChannel</span><span class="sxs-lookup"><span data-stu-id="8f984-207">updateChannel</span></span>|[<span data-ttu-id="8f984-208">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="8f984-208">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="8f984-209">Свойство для представления канала обновления Office 365.</span><span class="sxs-lookup"><span data-stu-id="8f984-209">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="8f984-210">Возможные значения: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="8f984-210">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="8f984-211">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="8f984-211">officePlatformArchitecture</span></span>|[<span data-ttu-id="8f984-212">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="8f984-212">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="8f984-213">Свойство для представления версию пакета приложения Office 365.</span><span class="sxs-lookup"><span data-stu-id="8f984-213">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="8f984-214">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="8f984-214">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="8f984-215">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="8f984-215">localesToInstall</span></span>|<span data-ttu-id="8f984-216">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8f984-216">String collection</span></span>|<span data-ttu-id="8f984-217">Свойство для представления языковых стандартов, которые устанавливаются при установке приложения из Office 365.</span><span class="sxs-lookup"><span data-stu-id="8f984-217">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="8f984-218">Используется стандартный 6033 RFC.</span><span class="sxs-lookup"><span data-stu-id="8f984-218">It uses standard RFC 6033.</span></span> <span data-ttu-id="8f984-219">Параметры REF:https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="8f984-219">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="8f984-220">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="8f984-220">installProgressDisplayLevel</span></span>|[<span data-ttu-id="8f984-221">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="8f984-221">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="8f984-222">Чтобы задать уровень отображения для пользовательского интерфейса программы установки ход выполнения установки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8f984-222">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="8f984-223">Возможные значения: `none`, `full`.</span><span class="sxs-lookup"><span data-stu-id="8f984-223">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="8f984-224">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="8f984-224">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="8f984-225">Логический</span><span class="sxs-lookup"><span data-stu-id="8f984-225">Boolean</span></span>|<span data-ttu-id="8f984-226">Свойство, позволяющее определить, нужно ли удалить существующий MSI Office, если пакет приложений Office 365 развертывается на устройство или нет.</span><span class="sxs-lookup"><span data-stu-id="8f984-226">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="8f984-227">targetVersion</span><span class="sxs-lookup"><span data-stu-id="8f984-227">targetVersion</span></span>|<span data-ttu-id="8f984-228">Строка</span><span class="sxs-lookup"><span data-stu-id="8f984-228">String</span></span>|<span data-ttu-id="8f984-229">Свойство для представления конкретной версия набора приложений Office 365, должны оставаться развернутое на устройствах.</span><span class="sxs-lookup"><span data-stu-id="8f984-229">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="8f984-230">updateVersion</span><span class="sxs-lookup"><span data-stu-id="8f984-230">updateVersion</span></span>|<span data-ttu-id="8f984-231">Строка</span><span class="sxs-lookup"><span data-stu-id="8f984-231">String</span></span>|<span data-ttu-id="8f984-232">Свойство для представления версии обновления, в котором версия целевой доступна для набора приложений Office 365.</span><span class="sxs-lookup"><span data-stu-id="8f984-232">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|



## <a name="response"></a><span data-ttu-id="8f984-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f984-233">Response</span></span>
<span data-ttu-id="8f984-234">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8f984-234">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f984-235">Пример</span><span class="sxs-lookup"><span data-stu-id="8f984-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f984-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f984-236">Request</span></span>
<span data-ttu-id="8f984-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f984-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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
  "updateVersion": "Update Version value"
}
```

### <a name="response"></a><span data-ttu-id="8f984-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="8f984-238">Response</span></span>
<span data-ttu-id="8f984-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8f984-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

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
  "updateVersion": "Update Version value"
}
```





