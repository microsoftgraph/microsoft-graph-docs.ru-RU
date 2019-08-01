---
title: Update iosVppApp
description: Обновление свойств объекта iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9f3fed75c969533436e9dbed628afa66107f59d0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002498"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="18e12-103">Update iosVppApp</span><span class="sxs-lookup"><span data-stu-id="18e12-103">Update iosVppApp</span></span>

> <span data-ttu-id="18e12-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18e12-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18e12-105">Обновление свойств объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-105">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18e12-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="18e12-106">Prerequisites</span></span>
<span data-ttu-id="18e12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18e12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18e12-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18e12-109">Permission type</span></span>|<span data-ttu-id="18e12-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18e12-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18e12-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18e12-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18e12-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18e12-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18e12-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18e12-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18e12-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18e12-114">Not supported.</span></span>|
|<span data-ttu-id="18e12-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18e12-115">Application</span></span>|<span data-ttu-id="18e12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18e12-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18e12-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18e12-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="18e12-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18e12-118">Request headers</span></span>
|<span data-ttu-id="18e12-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18e12-119">Header</span></span>|<span data-ttu-id="18e12-120">Значение</span><span class="sxs-lookup"><span data-stu-id="18e12-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18e12-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18e12-121">Authorization</span></span>|<span data-ttu-id="18e12-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18e12-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18e12-123">Accept</span><span class="sxs-lookup"><span data-stu-id="18e12-123">Accept</span></span>|<span data-ttu-id="18e12-124">application/json</span><span class="sxs-lookup"><span data-stu-id="18e12-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18e12-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18e12-125">Request body</span></span>
<span data-ttu-id="18e12-126">В теле запроса добавьте представление объекта [iosVppApp](../resources/intune-apps-iosvppapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18e12-126">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="18e12-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-127">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="18e12-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="18e12-128">Property</span></span>|<span data-ttu-id="18e12-129">Тип</span><span class="sxs-lookup"><span data-stu-id="18e12-129">Type</span></span>|<span data-ttu-id="18e12-130">Описание</span><span class="sxs-lookup"><span data-stu-id="18e12-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18e12-131">id</span><span class="sxs-lookup"><span data-stu-id="18e12-131">id</span></span>|<span data-ttu-id="18e12-132">String</span><span class="sxs-lookup"><span data-stu-id="18e12-132">String</span></span>|<span data-ttu-id="18e12-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="18e12-133">Key of the entity.</span></span> <span data-ttu-id="18e12-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-135">displayName</span><span class="sxs-lookup"><span data-stu-id="18e12-135">displayName</span></span>|<span data-ttu-id="18e12-136">Строка</span><span class="sxs-lookup"><span data-stu-id="18e12-136">String</span></span>|<span data-ttu-id="18e12-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="18e12-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="18e12-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-139">description</span><span class="sxs-lookup"><span data-stu-id="18e12-139">description</span></span>|<span data-ttu-id="18e12-140">Строка</span><span class="sxs-lookup"><span data-stu-id="18e12-140">String</span></span>|<span data-ttu-id="18e12-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="18e12-141">The description of the app.</span></span> <span data-ttu-id="18e12-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-143">publisher</span><span class="sxs-lookup"><span data-stu-id="18e12-143">publisher</span></span>|<span data-ttu-id="18e12-144">String</span><span class="sxs-lookup"><span data-stu-id="18e12-144">String</span></span>|<span data-ttu-id="18e12-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="18e12-145">The publisher of the app.</span></span> <span data-ttu-id="18e12-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="18e12-147">largeIcon</span></span>|[<span data-ttu-id="18e12-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="18e12-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="18e12-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="18e12-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="18e12-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18e12-151">createdDateTime</span></span>|<span data-ttu-id="18e12-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18e12-152">DateTimeOffset</span></span>|<span data-ttu-id="18e12-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="18e12-153">The date and time the app was created.</span></span> <span data-ttu-id="18e12-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18e12-155">lastModifiedDateTime</span></span>|<span data-ttu-id="18e12-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18e12-156">DateTimeOffset</span></span>|<span data-ttu-id="18e12-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="18e12-157">The date and time the app was last modified.</span></span> <span data-ttu-id="18e12-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="18e12-159">isFeatured</span></span>|<span data-ttu-id="18e12-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="18e12-160">Boolean</span></span>|<span data-ttu-id="18e12-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="18e12-162">privacyInformationUrl</span></span>|<span data-ttu-id="18e12-163">String</span><span class="sxs-lookup"><span data-stu-id="18e12-163">String</span></span>|<span data-ttu-id="18e12-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="18e12-164">The privacy statement Url.</span></span> <span data-ttu-id="18e12-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="18e12-166">informationUrl</span></span>|<span data-ttu-id="18e12-167">String</span><span class="sxs-lookup"><span data-stu-id="18e12-167">String</span></span>|<span data-ttu-id="18e12-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="18e12-168">The more information Url.</span></span> <span data-ttu-id="18e12-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-170">owner</span><span class="sxs-lookup"><span data-stu-id="18e12-170">owner</span></span>|<span data-ttu-id="18e12-171">String</span><span class="sxs-lookup"><span data-stu-id="18e12-171">String</span></span>|<span data-ttu-id="18e12-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="18e12-172">The owner of the app.</span></span> <span data-ttu-id="18e12-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-174">developer</span><span class="sxs-lookup"><span data-stu-id="18e12-174">developer</span></span>|<span data-ttu-id="18e12-175">String</span><span class="sxs-lookup"><span data-stu-id="18e12-175">String</span></span>|<span data-ttu-id="18e12-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="18e12-176">The developer of the app.</span></span> <span data-ttu-id="18e12-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-178">notes</span><span class="sxs-lookup"><span data-stu-id="18e12-178">notes</span></span>|<span data-ttu-id="18e12-179">String</span><span class="sxs-lookup"><span data-stu-id="18e12-179">String</span></span>|<span data-ttu-id="18e12-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="18e12-180">Notes for the app.</span></span> <span data-ttu-id="18e12-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18e12-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="18e12-182">publishingState</span></span>|[<span data-ttu-id="18e12-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="18e12-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="18e12-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="18e12-184">The publishing state for the app.</span></span> <span data-ttu-id="18e12-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="18e12-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="18e12-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18e12-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="18e12-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="18e12-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="18e12-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="18e12-188">usedLicenseCount</span></span>|<span data-ttu-id="18e12-189">Int32</span><span class="sxs-lookup"><span data-stu-id="18e12-189">Int32</span></span>|<span data-ttu-id="18e12-190">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="18e12-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="18e12-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="18e12-191">totalLicenseCount</span></span>|<span data-ttu-id="18e12-192">Int32</span><span class="sxs-lookup"><span data-stu-id="18e12-192">Int32</span></span>|<span data-ttu-id="18e12-193">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="18e12-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="18e12-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="18e12-194">releaseDateTime</span></span>|<span data-ttu-id="18e12-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18e12-195">DateTimeOffset</span></span>|<span data-ttu-id="18e12-196">Дата и время выпуска приложения, на которое распространяется программа VPP.</span><span class="sxs-lookup"><span data-stu-id="18e12-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="18e12-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="18e12-197">appStoreUrl</span></span>|<span data-ttu-id="18e12-198">String</span><span class="sxs-lookup"><span data-stu-id="18e12-198">String</span></span>|<span data-ttu-id="18e12-199">URL-адрес магазина.</span><span class="sxs-lookup"><span data-stu-id="18e12-199">The store URL.</span></span>|
|<span data-ttu-id="18e12-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="18e12-200">licensingType</span></span>|[<span data-ttu-id="18e12-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="18e12-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="18e12-202">Поддерживаемый тип лицензии.</span><span class="sxs-lookup"><span data-stu-id="18e12-202">The supported License Type.</span></span>|
|<span data-ttu-id="18e12-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="18e12-203">applicableDeviceType</span></span>|[<span data-ttu-id="18e12-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="18e12-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="18e12-205">Применимый тип устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="18e12-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="18e12-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="18e12-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="18e12-207">Строка</span><span class="sxs-lookup"><span data-stu-id="18e12-207">String</span></span>|<span data-ttu-id="18e12-208">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="18e12-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="18e12-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="18e12-209">vppTokenAccountType</span></span>|[<span data-ttu-id="18e12-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="18e12-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="18e12-211">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="18e12-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="18e12-212">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="18e12-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="18e12-213">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="18e12-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="18e12-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="18e12-214">vppTokenAppleId</span></span>|<span data-ttu-id="18e12-215">String</span><span class="sxs-lookup"><span data-stu-id="18e12-215">String</span></span>|<span data-ttu-id="18e12-216">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="18e12-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="18e12-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="18e12-217">bundleId</span></span>|<span data-ttu-id="18e12-218">String</span><span class="sxs-lookup"><span data-stu-id="18e12-218">String</span></span>|<span data-ttu-id="18e12-219">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="18e12-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="18e12-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="18e12-220">Response</span></span>
<span data-ttu-id="18e12-221">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosVppApp](../resources/intune-apps-iosvppapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="18e12-221">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18e12-222">Пример</span><span class="sxs-lookup"><span data-stu-id="18e12-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="18e12-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="18e12-223">Request</span></span>
<span data-ttu-id="18e12-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18e12-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18e12-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="18e12-225">Response</span></span>
<span data-ttu-id="18e12-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18e12-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



