---
title: Create iosVppApp
description: Создание объекта iosVppApp.
ms.openlocfilehash: df16640ea92296e793a6ebd965530e00112afac1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079745"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="ef0e2-103">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="ef0e2-103">Create iosVppApp</span></span>

> <span data-ttu-id="ef0e2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef0e2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef0e2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef0e2-107">Создание объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-107">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef0e2-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ef0e2-108">Prerequisites</span></span>
<span data-ttu-id="ef0e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef0e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef0e2-111">Permission type</span></span>|<span data-ttu-id="ef0e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef0e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef0e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef0e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef0e2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef0e2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef0e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef0e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef0e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-116">Not supported.</span></span>|
|<span data-ttu-id="ef0e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef0e2-117">Application</span></span>|<span data-ttu-id="ef0e2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef0e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef0e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ef0e2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef0e2-120">Request headers</span></span>
|<span data-ttu-id="ef0e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef0e2-121">Header</span></span>|<span data-ttu-id="ef0e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ef0e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef0e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef0e2-123">Authorization</span></span>|<span data-ttu-id="ef0e2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ef0e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef0e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef0e2-125">Accept</span></span>|<span data-ttu-id="ef0e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef0e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef0e2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef0e2-127">Request body</span></span>
<span data-ttu-id="ef0e2-128">В тексте запроса добавьте представление объекта iosVppApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-128">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="ef0e2-129">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-129">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="ef0e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef0e2-130">Property</span></span>|<span data-ttu-id="ef0e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ef0e2-131">Type</span></span>|<span data-ttu-id="ef0e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ef0e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef0e2-133">id</span><span class="sxs-lookup"><span data-stu-id="ef0e2-133">id</span></span>|<span data-ttu-id="ef0e2-134">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-134">String</span></span>|<span data-ttu-id="ef0e2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-135">Key of the entity.</span></span> <span data-ttu-id="ef0e2-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ef0e2-137">displayName</span></span>|<span data-ttu-id="ef0e2-138">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-138">String</span></span>|<span data-ttu-id="ef0e2-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ef0e2-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-141">описание</span><span class="sxs-lookup"><span data-stu-id="ef0e2-141">description</span></span>|<span data-ttu-id="ef0e2-142">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-142">String</span></span>|<span data-ttu-id="ef0e2-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-143">The description of the app.</span></span> <span data-ttu-id="ef0e2-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ef0e2-145">publisher</span></span>|<span data-ttu-id="ef0e2-146">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-146">String</span></span>|<span data-ttu-id="ef0e2-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-147">The publisher of the app.</span></span> <span data-ttu-id="ef0e2-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ef0e2-149">largeIcon</span></span>|[<span data-ttu-id="ef0e2-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ef0e2-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ef0e2-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ef0e2-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef0e2-153">createdDateTime</span></span>|<span data-ttu-id="ef0e2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef0e2-154">DateTimeOffset</span></span>|<span data-ttu-id="ef0e2-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-155">The date and time the app was created.</span></span> <span data-ttu-id="ef0e2-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef0e2-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ef0e2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef0e2-158">DateTimeOffset</span></span>|<span data-ttu-id="ef0e2-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ef0e2-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ef0e2-161">isFeatured</span></span>|<span data-ttu-id="ef0e2-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef0e2-162">Boolean</span></span>|<span data-ttu-id="ef0e2-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ef0e2-164">privacyInformationUrl</span></span>|<span data-ttu-id="ef0e2-165">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-165">String</span></span>|<span data-ttu-id="ef0e2-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-166">The privacy statement Url.</span></span> <span data-ttu-id="ef0e2-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ef0e2-168">informationUrl</span></span>|<span data-ttu-id="ef0e2-169">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-169">String</span></span>|<span data-ttu-id="ef0e2-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-170">The more information Url.</span></span> <span data-ttu-id="ef0e2-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-172">owner</span><span class="sxs-lookup"><span data-stu-id="ef0e2-172">owner</span></span>|<span data-ttu-id="ef0e2-173">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-173">String</span></span>|<span data-ttu-id="ef0e2-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-174">The owner of the app.</span></span> <span data-ttu-id="ef0e2-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-176">developer</span><span class="sxs-lookup"><span data-stu-id="ef0e2-176">developer</span></span>|<span data-ttu-id="ef0e2-177">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-177">String</span></span>|<span data-ttu-id="ef0e2-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-178">The developer of the app.</span></span> <span data-ttu-id="ef0e2-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-180">notes</span><span class="sxs-lookup"><span data-stu-id="ef0e2-180">notes</span></span>|<span data-ttu-id="ef0e2-181">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-181">String</span></span>|<span data-ttu-id="ef0e2-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-182">Notes for the app.</span></span> <span data-ttu-id="ef0e2-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ef0e2-184">uploadState</span></span>|<span data-ttu-id="ef0e2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ef0e2-185">Int32</span></span>|<span data-ttu-id="ef0e2-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-186">The upload state.</span></span> <span data-ttu-id="ef0e2-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ef0e2-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ef0e2-188">publishingState</span></span>|[<span data-ttu-id="ef0e2-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ef0e2-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ef0e2-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-190">The publishing state for the app.</span></span> <span data-ttu-id="ef0e2-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ef0e2-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef0e2-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ef0e2-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ef0e2-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ef0e2-194">usedLicenseCount</span></span>|<span data-ttu-id="ef0e2-195">Int32</span><span class="sxs-lookup"><span data-stu-id="ef0e2-195">Int32</span></span>|<span data-ttu-id="ef0e2-196">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-196">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="ef0e2-197">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ef0e2-197">totalLicenseCount</span></span>|<span data-ttu-id="ef0e2-198">Int32</span><span class="sxs-lookup"><span data-stu-id="ef0e2-198">Int32</span></span>|<span data-ttu-id="ef0e2-199">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-199">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="ef0e2-200">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="ef0e2-200">releaseDateTime</span></span>|<span data-ttu-id="ef0e2-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef0e2-201">DateTimeOffset</span></span>|<span data-ttu-id="ef0e2-202">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-202">The VPP application release date and time.</span></span>|
|<span data-ttu-id="ef0e2-203">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ef0e2-203">appStoreUrl</span></span>|<span data-ttu-id="ef0e2-204">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-204">String</span></span>|<span data-ttu-id="ef0e2-205">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-205">The store URL.</span></span>|
|<span data-ttu-id="ef0e2-206">licensingType</span><span class="sxs-lookup"><span data-stu-id="ef0e2-206">licensingType</span></span>|[<span data-ttu-id="ef0e2-207">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="ef0e2-207">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="ef0e2-208">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-208">The supported License Type.</span></span>|
|<span data-ttu-id="ef0e2-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ef0e2-209">applicableDeviceType</span></span>|[<span data-ttu-id="ef0e2-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ef0e2-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="ef0e2-211">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-211">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="ef0e2-212">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="ef0e2-212">vppTokenOrganizationName</span></span>|<span data-ttu-id="ef0e2-213">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-213">String</span></span>|<span data-ttu-id="ef0e2-214">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-214">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="ef0e2-215">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ef0e2-215">vppTokenAccountType</span></span>|[<span data-ttu-id="ef0e2-216">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ef0e2-216">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="ef0e2-217">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-217">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="ef0e2-218">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-218">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="ef0e2-219">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-219">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="ef0e2-220">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="ef0e2-220">vppTokenAppleId</span></span>|<span data-ttu-id="ef0e2-221">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-221">String</span></span>|<span data-ttu-id="ef0e2-222">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-222">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ef0e2-223">bundleId</span><span class="sxs-lookup"><span data-stu-id="ef0e2-223">bundleId</span></span>|<span data-ttu-id="ef0e2-224">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-224">String</span></span>|<span data-ttu-id="ef0e2-225">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-225">The Identity Name.</span></span>|
|<span data-ttu-id="ef0e2-226">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="ef0e2-226">vppTokenId</span></span>|<span data-ttu-id="ef0e2-227">String</span><span class="sxs-lookup"><span data-stu-id="ef0e2-227">String</span></span>|<span data-ttu-id="ef0e2-228">Идентификатор VPP маркер, связанный с этого приложения.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-228">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="ef0e2-229">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="ef0e2-229">revokeLicenseActionResults</span></span>|<span data-ttu-id="ef0e2-230">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ef0e2-230">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="ef0e2-231">Результаты отозвать действия лицензии на это приложение.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-231">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="ef0e2-232">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef0e2-232">Response</span></span>
<span data-ttu-id="ef0e2-233">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-233">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef0e2-234">Пример</span><span class="sxs-lookup"><span data-stu-id="ef0e2-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef0e2-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef0e2-235">Request</span></span>
<span data-ttu-id="ef0e2-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef0e2-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1951

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ef0e2-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef0e2-237">Response</span></span>
<span data-ttu-id="ef0e2-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ef0e2-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2059

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```





