---
title: Update iosVppApp
description: Обновление свойств объекта iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 26b2977cc8066dc6f43fac72c13597db10bd5d4a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974128"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="a05bc-103">Update iosVppApp</span><span class="sxs-lookup"><span data-stu-id="a05bc-103">Update iosVppApp</span></span>

> <span data-ttu-id="a05bc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a05bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a05bc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a05bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a05bc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a05bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a05bc-107">Обновление свойств объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-107">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a05bc-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a05bc-108">Prerequisites</span></span>
<span data-ttu-id="a05bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a05bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a05bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a05bc-111">Permission type</span></span>|<span data-ttu-id="a05bc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a05bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a05bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a05bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a05bc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a05bc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a05bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a05bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a05bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a05bc-116">Not supported.</span></span>|
|<span data-ttu-id="a05bc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a05bc-117">Application</span></span>|<span data-ttu-id="a05bc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a05bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a05bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a05bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a05bc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a05bc-120">Request headers</span></span>
|<span data-ttu-id="a05bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a05bc-121">Header</span></span>|<span data-ttu-id="a05bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a05bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a05bc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a05bc-123">Authorization</span></span>|<span data-ttu-id="a05bc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a05bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a05bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a05bc-125">Accept</span></span>|<span data-ttu-id="a05bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a05bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a05bc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a05bc-127">Request body</span></span>
<span data-ttu-id="a05bc-128">В теле запроса добавьте представление объекта [iosVppApp](../resources/intune-apps-iosvppapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a05bc-128">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="a05bc-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-129">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="a05bc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a05bc-130">Property</span></span>|<span data-ttu-id="a05bc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a05bc-131">Type</span></span>|<span data-ttu-id="a05bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a05bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a05bc-133">id</span><span class="sxs-lookup"><span data-stu-id="a05bc-133">id</span></span>|<span data-ttu-id="a05bc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a05bc-134">String</span></span>|<span data-ttu-id="a05bc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a05bc-135">Key of the entity.</span></span> <span data-ttu-id="a05bc-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a05bc-137">displayName</span></span>|<span data-ttu-id="a05bc-138">String</span><span class="sxs-lookup"><span data-stu-id="a05bc-138">String</span></span>|<span data-ttu-id="a05bc-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a05bc-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a05bc-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-141">описание</span><span class="sxs-lookup"><span data-stu-id="a05bc-141">description</span></span>|<span data-ttu-id="a05bc-142">String</span><span class="sxs-lookup"><span data-stu-id="a05bc-142">String</span></span>|<span data-ttu-id="a05bc-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a05bc-143">The description of the app.</span></span> <span data-ttu-id="a05bc-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a05bc-145">publisher</span></span>|<span data-ttu-id="a05bc-146">String</span><span class="sxs-lookup"><span data-stu-id="a05bc-146">String</span></span>|<span data-ttu-id="a05bc-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a05bc-147">The publisher of the app.</span></span> <span data-ttu-id="a05bc-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a05bc-149">largeIcon</span></span>|[<span data-ttu-id="a05bc-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a05bc-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a05bc-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a05bc-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a05bc-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a05bc-153">createdDateTime</span></span>|<span data-ttu-id="a05bc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a05bc-154">DateTimeOffset</span></span>|<span data-ttu-id="a05bc-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a05bc-155">The date and time the app was created.</span></span> <span data-ttu-id="a05bc-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a05bc-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a05bc-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a05bc-158">DateTimeOffset</span></span>|<span data-ttu-id="a05bc-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a05bc-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a05bc-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a05bc-161">isFeatured</span></span>|<span data-ttu-id="a05bc-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a05bc-162">Boolean</span></span>|<span data-ttu-id="a05bc-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a05bc-164">privacyInformationUrl</span></span>|<span data-ttu-id="a05bc-165">String</span><span class="sxs-lookup"><span data-stu-id="a05bc-165">String</span></span>|<span data-ttu-id="a05bc-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a05bc-166">The privacy statement Url.</span></span> <span data-ttu-id="a05bc-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a05bc-168">informationUrl</span></span>|<span data-ttu-id="a05bc-169">String</span><span class="sxs-lookup"><span data-stu-id="a05bc-169">String</span></span>|<span data-ttu-id="a05bc-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a05bc-170">The more information Url.</span></span> <span data-ttu-id="a05bc-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-172">owner</span><span class="sxs-lookup"><span data-stu-id="a05bc-172">owner</span></span>|<span data-ttu-id="a05bc-173">String</span><span class="sxs-lookup"><span data-stu-id="a05bc-173">String</span></span>|<span data-ttu-id="a05bc-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a05bc-174">The owner of the app.</span></span> <span data-ttu-id="a05bc-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-176">developer</span><span class="sxs-lookup"><span data-stu-id="a05bc-176">developer</span></span>|<span data-ttu-id="a05bc-177">String</span><span class="sxs-lookup"><span data-stu-id="a05bc-177">String</span></span>|<span data-ttu-id="a05bc-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a05bc-178">The developer of the app.</span></span> <span data-ttu-id="a05bc-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-180">notes</span><span class="sxs-lookup"><span data-stu-id="a05bc-180">notes</span></span>|<span data-ttu-id="a05bc-181">String</span><span class="sxs-lookup"><span data-stu-id="a05bc-181">String</span></span>|<span data-ttu-id="a05bc-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="a05bc-182">Notes for the app.</span></span> <span data-ttu-id="a05bc-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a05bc-184">uploadState</span></span>|<span data-ttu-id="a05bc-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a05bc-185">Int32</span></span>|<span data-ttu-id="a05bc-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="a05bc-186">The upload state.</span></span> <span data-ttu-id="a05bc-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a05bc-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="a05bc-188">publishingState</span></span>|[<span data-ttu-id="a05bc-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a05bc-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a05bc-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="a05bc-190">The publishing state for the app.</span></span> <span data-ttu-id="a05bc-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a05bc-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a05bc-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a05bc-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a05bc-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a05bc-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a05bc-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a05bc-194">usedLicenseCount</span></span>|<span data-ttu-id="a05bc-195">Int32</span><span class="sxs-lookup"><span data-stu-id="a05bc-195">Int32</span></span>|<span data-ttu-id="a05bc-196">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="a05bc-196">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="a05bc-197">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a05bc-197">totalLicenseCount</span></span>|<span data-ttu-id="a05bc-198">Int32</span><span class="sxs-lookup"><span data-stu-id="a05bc-198">Int32</span></span>|<span data-ttu-id="a05bc-199">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="a05bc-199">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="a05bc-200">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="a05bc-200">releaseDateTime</span></span>|<span data-ttu-id="a05bc-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a05bc-201">DateTimeOffset</span></span>|<span data-ttu-id="a05bc-202">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="a05bc-202">The VPP application release date and time.</span></span>|
|<span data-ttu-id="a05bc-203">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a05bc-203">appStoreUrl</span></span>|<span data-ttu-id="a05bc-204">String</span><span class="sxs-lookup"><span data-stu-id="a05bc-204">String</span></span>|<span data-ttu-id="a05bc-205">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="a05bc-205">The store URL.</span></span>|
|<span data-ttu-id="a05bc-206">licensingType</span><span class="sxs-lookup"><span data-stu-id="a05bc-206">licensingType</span></span>|[<span data-ttu-id="a05bc-207">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="a05bc-207">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="a05bc-208">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="a05bc-208">The supported License Type.</span></span>|
|<span data-ttu-id="a05bc-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="a05bc-209">applicableDeviceType</span></span>|[<span data-ttu-id="a05bc-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="a05bc-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="a05bc-211">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="a05bc-211">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="a05bc-212">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="a05bc-212">vppTokenOrganizationName</span></span>|<span data-ttu-id="a05bc-213">String</span><span class="sxs-lookup"><span data-stu-id="a05bc-213">String</span></span>|<span data-ttu-id="a05bc-214">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="a05bc-214">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="a05bc-215">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="a05bc-215">vppTokenAccountType</span></span>|[<span data-ttu-id="a05bc-216">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="a05bc-216">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="a05bc-217">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="a05bc-217">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="a05bc-218">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="a05bc-218">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="a05bc-219">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="a05bc-219">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="a05bc-220">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="a05bc-220">vppTokenAppleId</span></span>|<span data-ttu-id="a05bc-221">String</span><span class="sxs-lookup"><span data-stu-id="a05bc-221">String</span></span>|<span data-ttu-id="a05bc-222">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="a05bc-222">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a05bc-223">bundleId</span><span class="sxs-lookup"><span data-stu-id="a05bc-223">bundleId</span></span>|<span data-ttu-id="a05bc-224">String</span><span class="sxs-lookup"><span data-stu-id="a05bc-224">String</span></span>|<span data-ttu-id="a05bc-225">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a05bc-225">The Identity Name.</span></span>|
|<span data-ttu-id="a05bc-226">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="a05bc-226">vppTokenId</span></span>|<span data-ttu-id="a05bc-227">Строка</span><span class="sxs-lookup"><span data-stu-id="a05bc-227">String</span></span>|<span data-ttu-id="a05bc-228">Идентификатор VPP маркер, связанный с этого приложения.</span><span class="sxs-lookup"><span data-stu-id="a05bc-228">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="a05bc-229">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="a05bc-229">revokeLicenseActionResults</span></span>|<span data-ttu-id="a05bc-230">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a05bc-230">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="a05bc-231">Результаты отозвать действия лицензии на это приложение.</span><span class="sxs-lookup"><span data-stu-id="a05bc-231">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="a05bc-232">Ответ</span><span class="sxs-lookup"><span data-stu-id="a05bc-232">Response</span></span>
<span data-ttu-id="a05bc-233">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a05bc-233">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a05bc-234">Пример</span><span class="sxs-lookup"><span data-stu-id="a05bc-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="a05bc-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="a05bc-235">Request</span></span>
<span data-ttu-id="a05bc-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a05bc-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1903

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

### <a name="response"></a><span data-ttu-id="a05bc-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="a05bc-237">Response</span></span>
<span data-ttu-id="a05bc-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a05bc-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





