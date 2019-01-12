---
title: Update iosVppApp
description: Обновление свойств объекта iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 777b92cb56c61889f463b28c14e54c8300491242
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27992079"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="a4ac9-103">Update iosVppApp</span><span class="sxs-lookup"><span data-stu-id="a4ac9-103">Update iosVppApp</span></span>

> <span data-ttu-id="a4ac9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4ac9-105">Обновление свойств объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-105">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4ac9-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a4ac9-106">Prerequisites</span></span>
<span data-ttu-id="a4ac9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4ac9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4ac9-109">Permission type</span></span>|<span data-ttu-id="a4ac9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4ac9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4ac9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4ac9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4ac9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4ac9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4ac9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4ac9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4ac9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-114">Not supported.</span></span>|
|<span data-ttu-id="a4ac9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4ac9-115">Application</span></span>|<span data-ttu-id="a4ac9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4ac9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4ac9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="a4ac9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4ac9-118">Request headers</span></span>
|<span data-ttu-id="a4ac9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4ac9-119">Header</span></span>|<span data-ttu-id="a4ac9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a4ac9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4ac9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4ac9-121">Authorization</span></span>|<span data-ttu-id="a4ac9-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a4ac9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4ac9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a4ac9-123">Accept</span></span>|<span data-ttu-id="a4ac9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a4ac9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4ac9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a4ac9-125">Request body</span></span>
<span data-ttu-id="a4ac9-126">В теле запроса добавьте представление объекта [iosVppApp](../resources/intune-apps-iosvppapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-126">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="a4ac9-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-127">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="a4ac9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4ac9-128">Property</span></span>|<span data-ttu-id="a4ac9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a4ac9-129">Type</span></span>|<span data-ttu-id="a4ac9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a4ac9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4ac9-131">id</span><span class="sxs-lookup"><span data-stu-id="a4ac9-131">id</span></span>|<span data-ttu-id="a4ac9-132">Строка</span><span class="sxs-lookup"><span data-stu-id="a4ac9-132">String</span></span>|<span data-ttu-id="a4ac9-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-133">Key of the entity.</span></span> <span data-ttu-id="a4ac9-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a4ac9-135">displayName</span></span>|<span data-ttu-id="a4ac9-136">String</span><span class="sxs-lookup"><span data-stu-id="a4ac9-136">String</span></span>|<span data-ttu-id="a4ac9-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a4ac9-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-139">описание</span><span class="sxs-lookup"><span data-stu-id="a4ac9-139">description</span></span>|<span data-ttu-id="a4ac9-140">String</span><span class="sxs-lookup"><span data-stu-id="a4ac9-140">String</span></span>|<span data-ttu-id="a4ac9-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-141">The description of the app.</span></span> <span data-ttu-id="a4ac9-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-143">publisher</span><span class="sxs-lookup"><span data-stu-id="a4ac9-143">publisher</span></span>|<span data-ttu-id="a4ac9-144">String</span><span class="sxs-lookup"><span data-stu-id="a4ac9-144">String</span></span>|<span data-ttu-id="a4ac9-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-145">The publisher of the app.</span></span> <span data-ttu-id="a4ac9-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a4ac9-147">largeIcon</span></span>|[<span data-ttu-id="a4ac9-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a4ac9-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a4ac9-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a4ac9-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4ac9-151">createdDateTime</span></span>|<span data-ttu-id="a4ac9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4ac9-152">DateTimeOffset</span></span>|<span data-ttu-id="a4ac9-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-153">The date and time the app was created.</span></span> <span data-ttu-id="a4ac9-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4ac9-155">lastModifiedDateTime</span></span>|<span data-ttu-id="a4ac9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4ac9-156">DateTimeOffset</span></span>|<span data-ttu-id="a4ac9-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-157">The date and time the app was last modified.</span></span> <span data-ttu-id="a4ac9-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a4ac9-159">isFeatured</span></span>|<span data-ttu-id="a4ac9-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4ac9-160">Boolean</span></span>|<span data-ttu-id="a4ac9-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a4ac9-162">privacyInformationUrl</span></span>|<span data-ttu-id="a4ac9-163">String</span><span class="sxs-lookup"><span data-stu-id="a4ac9-163">String</span></span>|<span data-ttu-id="a4ac9-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-164">The privacy statement Url.</span></span> <span data-ttu-id="a4ac9-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a4ac9-166">informationUrl</span></span>|<span data-ttu-id="a4ac9-167">String</span><span class="sxs-lookup"><span data-stu-id="a4ac9-167">String</span></span>|<span data-ttu-id="a4ac9-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-168">The more information Url.</span></span> <span data-ttu-id="a4ac9-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-170">owner</span><span class="sxs-lookup"><span data-stu-id="a4ac9-170">owner</span></span>|<span data-ttu-id="a4ac9-171">String</span><span class="sxs-lookup"><span data-stu-id="a4ac9-171">String</span></span>|<span data-ttu-id="a4ac9-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-172">The owner of the app.</span></span> <span data-ttu-id="a4ac9-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-174">developer</span><span class="sxs-lookup"><span data-stu-id="a4ac9-174">developer</span></span>|<span data-ttu-id="a4ac9-175">String</span><span class="sxs-lookup"><span data-stu-id="a4ac9-175">String</span></span>|<span data-ttu-id="a4ac9-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-176">The developer of the app.</span></span> <span data-ttu-id="a4ac9-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-178">notes</span><span class="sxs-lookup"><span data-stu-id="a4ac9-178">notes</span></span>|<span data-ttu-id="a4ac9-179">String</span><span class="sxs-lookup"><span data-stu-id="a4ac9-179">String</span></span>|<span data-ttu-id="a4ac9-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-180">Notes for the app.</span></span> <span data-ttu-id="a4ac9-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4ac9-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="a4ac9-182">publishingState</span></span>|[<span data-ttu-id="a4ac9-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a4ac9-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a4ac9-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-184">The publishing state for the app.</span></span> <span data-ttu-id="a4ac9-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a4ac9-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a4ac9-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a4ac9-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a4ac9-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a4ac9-188">usedLicenseCount</span></span>|<span data-ttu-id="a4ac9-189">Int32</span><span class="sxs-lookup"><span data-stu-id="a4ac9-189">Int32</span></span>|<span data-ttu-id="a4ac9-190">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="a4ac9-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a4ac9-191">totalLicenseCount</span></span>|<span data-ttu-id="a4ac9-192">Int32</span><span class="sxs-lookup"><span data-stu-id="a4ac9-192">Int32</span></span>|<span data-ttu-id="a4ac9-193">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="a4ac9-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="a4ac9-194">releaseDateTime</span></span>|<span data-ttu-id="a4ac9-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4ac9-195">DateTimeOffset</span></span>|<span data-ttu-id="a4ac9-196">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="a4ac9-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a4ac9-197">appStoreUrl</span></span>|<span data-ttu-id="a4ac9-198">String</span><span class="sxs-lookup"><span data-stu-id="a4ac9-198">String</span></span>|<span data-ttu-id="a4ac9-199">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-199">The store URL.</span></span>|
|<span data-ttu-id="a4ac9-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="a4ac9-200">licensingType</span></span>|[<span data-ttu-id="a4ac9-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="a4ac9-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="a4ac9-202">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-202">The supported License Type.</span></span>|
|<span data-ttu-id="a4ac9-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="a4ac9-203">applicableDeviceType</span></span>|[<span data-ttu-id="a4ac9-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="a4ac9-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="a4ac9-205">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="a4ac9-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="a4ac9-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="a4ac9-207">String</span><span class="sxs-lookup"><span data-stu-id="a4ac9-207">String</span></span>|<span data-ttu-id="a4ac9-208">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="a4ac9-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="a4ac9-209">vppTokenAccountType</span></span>|[<span data-ttu-id="a4ac9-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="a4ac9-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="a4ac9-211">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="a4ac9-212">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="a4ac9-213">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="a4ac9-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="a4ac9-214">vppTokenAppleId</span></span>|<span data-ttu-id="a4ac9-215">String</span><span class="sxs-lookup"><span data-stu-id="a4ac9-215">String</span></span>|<span data-ttu-id="a4ac9-216">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a4ac9-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="a4ac9-217">bundleId</span></span>|<span data-ttu-id="a4ac9-218">String</span><span class="sxs-lookup"><span data-stu-id="a4ac9-218">String</span></span>|<span data-ttu-id="a4ac9-219">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="a4ac9-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4ac9-220">Response</span></span>
<span data-ttu-id="a4ac9-221">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-221">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4ac9-222">Пример</span><span class="sxs-lookup"><span data-stu-id="a4ac9-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4ac9-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4ac9-223">Request</span></span>
<span data-ttu-id="a4ac9-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1222

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
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
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
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="a4ac9-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4ac9-225">Response</span></span>
<span data-ttu-id="a4ac9-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a4ac9-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1394

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
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
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
  "bundleId": "Bundle Id value"
}
```



